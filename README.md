
# The comparison of classical optical flow estimation algorithms with algorithms using artificial neural networks.

Abstract of MA thesis:

The thesis presents a comparative analysis of traditional approaches to optical flow estimation with modern methods using artificial neural networks. Six classical algorithms (Lukas-Kanade, Farneback, Horn-Schunck/DualTV-L1, DenseRLOF, PCAFlow, Brox) and five deep learning methods (PWCNet, FastFlowNet, HD3, RAFT, RAFT-small) were analyzed. Classic algorithms are known for low hardware requirements, mathematical clarity, and limited precision in complex scenarios. Neural methods achieve significantly greater accuracy but require substantial GPU resources to function correctly. It's not possible to determine the best method clearly. The choice of algorithm should consider the specific requirements of the application, such as real-time use or high precision.

## Authors

- [@t0pzz](https://www.github.com/t0pzz), M. Sc. Konrad Kruk


## Software 

- pycharm proffesional,
- python 3.13,
- opencv 4.12.0-dev (compiled with cuda),
- ptlflow,
- pandas,
- numpy, 
- os, 
- time, 
- pynvml (nvidia api), 
- psutil.
## Hardware
- RTX 2060 6 GB Gainward Phantom
- Ryzen 7 5800x (watercooled)
- 2 x 16 GB DDR4 RAM @3600 MHz, Dual Channel
- NVMe SSD 
- Windows 11 Home 24H1 
## Datasets

 - [MPI - SINTEL](http://sintel.is.tue.mpg.de/)
 - [KITTI (flow2015)](https://www.cvlibs.net/datasets/kitti/eval_scene_flow.php?benchmark=flow)
 - [Flying Chairs2](https://lmb.informatik.uni-freiburg.de/resources/datasets/FlyingChairs.en.html)


## Algorithms

Traditional methods were implemented using OpenCV (including contrib modules with CUDA acceleration), whereas modern approaches were built with the PTLFlow library.

| Traditional | Moddern (AI) |
| --- | --- |
| PyrLK|RAFT_large|
|Farneback|RAFT_small|
| PCAFlow | HD3 |
| DenseRLOF|FastFlowNet|
|DualTV_L1|PWCNet|
|Brox|  | 


## Features

- Preprocessing data eg. File paths -> pandas -> read all as GRAYSCALE
- Data aquisition & post-processing,
- Hardware monitoring,
- Optical flow  estimation using both traditional and modern approaches, also using CNNs,
- Measuring typical optical flow estimation metrics - EPE, AE (occ,noc),
- Restults visualization


## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

