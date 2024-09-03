---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
## Introduction

We are proud to announce a new large scale multimodal event-based human pose/action dataset `CDEHP Dataset`(**C**olor **D**epth **E**vent **H**uman **P**ose) with Color (RGB), Depth, and Event modules. `CDEHP Dataset` uses RGB, Depth, and Event cameras to simultaneously capture actions from a variety of subjects, bringing a new multimodal benchmark to the research of event-based human pose estimation and action recognition. Of course, you can also use this dataset to carry out research work in the RGB-D field or event camera field. If you are interested to build a multimodal event-based dataset, please refer to [How to Make](/how-to-make).

## Dataset Statistic

|  Scenes   | # Subjects  |  # Actions |  Modality |  # Frames of Train Set   |  # Frames of Test Set | # Total Frames |
| :-------: | :----: | :---: | :------------------: | :---: |:---: |:---: |
|  Outdoor        |  10  |  13 |  RGB, Depth, Event |   82.785K   |  18.486K |101.271K|
|  Indoor         |  20  |  25 |  RGB, Depth, Event |   30.232K   |  14.643K |  44.875K|
|  Outdoor&Indoor |  30  |  25 |  RGB, Depth, Event |   113.017K   |  33.129K |  146.146K|

## Action Class

#### Indoor Actions (13)

|  ID   | Action Name  |  ID   |   Action Name    |  ID   |     Action Name     |  ID   |       Action Name       |
| :---: | :----------: | :---: | :--------------: | :---: | :-----------------: | :---: | :---------------------: |
|  A1   |   walking    |  A2   |  squat jump   |  A3   |       boxing        |  A4   |       picking up        |
|  A5   | jumping jack |  A6   | crotch high five |  A7   |      sweeping       |  A8   | alternate jumping lunge |
|  A9   |   big jump   |  A10  |   sit-up jump    |  A11  | shuttlecock kicking |  A12  |        throwing         |
|  A13  |   spinning   |       |                  |       |                     |       |                         |

#### Outdoor Actions (25)

|  ID   |   Action Name    |  ID   |  Action Name  |  ID   |       Action Name       |  ID   |       Action Name       |
| :---: | :--------------: | :---: | :-----------: | :---: | :---------------------: |:---: | :---------------------: |
|  A1  | walking           |  A2  |     running    |  A3  | squat jump         |  A4  |        frog jump |        
|  A5  | jump fwd/bwd/left/right  |  A6  |      boxing      |  A7  |  picking up   |  A8  |  cartwheel           |
|  A9  |      jumping jack  |  A10  | crotch high five |  A11  |   crawling    |  A12  |   rope skipping   |      
|  A13 |   sweeping         |  A14  |     mopping      |  A15  |    cycling    |  A16  | alternate jumping lunge | 
|  A17 |        big jump    |  A18  |   sit-up jump    |  A19  |    kicking    |  A20  |    jump shot        |  
|  A21 |   shuttlecock kicking   |  A22  |     spinning     |  A23  |   throwing    |  A24  |        long jump   |
|  A25 |        burpee          |      |             |       |            |       |                        |


## Visualization of Action Samples

![Indoor samples of all action classes](/assets/Indoor.png)
![Outdoor samples of all action classes](/assets/Outdoor.png)

## Citation

To cite our datasets, please refer to:

```text
@article{Zhanpeng Shao:2024,
   TITLE      = {A temporal densely connected recurrent network for event-based human pose estimation},
   JOURNAL    = {Pattern Recognition},
   VOLUME     = {147},
   PAGES      = {110048},
   YEAR       = {2024},
   ISSN       = {0031-3203},
   DOI        = {https://doi.org/10.1016/j.patcog.2023.110048},
   URL        = {https://www.sciencedirect.com/science/article/pii/S0031320323007458},
   AUTHOR     = {Zhanpeng Shao and Xueping Wang and Wen Zhou and Wuzhen Wang and Jianyu Yang and Youfu Li},
   KEYWORDS   = {Event signal, Human pose estimation, Dense connections, Recurrent network, Dataset},
}
```

## Use Dataset

* The size of the `CDEHP Dataset` is large. We have prepared a couple of official distribution channels. Please follow the [download page](/download) to get the dataset and annotation files, please remember to verify the size of each fragment.
* In order to make a fair comparison, `CDEHP Dataset` has been officially divided into the training set and the verification set for your information. **Please follow this protocol to ensure the fairness of the comparison.**


## Projects

* [Website](https://github.com/CDEHP-Dataset/cdehp-dataset.github.io): This website is for the dataset distribution and any feedback.
* [PyCeleX5](https://github.com/CDEHP-Dataset/PyCeleX5): CelePixel CeleX5-MIPI C++ API Wrapper for Python 3.
* [Calibration-Tool](https://github.com/CDEHP-Dataset/Calibration-Tool): Twin calibration tools for RGB cameras and event cameras.
* [Recording-Tool](https://github.com/CDEHP-Dataset/Calibration-Tool): Recording tools for making CDEHP-Dataset.
* [Annotation-Tool](https://github.com/CDEHP-Dataset/Annotation-Tool): Labeling tools for making CDEHP-Dataset.

## Team

<div class="row">
   <div class="cell">
      <img class="member_avatar" src="/assets/perry.jpg" alt="Zhanpeng Shao" />
      <p class="member_name"><a href="https://perryshao.github.io/">Zhanpeng Shao</a></p>
      <p>Associate Professor with College of Information Science and Engineering, Hunan Normal University. Specifically interested in activity understanding in videos.</p>
   </div>

   <div class="cell">
      <img class="member_avatar" src="/assets/xavier.jpg" alt="Wen Zhou" />
      <p class="member_name"><a herf="https://github.com/xavier-zw">Wen Zhou</a></p>
      <p>Obtained a Master's degree from Zhejiang University of Technology.</p>
   </div>

   <div class="cell">
      <img class="member_avatar" src="/assets/kuretru.jpg" alt="Wuzhen Wang" />
      <p class="member_name"><a href="https://github.com/kuretru">Wuzhen Wang</a></p>
      <p>Obtained a Master's degree from Zhejiang University of Technology, currently work for ByteDance.</p>
   </div>
</div>

## Contact

* If you have any question, please raise an issue on the project's [Github repository](https://github.com/CDEHP-Dataset/cdehp-dataset.github.io/issues).
* If you are looking for further discussion and opportunities please contact [Prof. Z.P. Shao](https://perryshao.github.io/).
