# IEEE BigData Cup 2024: Building Extraction Generalization Challenge

### Team: Double Y (Yi Jie Wong, Yin Loon Khor)

This [competition](https://www.kaggle.com/competitions/building-extraction-generalization-2024/overview) embarks on this challenge by utilizing a building footprint dataset from the Tokyo area as the primary training set, with plans to extend testing to other Japanese regions. This approach aims to inspire the development of models with robust generalization capabilities, capable of overcoming the hurdles of automatic building footprint detection and extraction across various landscapes. Overcoming this challenge signifies the creation of a novel approach for efficient, cost-effective, and precise building footprint extraction at a national level with minimal regional data, showcasing its potential applicability worldwide.

## Our Solution

- We proposed using customized YOLOv8m-seg instance segmentation model for the task.
- We leveraged open-source Microsoft Building Footprint Dataset to expand the diversity of the training dataset.
- To improve the label-efficiency, we proposed using segmentation-guided diffusion as our diffusion augmentation pipeline to create synthetic dataset for the YOLOv8 training, without relying extra dataset.
- Our solution ranked 1st out of all participating teams! 🏅
- Feel free to check our technical report [here](https://doubley-begc2024.github.io/)

## Top 5 Standings
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <table border="1">
        <tr>
            <th>Rank #</th>
            <th>Team</th>
            <th>Private F1 Score</th>
        </tr>
        <tr>
            <td>1</td>
            <td>DoubleY (our Team)</td>
            <td>0.89711</td>
        </tr>
        <tr>
            <td>2</td>
            <td>BDASL</td>
            <td>0.68453</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Big Ben</td>
            <td>0.60649</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Edge 1234</td>
            <td>0.58565</td>
        </tr>
        <tr>
            <td>5</td>
            <td>The Curio Cat</td>
            <td>0.51963</td>
        </tr>
    </table>
</body>
</html>

## Cite this repository

Our paper has been accepted by IEEE BigData 2024! Please cite our preprint if this repo helps your research.
```
@article{Wong2024,
   author = {Yi Jie Wong and Yin-Loon Khor and Mau-Luen Tham and Ban-Hoe Kwan and Anissa Mokraoui and Yoong Choon Chang},
   doi = {10.36227/TECHRXIV.173091008.80781383/V1},
   institution = {Techrxiv},
   journal = {Authorea Preprints},
   month = {11},
   publisher = {Authorea},
   title = {Cross-City Building Instance Segmentation: From More Data to Diffusion-Augmentation},
   url = {https://www.techrxiv.org/users/844381/articles/1235896-cross-city-building-instance-segmentation-from-more-data-to-diffusion-augmentation?commit=b5f5b583761fbb4a7a1e5c99b9c3dae7c50f11c7},
   year = {2024},
}
```
