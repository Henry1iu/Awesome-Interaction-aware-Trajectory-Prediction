# Awesome Trajectory Prediction for Vehicles and Pedestrain
![Version](https://img.shields.io/badge/Version-0.0.1-blue) 
![LastUpdated](https://img.shields.io/badge/LastUpdated-2021.09-lightgrey.svg)
![Topic](https://img.shields.io/badge/Topic-trajectory--prediction-yellow.svg?logo=github) 
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<p align="center">
  <img width="250" src="https://camo.githubusercontent.com/1131548cf666e1150ebd2a52f44776d539f06324/68747470733a2f2f63646e2e7261776769742e636f6d2f73696e647265736f726875732f617765736f6d652f6d61737465722f6d656469612f6c6f676f2e737667"
	"Awesome!">
</p>

This is a checklist of some research materials, including public datasets, surveys, papers with public codes, and blogs, on trajectory prediction.
The literatures are categorized by the type of target agent (pedestrain or vehicle) and the (deep learning) modelling approaches.

**Maintainers**: {[**Jianbang Liu**](https://henry1iu.github.io/homepage/), Xinyu Mao} @ EE Department, The Chinese University of Hong Kong

**Emails**: {henryliu, maoxinyu}@connect.cuhk.edu.hk

Please feel free to pull request to add new resources or send emails to us for questions, discussion and collaborations.

**Note**: This repository is built based on [**Awesome Interaction-aware Behavior and Trajectory Prediction**](https://github.com/jiachenli94/Awesome-Interaction-aware-Trajectory-Prediction).
Thanks for the maintainers' contribution. 

Please consider citing our work if you found this repo useful:

```


```

### Table of Contents

<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave: orderedList:0 -->
- [**Datasets**](#datasets)
	- [Vehicles and Traffic](#vehicles-and-traffic)
	- [Pedestrians](#pedestrians)
	
- [**Literature and Codes**](#literature-and-codes)
	- [Survey Papers](#survey-papers)
	- [Vehicles & Traffic](#intelligent-vehicles-traffic)
	- [Pedestrians](#pedestrians-1)
	- [Benchmark and Evaluation Metrics](#benchmark-and-evaluation-metrics)
	- [Others](#others)
<!-- /TOC -->

## **Datasets**

### Vehicles and Traffic

|                           Dataset                            |            Agents            |         Scenarios         |        Sensors         |
| :----------------------------------------------------------: | :--------------------------: | :-----------------------: | :--------------------: |
|      [INTERACTION](http://www.interaction-dataset.com/)      | Vehicles / cyclists/ people  | Roundabout / intersection |     Camera     |
|        [KITTI](http://www.cvlibs.net/datasets/kitti/)        | Vehicles / cyclists/ people  |   Highway / rural areas   |     Camera / LiDAR     |
|           [HighD](https://www.highd-dataset.com/)            |           Vehicles           |          Highway          |         Camera         |
|           [InD](https://www.ind-dataset.com/)                |           Vehicles           |          Highway          |         Camera         |
|           [RoundD](https://www.round-dataset.com/)           |           Vehicles           |          Highway          |         Camera         |
| [NGSIM](https://ops.fhwa.dot.gov/trafficanalysistools/ngsim.htm) |           Vehicles       |          Highway          |         Camera         |
| [Cyclists](http://www.gavrila.net/Datasets/Daimler_Pedestrian_Benchmark_D/Tsinghua-Daimler_Cyclist_Detec/tsinghua-daimler_cyclist_detec.html) |           Cyclists           |           Urban           |         Camera         |
|            [nuScenes](https://www.nuscenes.org/)             |           Vehicles           |           Urban           | Camera / LiDAR / RADAR |
|          [BDD100k](https://bdd-data.berkeley.edu/)           | Vehicles / cyclists / people |      Highway / urban      |         Camera         |
| [Apolloscapes](http://apolloscape.auto/?source=post_page---------------------------) | Vehicles / cyclists / people |           Urban           |         Camera         |
| [Udacity](https://github.com/udacity/self-driving-car/tree/master/datasets) |           Vehicles           |           Urban           |         Camera         |
|      [Cityscapes](https://www.cityscapes-dataset.com/)       |       Vehicles/ people       |           Urban           |         Camera         |
| [Stanford Drone](http://cvgl.stanford.edu/projects/uav_data/) | Vehicles / cyclists/ people |           Urban           |         Camera         |
|           [Argoverse](https://www.argoverse.org/)            |      Vehicles / people       |           Urban           |     Camera / LiDAR     |
| [TRAF](https://gamma.umd.edu/researchdirections/autonomousdriving/trafdataset) |      Vehicles/buses/cyclists/bikes / people/animals       |           Urban           |     Camera      |
| [Lyft Level 5](https://level5.lyft.com/dataset/)             | Vehicles/cyclists/people     | Urban                     | Camera/ LiDAR   |

### Pedestrians

|                           Dataset                            |           Agents            |       Scenarios       |    Sensors     |
| :----------------------------------------------------------: | :-------------------------: | :-------------------: | :------------: |
| [UCY](https://graphics.cs.ucy.ac.cy/research/downloads/crowd-data) |           People      |    Zara / students    |     Camera     |
|       [ETH](http://www.vision.ee.ethz.ch/en/datasets/)       |           People            |         Urban         |     Camera     |
|              [VIRAT](http://www.viratdata.org/)              |      People / vehicles      |         Urban         |     Camera     |
|        [KITTI](http://www.cvlibs.net/datasets/kitti/)        | Vehicles / cyclists/ people | Highway / rural areas | Camera / LiDAR |
|     [ATC](https://irc.atr.jp/crest2010_HRI/ATC_dataset/)     |           People            |    Shopping center    |  Range sensor  |
| [Daimler](http://www.gavrila.net/Datasets/Daimler_Pedestrian_Benchmark_D/daimler_pedestrian_benchmark_d.html) |           People            |  From moving vehicle  |     Camera     |
| [Central Station](http://www.ee.cuhk.edu.hk/~xgwang/grandcentral.html) |       People      |    Inside station     |     Camera     |
| [Town Center](http://www.robots.ox.ac.uk/ActiveVision/Research/Projects/2009bbenfold_headpose/project.html#datasets) |           People            |     Urban street      |     Camera     |
| [Edinburgh](http://homepages.inf.ed.ac.uk/rbf/FORUMTRACKING/) |           People           |         Urban         |     Camera     |
|   [Cityscapes](https://www.cityscapes-dataset.com/login/)    |      Vehicles/ people       |         Urban         |     Camera     |
|           [Argoverse](https://www.argoverse.org/)            |      Vehicles / people      |         Urban         | Camera / LiDAR |
| [Stanford Drone](http://cvgl.stanford.edu/projects/uav_data/) | Vehicles / cyclists/ people |         Urban         |     Camera     |
|           [TrajNet](http://trajnet.stanford.edu/)            |           People            |         Urban         |     Camera     |
| [PIE](http://data.nvision2.eecs.yorku.ca/PIE_dataset/)       |           People            |         Urban         |     Camera     |
| [ForkingPaths](https://next.cs.cmu.edu/multiverse/index.html) |           People           |         Urban / Simulation         |     Camera     |
| [TrajNet++](https://www.aicrowd.com/challenges/trajnet-a-trajectory-forecasting-challenge) |           People            |         Urban         |     Camera     |

## **Literature and Codes**

### Survey Papers

- Modeling and Prediction of Human Driver Behavior: A Survey, 2020. [[paper](https://arxiv.org/abs/2006.08832)]
- Human Motion Trajectory Prediction: A Survey, 2019. [[paper](https://arxiv.org/abs/1905.06113)]
- A literature review on the prediction of pedestrian behavior in urban scenarios, ITSC 2018. [[paper](https://ieeexplore.ieee.org/document/8569415)]
- Survey on Vision-Based Path Prediction. [[paper](https://link.springer.com/chapter/10.1007/978-3-319-91131-1_4)]
- Autonomous vehicles that interact with pedestrians: A survey of theory and practice. [[paper](https://arxiv.org/abs/1805.11773)]
- Trajectory data mining: an overview. [[paper](https://dl.acm.org/citation.cfm?id=2743025)]
- A survey on motion prediction and risk assessment for intelligent vehicles. [[paper](https://robomechjournal.springeropen.com/articles/10.1186/s40648-014-0001-z)]

**Notes**:
```
We use following tag to indicte the modelling detail of the approach:

(Scene: {Graph, BEV, None}): The representatioin of scene context information{Graph, BEV}, or not include {None}.
(Hist: {MLP(Attention), CNN, RNN, GNN}): This historical observation of the agent trajectory is encoded by {MLP, CNN, RNN, GNN} module.
(InterX: {MLP(Attention), CNN, RNN, GNN, None}): The explict interaction modeling of the approach. 
```

### Vehicles & Traffic
- Deep Neural Networks for Markovian Interactive Scene Prediction in Highway Scenarios, IEEE IV 2017. (**Hist**: MLP)(**Scene**: None)(**InterX**: None) [[paper](https://ieeexplore.ieee.org/document/7995797)]
- DESIRE: Distant Future Prediction in Dynamic Scenes with Interacting Agents, CVPR 2017. (**Hist**: RNN)(**Scene**: CNN)(**InterX**: CNN) [[paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Lee_DESIRE_Distant_Future_CVPR_2017_paper.pdf)][[code](https://github.com/tdavchev/DESIRE)]
- VectorNet: Encoding HD Maps and Agent Dynamics, CVPR 2020. (**Hist**: MLP)(**Scene**: Graph)(**InterX**: Attention) [[paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Gao_VectorNet_Encoding_HD_Maps_and_Agent_Dynamics_From_Vectorized_Representation_CVPR_2020_paper.pdf)][[code](https://github.com/Henry1iu/TNT-Trajectory-Predition)]
- TNT: Target-driveN Trajectory Prediction, CoRL 2020. (**Hist**: MLP) (**Scene**: Graph) (**InterX**: Attention) [[paper](https://arxiv.org/abs/2008.08294)][[code](https://github.com/Henry1iu/TNT-Trajectory-Predition)]
- 

### Pedestrians


### Benchmark and Evaluation Metrics
- OpenTraj: Assessing Prediction Complexity in Human Trajectories Datasets, ACCV 2020. [[paper](https://arxiv.org/abs/2010.00890)][[code](https://github.com/crowdbotp/OpenTraj)]
- Testing the Safety of Self-driving Vehicles by Simulating Perception and Prediction, ECCV 2020. [[paper](https://arxiv.org/abs/2008.06020)]
- PIE: A Large-Scale Dataset and Models for Pedestrian Intention Estimation and Trajectory Prediction, ICCV 2019. [[paper](http://openaccess.thecvf.com/content_ICCV_2019/papers/Rasouli_PIE_A_Large-Scale_Dataset_and_Models_for_Pedestrian_Intention_Estimation_ICCV_2019_paper.pdf)]
- Towards a fatality-aware benchmark of probabilistic reaction prediction in highly interactive driving scenarios, ITSC 2018. [[paper](https://arxiv.org/abs/1809.03478)]
- How good is my prediction? Finding a similarity measure for trajectory prediction evaluation, ITSC 2017. [[paper](http://ieeexplore.ieee.org/document/8317825/)]
- Trajnet: Towards a benchmark for human trajectory prediction. [[website](http://trajnet.epfl.ch/)]

### Others
