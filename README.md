# Awesome Radar Perception
A curated list of radar datasets, detection, tracking and fusion. <br>Keep updating.<br>Author: Yi Zhou<br>Contact: zhouyi1023@tju.edu.cn
<br>Update some public-available codes, see [useful_codes.md](./useful_codes.md)

🚩I have published a review paper on radar perception. Please see the link below. It is open access. If you find the contents are useful, please cite this paper in your work. I will keep updating this repository for the latest works in the radar perception field.

## [Towards Deep Radar Perception for Autonomous Driving: Datasets, Methods, and Challenges](https://www.mdpi.com/1424-8220/22/11/4208)

## The 41-page slides associated with this paper: [Link](https://www.slideshare.net/YiZhou66/slidesdeepradarperceptionforautonomousdrivingpdf) ; [Link for China Mainland](https://www.aliyundrive.com/s/CZ3SKqY3U4w) 

Radar perception is getting popular. More and more researchers from computer vision, intelligent vehicle and robotics are starting to enter this field. I hope my review article and this repository can be a good starting point for these newcomers.
<div align="center">
    <img class="aligncenter" src="images/radar_stat.png"/>
</div>
<br/>


## Radar Datasets
In my [review paper](https://www.mdpi.com/1424-8220/22/11/4208), there is a table with more detials.


### Conventional Radar Datasets for Autonomous Driving
| Dataset | Radar Type | Data Type| Annotation | Link |
| ---- |----| ---- | ---- | ---- |
| nuScenes | Continental ARS408 x5 | Sparse PC | 3D bbox, TrackID | [Website](https://www.nuscenes.org/) |
| DENSE| 77Ghz Long-Range Radar | Sparse PC | 3D bbox |[Website](https://www.uni-ulm.de/en/in/driveu/projects/dense-datasets) |
| PixSet| TI AWR1843| Sparse PC | 3D bbox, TrackID|  [Website](https://leddartech.com/solutions/leddar-pixset-dataset/)|
| Radar Scenes | 77GHz Middle-Range Radar x4 | Dense PC |2D point-wise, TrackID| [Website](https://radar-scenes.com/)|
| Pointillism | 2 TI AWR 1443 | PC | 3D bbox | [Github](https://github.com/Kshitizbansal/pointillism-multi-radar-data) |
| Zendar SAR | SAR | ADC, RD, PC|Pointwise Mask of Moving Vehicle |[Github](https://github.com/ZendarInc/ZendarSDK) |


<br>Brief Review: nuScenes, DENSE and Pixset are for sensor fusion, but not particularly address the role of radar. Radar scenes provides point-wise annotations for radar point cloud, but has no other modalities. Pointillism uses 2 radars with overlapped view. Zendar seems no longer available for downloading.


### Pre-CFAR Datasets for Detection
| Dataset | Radar Type | Data Type| Annotation | Link |
| ---- |----| ---- | ---- | ---- |
| CRUW |  TI AWR1843 Ultra Short Range | RA | Pointlevel Object |[Website](https://www.cruwdataset.org/home)|
| CARRADA | TI AWR1843 Short Range | RA,RD,RAD | Pointwise, 2D bbox, Mask | [Website](https://arthurouaknine.github.io/codeanddata/carrada)|
| RADDet | TI AWR1843 | RAD | 3D bbox for RAD tensor | [Github](https://github.com/ZhangAoCanada/RADDet) |
| RaDICaL | TI IWR1443 | ADC | 2D bbox | [Website](https://publish.illinois.edu/radicaldata/)|
| GhentVRU | TI AWR1243 Short Range | RAD | Segmentation Mask for VRUs| [Paper](https://ieeexplore.ieee.org/document/9294399) |


<br>Brief Review: CARRADA is too simple, CRUW uses RA maps, RADDet provides annotations for RAD tensor, RADICaL provides raw ADC data and signal processing toolboxes, GhentVRU can be accssed by contacting with authors.

### 4D Radar Datasets for Detection
| Dataset | Radar Type | Data Type| Annotation | Link |
| ---- |----| ---- | ---- | ---- |
| Astyx  Hires2019 | Astyx 6455 HiRes Middel Range| PC | 3D bbox|[Dateset](https://github.com/under-the-radar/radar_dataset_astyx)|
| View-of-Delft | ZF FRGen21 Short Range| PC | 3D bbox |[Website](https://intelligent-vehicles.org/datasets/view-of-delft/)|
| RADIal | Valeo Middel Range DDM | ADC,RAD,PC | Point-level Vehicle; Open Space Mask|[Github](https://github.com/valeoai/RADIal)|
| TJ4DRadSet | Oculii Eagle Long Range | PC |  3D bbox, TrackID| [Paper](https://arxiv.org/abs/2204.13483) |


<br>Brief Review: Astyx is small, VoD focuses on VRU classification, RADIal's annotation is coarse but provides raw data, TJ4D features for its long range detection. Both VoD and TJ4D are not yet public available.

### Specific Tasks
| Dataset | Radar Type | Task | Link |
| ---- |----| ---- | ---- |
| HawkEye | SAR | Static vehicle classification | [Website](https://jaydeng1019.github.io/HawkEye/)|
| PREVENTION | Conti ARS308 + SRR208 x2 | Trajectory Prediction | [Website](https://prevention-dataset.uah.es/)|
| SCORP | 76GHz | Open space segmentation | [Website](https://sensorcortek.ai/paper-and-datasets/) |
| Ghost | 77GHz long range *2  | Ghost object detection | [Github](https://github.com/flkraus/ghosts) |
| DopNet | 24Ghz | Gesture Classification | [Website](http://dop-net.com/)
| Radar signatures of human activities  | Soli |  Indoor human activities | [Dataset](http://researchdata.gla.ac.uk/848/) |
| Solinteraction Data | Soli | Tangible interactions| [Github](https://github.com/tcboy88/solinteractiondata) |
| GROUNDED | Ground Penetrating Radar | Localization | [Website](https://lgprdata.com/)|
|FloW Dataset | TI AWR1843 | Floating waste detection | [Website](http://orca-tech.cn/datasets/FloW/Introduction) |


### Odometry and Localization
| Dataset | Radar Type | Task | Link |
| ---- |----| ---- | ---- | 
| Oxford Radar Robocar | Navtech Spinning Radar |  Odometry | [Website](https://oxford-robotics-institute.github.io/radar-robotcar-dataset/) |
|RADIATE| Navtech Spinning  Radar | Odometry, Detection, Tracking | [Website](http://pro.hw.ac.uk/radiate/doc/dataset/)|
| MulRan | Navtech Spinning  Radar | Place Recognition |[Website](https://sites.google.com/view/mulran-pr/dataset)|
| Boreas | Navtech Spinning  Radar|   Long-term Odometry, Localization, Detection | [Website](https://www.boreas.utias.utoronto.ca/#/)|
| EU Long-term Dataset | Conti ARS 308 | Long-term SLAM | [Website](https://epan-utbm.github.io/utbm_robocar_dataset/)|
| ColoRadar | TI AWR2243 Cascade + AWR1843 |Odometry |  [Website](https://arpg.github.io/coloradar/) |
| USVInland | TI AWR1843 | SLAM in inland waterways, Water segmentation| [Website](http://orca-tech.cn/datasets/USVInland/Introduction) |
| Endeavour Radar Dataset | Conti ARS 430 x5 | Odometry | [Website](https://gloryhry.github.io/2021/06/25/Endeavour_Radar_Dataset.html)|



## Radar Toolbox and ROS Node

### TI Signal Processing SDK:
RaDICaL's Toolbox: [SDK](https://github.com/moodoki/radical_sdk); <br>PyRapid: [SDK](http://radar.alizadeh.ca);<br>OpenRadar : [SDK](https://github.com/presenseradar/openradar);<br>Pymmw: [SDK](https://github.com/m6c7l/pymmw);<br>Open radar initiative: [SDK](https://github.com/openradarinitiative);<br>RADIal's Emptyband-DDM Script: [Code](https://github.com/valeoai/RADIal/tree/main/SignalProcessing)

### Official SDK:
NXP Premium Radar SDK: [Link](https://www.nxp.com/design/automotive-software-and-tools/premium-radar-sdk-advanced-radar-processing:PREMIUM-RADAR-SDK);<br>TI mmWAVE Studio: [Link](https://www.ti.com/tool/MMWAVE-STUDIO)<br>TI Toolbox: [Link](https://dev.ti.com/tirex/explore/node?node=AHJY4qNCowO17wH-P2ICKQ)<br>Matlab Radar Toolbox: [Link](https://uk.mathworks.com/products/radar.html)

### ROS:
Ainstein Radar ROS Node: [ROS Node](https://github.com/AinsteinAI/ainstein_radar);<br>Continental ARS 408 ROS Node: [ROS Node](https://gitlab.com/ApexAI/autowareclass2020/-/tree/master/code/src/09_Perception_Radar/Radar-Hands-On-WS);<br>TI mmWave ROS Driver: [Guide](https://dev.ti.com/tirex/explore/node?node=ADINBw2NDaxb6JeW7V-lMQ__VLyFKFf__LATEST&search=ROS);<br>RaDICaL's TI ROS Node: [ROS Node](https://github.com/moodoki/iwr_raw_rosnode);<br>UoA's TI ROS Package: [ROS Node](https://github.com/radar-lab/ti_mmwave_rospkg)



## Seminars and Workshops
### Radar
* 2021 ICRA Radar Perception for All-Weather Autonomy [[Website]](https://sites.google.com/view/radar-robotics/home)
* 2021 ICASSP Recent Advances in mmWave Radar Sensing for Autonomous Vehicles [[Website]](https://www.2021.ieeeicassp.org/Papers/ViewSession_MS.asp?Sessionid=1280)
* Radar in Action Series by Fraunhofer FHR [[Video]](https://www.youtube.com/hashtag/radarinaction)
* IEEE AESS Virtual Distinguished Lecturer Webinar Series [[Website]](https://ieee-aess.org/activities/educational-activities/distinguished-lecturers)
* Journal of Radar Webinar Series (in Chinese) [[Video]](https://space.bilibili.com/1288394672)

* Markus Gardill: Automotive Radar – An Overview on State-of-the-Art Technology [[Video]](https://www.youtube.com/watch?v=P-C6_4ceY64&t=2416s)
* Markus Gardill: Automotive Radar – A Signal Processing Perspective on Current Technology and Future Systems [[Video]](https://www.youtube.com/watch?v=IxoPYhXY30k&t=11s)[[Slides]](https://cloud.gardill.net/s/tjoSLSB7fXWTEBb)
* Francesco Fioranelli: Radar Old but Gold- current research challenges and activities in radar micro-Doppler signatures [[Video]](https://www.youtube.com/watch?v=ysL6rk-4L9o&list=PLa5-fgjZm9MtJBtb6M3YplIDSdgr1m94n&index=3)
* Andrej Karpathy from Tesla:  [[Video]](https://www.youtube.com/watch?v=g6bOwQdCJrc)
* Ole Schumann: Radar Perception for Automated Driving – Data and Methods [[Video]](https://www.youtube.com/watch?v=UQL7_Zy2Kjg&t=73s)
* Sani Ronen from Arbe: Using AI layer to transform HR radar into insights for Autonomous Driving applications [[Video]](https://www.youtube.com/watch?v=TtJW-c02YH8)
* Stefan Haag: Co-Development of Automatic Annotation for ML and Sensor Fusion Improvement System  [[Video]](https://www.youtube.com/watch?v=ANbmXg2TxlE)
* Arthur Ouaknine: Deep Learning & Scene Understanding for autonomous vehicle [[Video]](https://www.youtube.com/watch?v=sOOvnTCnhPg)
* Paul Newman: The Road to Anywhere-Autonomy [[Video]](https://www.youtube.com/watch?v=MzYQMRG9HW0)
* Jaime Lien: Soli: Millimeter-wave radar for touchless interaction [[Video]](https://www.youtube.com/watch?v=JFr8Whnx630)
* Accelerating end-to-end Development of Software-Defined 4D Imaging Radar [[Videp]](https://www.youtube.com/watch?v=QPoj1zM2vCs)
* Radar-Imaging - An Introduction to the Theory Behind [[Video]](https://www.youtube.com/watch?v=ej2smyTZLHE)
* NXP - Radar Experts Discuss the Evolution of Automotive Radar [[Video]](https://www.youtube.com/watch?v=RfJiiSlesyE&t=347s)
* Need to Successfully Design a Milimeter-Wave Automotive Radar Antenna? [[Video]](https://www.youtube.com/watch?v=0lK8qJSWY_c)
* Webinar SAR Imaging using Ancortek’s Software Defined Radars [[Video]](https://www.youtube.com/watch?v=BMSVvQJYCIs)

### Uncertainty Quantification
* History of Bayesian Neural Networks [[Video]](https://www.youtube.com/watch?v=FD8l2vPU5FY&list=PLa5-fgjZm9Mv-aNvqc-V40UgSF6fBeOwY&index=8)
* Uncertainty and Out-of-Distribution Robustness in Deep Learning [[Video]](https://www.youtube.com/watch?v=ssD7jNDIL2c&list=PLa5-fgjZm9Mv-aNvqc-V40UgSF6fBeOwY&index=12)


## Recommended Books and Tutorials
### Radar Textbook
* Fundamentals of Radar Signal Processing by Mark A. Richard
* Radar Systems Analysis and Design using Matlab by Bassem R. Mahafza 
### Signal Processing
* [Introduction to mmwaveSensing: FMCW Radars](https://training.ti.com/sites/default/files/docs/mmwaveSensing-FMCW-offlineviewing_0.pdf)
* [The fundamentals of millimeter wave sensors](https://www.ti.com/lit/wp/spyy005a/spyy005a.pdf?ts=1619205965675)
* [Signal Processing for TDM MIMO FMCW Millimeter-Wave Radar Sensors](https://ieeexplore.ieee.org/document/9658500)
### Waveform
* [Analysis and Comparison of MIMO Radar Waveforms](https://ieeexplore.ieee.org/document/9658500)
### Quadrature Signal
* [Quadrature Signals: Complex, But Not Complicated](https://dspguru.com/dsp/tutorials/quadrature-signals/) 
* [Using a complex-baseband architecture in FMCW radar systems](https://www.ti.com/lit/wp/spyy007/spyy007.pdf)
### MIMO
* [TI MIMO radar](https://www.ti.com/lit/an/swra554a/swra554a.pdf)
* [TI EmptyBand DDM (Chinese)]() [(English)]()
### Conformal Prediction
* [A Gentle Introduction to Conformal Prediction and Distribution-Free Uncertainty Quantification](https://arxiv.org/abs/2107.07511)

## Review Papers

Radar vs Lidar
* [Comparative Analysis of Radar and Lidar Technologies for Automotive Applications](https://ieeexplore.ieee.org/document/9760734/)
* [Testing and Validation of Automotive Point-Cloud Sensors in Adverse Weather Conditions](https://www.mdpi.com/2076-3417/9/11/2341)

Antenna:
* [Millimeter-Wave Technology for Automotive Radar Sensors in the 77 GHz Frequency Band](https://ieeexplore.ieee.org/document/6127923)
* [Antenna Concepts for Millimeter-Wave Automotive Radar Sensors](https://ieeexplore.ieee.org/document/6165323)


Radar Signal Processing:
* General: [The Rise of Radar for Autonomous Vehicles: Signal Processing Solutions and Future Research Directions](https://ieeexplore.ieee.org/document/8828025/)
* Signal Processing: [Radar-on-Chip/in-Package in Autonomous Driving Vehicles and Intelligent Transport Systems](https://ieeexplore.ieee.org/document/9369027)
* Signal Processing: [Automotive Radars A review of signal processing techniques](https://ieeexplore.ieee.org/abstract/document/7870764
* PseudoNoise(PN): [On the Safe Road Toward Autonomous Driving: Phase Noise Monitoring in Radar Sensors for Functional Safety Compliance](https://ieeexplore.ieee.org/document/8827996)
* MIMO: [MIMO Radar for Advanced Driver-Assistance Systems and Autonomous Driving: Advantages and Challenges](https://ieeexplore.ieee.org/document/9127853)
* Digital Radar: [High-Performance Automotive Radar: A Review of Signal Processing Algorithms and Modulation Schemes](https://ieeexplore.ieee.org/document/8828004)
* Interference: [Radar Interference Mitigation for Automated Driving: Exploring Proactive Strategies](https://ieeexplore.ieee.org/document/9127843)
* Interference: [Interference in Automotive Radar Systems: Characteristics, Mitigation Techniques, and Current and Future Research](https://ieeexplore.ieee.org/document/8828037)
* Micro-Doppler: [Micro-Doppler Effect in Radar: Phenomenon, Model, and Simulation Study](https://ieeexplore.ieee.org/document/1603402)


Deep Learning Applications for Radar:
* Overview: [Automotive Radar Signal Processing: Research Directions and Practical Challenges](https://ieeexplore.ieee.org/document/9369027)
* Overview: [Millimeter Wave FMCW RADARs for perception, recognition and localization in automotive applications: A survey](https://ieeexplore.ieee.org/abstract/document/9760104)
* Interference: [Interference Suppression Using Deep Learning: Current Approaches and Open Challenges](https://arxiv.org/abs/2112.08988)
* DoA: [A Machine Learning Perspective on Automotive Radar Direction of Arrival Estimation](https://ieeexplore.ieee.org/abstract/document/9674901)
* Detection: [Application of Deep Learning on Millimeter-Wave Radar Signals: A Review](https://www.mdpi.com/1424-8220/21/6/1951)
* Localization: [MMW Radar-Based Technologies in Autonomous Driving: A Review](https://www.mdpi.com/1424-8220/20/24/7283)
* Fusion: [MmWave Radar and Vision Fusion for Object Detection in Autonomous Driving: A Review](https://www.mdpi.com/1424-8220/22/7/2542)
* Tracking: [On-Road Object Detection and Tracking Based on Radar and Vision Fusion: A Review](https://ieeexplore.ieee.org/document/9506829)
* Semantic Understanding: [Radar for Autonomous Driving – Paradigm Shift from Mere Detection to Semantic Environment Understanding](https://link.springer.com/chapter/10.1007/978-3-658-23751-6_1)
* Detection: [New Challenges for Deep Neural Networks in Automotive Radar Perception An Overview of Current Research Trend](https://www.springerprofessional.de/en/new-challenges-for-deep-neural-networks-in-automotive-radar-perc/19534946)


General Object Detection:
* [3D Object Detection from Images for Autonomous Driving: A Survey](https://arxiv.org/abs/2202.02980)
* [Deep Learning for 3D Point Clouds: A Survey](https://arxiv.org/abs/1912.12033)
* [Attention Mechanisms in Computer Vision: A Survey](https://arxiv.org/abs/2111.07624)


Sensor Fusion:
* To understand Vision: [Object Detection Under Rainy Conditions for Autonomous Vehicles: A Review of State-of-the-Art and Emerging Techniques](https://ieeexplore.ieee.org/document/9307324)
* To understand LiDAR: [Testing and Validation of Automotive Point-Cloud Sensors in Adverse Weather Conditions](https://www.mdpi.com/2076-3417/9/11/2341)
* Learning: [Multi-Modal 3D Object Detection in Autonomous Driving: a Survey](https://arxiv.org/abs/2106.12735)
* Learning: [Deep Multi-Modal Object Detection and Semantic Segmentation for Autonomous Driving: Datasets, Methods, and Challenges](https://ieeexplore.ieee.org/document/9000872)
* Traditional: [Multisensor data fusion: A review of the state-of-the-art](https://www.sciencedirect.com/science/article/abs/pii/S1566253511000558)
* [Information Decomposition of Target Effects from Multi-Source Interactions: Perspectives on Previous, Current and FutureWork](https://www.mdpi.com/1099-4300/20/4/307)


Uncertainty Estimation:
* [A Review and Comparative Study on Probabilistic Object Detection in Autonomous Driving](https://arxiv.org/abs/2011.10671)
* [Aleatoric and Epistemic Uncertainty in Machine Learning: An Introduction to Concepts and Methods](https://link.springer.com/article/10.1007/s10994-021-05946-3)




## Radar Characteristics
### Weather Effects
* [The Impact of Adverse Weather Conditions on Autonomous Vehicles: How Rain, Snow, Fog, and Hail Affect the Performance of a Self-Driving Car](https://ieeexplore.ieee.org/abstract/document/8666747)
* [Seeing through dust and water vapor: Millimeter wave radar sensors for mining applications](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.20166)
* [Analysis of rain clutter detections in commercial 77 GHz automotive radar](https://ieeexplore.ieee.org/abstract/document/8249138)
* [The Perception System of Intelligent Ground Vehicles in All Weather Conditions: A Systematic Literature Review](https://www.mdpi.com/1424-8220/20/22/6532)


### RCS
* 2018-[Review of Radar Classification & RCS Characterisation Techniques for Small UAVs or Drones](http://eprints.gla.ac.uk/164563/)
* 2021-[Machine Learning-Based Target Classification for MMW Radar in Autonomous Driving](https://ieeexplore.ieee.org/document/9319548)

### Reflection Signature
* 2017-[Radar Reflection Characteristics of Vehicles for Contour and Feature Estimation](https://ieeexplore.ieee.org/abstract/document/8126352)
* 2018-[Radar and Lidar Target Signatures of Various Object Types and Evaluation of Extended Object Tracking Methods for Autonomous Driving Applications](https://ieeexplore.ieee.org/abstract/document/8455395)

### Multi-Path
* 2017-[A Novel Target-Height Estimation Approach Using Radar-Wave Multipath Propagation for Automotive Applications](https://ars.copernicus.org/articles/15/61/2017/)
* 2018-[Automotive Radar Multipath Propagation in Uncertain Environments](https://ieeexplore.ieee.org/abstract/document/8570016)
* 2018-[Analysis of Multipath and DOA Detection Using a Fully Polarimetric Automotive Radar](https://www.cambridge.org/core/journals/international-journal-of-microwave-and-wireless-technologies/article/analysis-of-multipath-and-doa-detection-using-a-fully-polarimetric-automotive-radar/C3659FC550A9A4CDDE9ED420B97A6587)
* 2020-[Using Machine Learning to Detect Ghost Images in Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9294631)
* 2020-[Seeing Around Street Corners Non-Line-of-Sight Detection and Tracking In-the-Wild Using Doppler Radar](https://openaccess.thecvf.com/content_CVPR_2020/html/Scheiner_Seeing_Around_Street_Corners_Non-Line-of-Sight_Detection_and_Tracking_In-the-Wild_Using_CVPR_2020_paper.html)
* 2021-[Ghost Target Detection in 3D Radar Data using Point Cloud based Deep Neural Network](https://ieeexplore.ieee.org/abstract/document/9413247)

### Micro-Doppler
* 2006-[Micro-Doppler Effect in Radar: Phenomenon, Model, and Simulation Study](https://ieeexplore.ieee.org/abstract/document/1603402)
* 2020-[New Radar Micro-Doppler Tag for Road Safety Based on the Signature of Rotating Backscatters](https://ieeexplore.ieee.org/abstract/document/9311635)

### Polarimetric
* 2016-[A Polarimetric 76-79 GHz Radar-Frontend for Target Classification in Automotive Use](https://ieeexplore.ieee.org/abstract/document/7824638)
* 2018-[Performance Analysis of 79 GHz Polarimetric Radar Sensors for Autonomous Driving](https://ieeexplore.ieee.org/abstract/document/8249142)
* 2018-[Autonomous Driving Features based on 79 GHz Polarimetric Radar Data](https://ieeexplore.ieee.org/abstract/document/8546632)
* 2019-[Polarimetric Signatures of a Passenger Car](https://ieeexplore.ieee.org/abstract/document/8890117)


## Simulation
* [Diversified Radar Micro-Doppler Simulations as Training Data for Deep Residual Neural Networks](https://ieeexplore.ieee.org/document/8378629)
* [Measurements revealing Challenges in Radar Sensor Modeling for Virtual Validation of Autonomous Driving](https://link.springer.com/chapter/10.1007/978-3-030-58523-5_29)
* [Virtual Radar: Real-Time Millimeter-Wave Radar Sensor Simulation for Perception-Driven Robotics](https://ieeexplore.ieee.org/abstract/document/9387149)
* [Vid2Doppler: Synthesizing Doppler Radar Data from Videos for Training Privacy-Preserving Activity Recognition](https://dl.acm.org/doi/abs/10.1145/3411764.3445138)
* [Scalable and Physical Radar Sensor Simulation for Interacting Digital Twins](https://ieeexplore.ieee.org/abstract/document/9205224)
* [A Multi-Layered Approach for Measuring the Simulation-to-Reality Gap of Radar Perception for Autonomous Driving](https://ieeexplore.ieee.org/document/9564521)

## Generative
* 2017-[Deep Stochastic Radar Models](https://ieeexplore.ieee.org/document/7995697)
* 2020-[GenRadar: Self-supervised Probabilistic Camera Synthesis based on Radar Frequencies](https://arxiv.org/abs/2107.08948)
* 2019-[Automotive radar and camera fusion using Generative Adversarial Networks](https://www.sciencedirect.com/science/article/abs/pii/S1077314219300530)
* 2020-[L2R GAN: LiDAR-to-Radar Translation](https://openaccess.thecvf.com/content/ACCV2020/papers/Wang_L2R_GAN_LiDAR-to-Radar_Translation_ACCV_2020_paper.pdf)
* 2020-[There and Back Again: Learning to Simulate Radar Data for Real-World Applications](https://arxiv.org/abs/2011.14389)


## Calibration
### Radar & Multi Radars
* [Auto-Calibration of Automotive Radars in Operational Mode Using Simultaneous Localisation and Mapping](https://ieeexplore.ieee.org/document/9353252)
* [Multi-Radar Self-Calibration Method using High-Definition Digital Maps for Autonomous Driving](https://ieeexplore.ieee.org/document/8569272/)
### Radar-Camera
* [Obstacle Detection Using Millimeter-wave Radar and Its Visualization on Image Sequence](https://ieeexplore.ieee.org/document/1334537/)
* [Radar and vision sensors calibration for outdoor 3D reconstruction]()
* [Spatio-Temporal Multisensor Calibration Based on Gaussian Processes Moving Object Tracking](https://arxiv.org/abs/1904.04187)
* [Targetless Rotational Auto-Calibration of Radar and Camera for Intelligent Transportation Systems](https://ieeexplore.ieee.org/document/8917135)
* [A Continuous-Time Approach for 3D Radar-to-Camera Extrinsic Calibration](https://arxiv.org/abs/2103.07505)
### Radar-Lidar
* [Extrinsic 6DoF calibration of 3D LiDAR and radar](https://ieeexplore.ieee.org/document/8098688)
* [Extrinsic and Temporal Calibration of Automotive Radar and 3D LiDAR](https://ieeexplore.ieee.org/document/9341715)
* [Automatic Targetless Extrinsic Calibration of Multiple 3D LiDARs and Radars](https://ieeexplore.ieee.org/document/9340866/)
### Radar-Lidar-Camera
* [Extrinsic 6DoF Calibration of a Radar – LiDAR– Camera System Enhanced by Radar Cross Section Estimates Evaluation](https://www.sciencedirect.com/science/article/pii/S0921889018301994)
* [An Joint Extrinsic Calibration Tool for Radar, Camera and Lidar](https://ieeexplore.ieee.org/document/9380784)
* [Online multi-sensor calibration based on moving object tracking](https://www.tandfonline.com/doi/full/10.1080/01691864.2020.1819874)

## Ego Motion
* 2018-[Precise Ego-Motion Estimation with Millimeter-Wave Radar under Diverse and Challenging Conditions](https://ieeexplore.ieee.org/abstract/document/8460687)
* 2019-[An Instantaneous 3D Ego-Velocity Measurement Algorithm for Frequency Modulated Continuous Wave Doppler Radar Data](https://www.proquest.com/openview/0354baf8a7e55480288b5abc6bb52677/1?pq-origsite=gscholar&cbl=18750&diss=y)
* 2020-[Radar-Inertial Ego-Velocity Estimation for Visually Degraded Environments](https://ieeexplore.ieee.org/abstract/document/9196666)
* 2020-[milliEgo: Single-chip mmWave Aided Egomotion Estimation with Deep Sensor Fusion](https://dl.acm.org/doi/abs/10.1145/3384419.3430776?casa_token=-THoSVYXSK0AAAAA:W29x9r07Oow3kwQL8zyj9BtJj6liQLYi0yzsB47PzK7H3B8Mi3LHExeql9h7_5CR8o2EEBMqU7j_DMI)

## Static Objects and Surrounding Environments
### Classification
* 2016-[Potential of Radar for Static Object Classification using Deep Learning Methods](https://ieeexplore.ieee.org/abstract/document/7533931)
* 2017-[Object Classification in Radar Using Ensemble Methods](https://ieeexplore.ieee.org/abstract/document/7918863)
### Segmentation
* 2018-[Semantic Segmentation on Radar Point Clouds](https://ieeexplore.ieee.org/abstract/document/8455344)
* 2019-[Scene Understanding With Automotive Radar](https://ieeexplore.ieee.org/abstract/document/8911477)
* 2019-[Road Scene Understanding by Occupancy Grid Learning from Sparse Radar Clusters using Semantic Segmentation](https://openaccess.thecvf.com/content_ICCVW_2019/html/CVRSUAD/Sless_Road_Scene_Understanding_by_Occupancy_Grid_Learning_from_Sparse_Radar_ICCVW_2019_paper.html)
* 2020-[Semantic Segmentation on 3D Occupancy Grids for Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9229096)
* 2020-[Deep Open Space Segmentation using Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9299052)
* 2020-[Statistical Image Segmentation and Region Classification Approaches for Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9337399)
* 2021-[PolarNet Accelerated Deep Open Space Segmentation Using Automotive Radar in Polar Domain](https://arxiv.org/abs/2103.03387)
### Mapping and Localization 
* 2019-[Probably Unknown Deep Inverse Sensor Modelling Radar](https://ieeexplore.ieee.org/abstract/document/8793263)
* 2019-[Occupancy Grids Generation Using Deep Radar Network for Autonomous Driving](https://ieeexplore.ieee.org/abstract/document/8916897)
* 2020-[Kidnapped Radar Topological Radar Localisation using Rotationally-Invariant Metric Learning](https://ieeexplore.ieee.org/abstract/document/9196682)
* 2020-[RadarSLAM Radar Based Large-Scale SLAM in All Weathers](https://ieeexplore.ieee.org/abstract/document/9341287)
* 2021-[Unsupervised Place Recognition with Deep Embedding Learning over Radar Videos](https://arxiv.org/abs/2106.06703)
* 2020-[Deep Learning for Autonomous and Driver Assistant Systems](https://ruor.uottawa.ca/handle/10393/40852)
* 2020-[A Scalable Framework for Robust Vehicle State Estimation with a Fusion of a Low-Cost IMU, the GNSS, Radar, a Camera and Lidar](https://ieeexplore.ieee.org/abstract/document/9341419)
* 2020-[See Through Smoke: Robust Indoor Mapping with Low-cost mmWave Radar](https://dl.acm.org/doi/abs/10.1145/3386901.3388945?casa_token=lMQ6u0JpykAAAAAA:AyBOL6HY0OWSncmMdssUvXBo31y2vXISKDquU5cMom68xbwWz0s68Tz1OJVhRrL6WpZF-Gz8ntDwD8A)
* 2021-[AutoPlace: Robust Place Recognition with Low-cost Single-chip Automotive Radar](https://arxiv.org/abs/2109.08652)
* 2021-[Do We Need to Compensate for Motion Distortion and Doppler Effects in Spinning Radar Navigation](https://ieeexplore.ieee.org/abstract/document/9327473)
* 2021-[Cross-Modal Contrastive Learning of Representations for Navigation using Lightweight, Low-Cost Millimeter Wave Radar for Adverse Environmental Conditions](https://ieeexplore.ieee.org/abstract/document/9362209)


## Detection of Dynamic Objects
### Clustering
* 2012-[Grid-Based DBSCAN for Clustering Extended Objects in Radar Data](https://ieeexplore.ieee.org/abstract/document/6232167)
* 2016-[Adaptive Clustering for Contour Estimation of Vehicles for High-Resolution Radar](https://ieeexplore.ieee.org/abstract/document/7533930)
* 2018-[Supervised Clustering for Radar Applications On the Way to Radar Instance Segmentation](https://ieeexplore.ieee.org/abstract/document/8443534)
* 2019-[A Multi-Stage Clustering Framework for Automotive Radar Data](https://ieeexplore.ieee.org/abstract/document/8916873)
* 2019-[Robust and Adaptive Radar Elliptical Density-Based Spatial Clustering and labeling for mmWave Radar Point Cloud Data](https://ieeexplore.ieee.org/abstract/document/9048869)
* 2021-[Anomaly Detection in Radar Data Using PointNets](https://ieeexplore.ieee.org/document/9564730)
* 2021-[Fast Rule-Based Clutter Detection in Automotive Radar Data](https://ieeexplore.ieee.org/document/9564776?source=AUTHORALERT&dld=dGp1LmVkdS5jbg%3D%3D)

### Classification of Clusters
* 2015-[Making Bertha See Even More](https://ieeexplore.ieee.org/abstract/document/7161279)
* 2017-[Comparison of Random Forest and Long Short-Term Memory Network Performances in Classification Tasks Using Radar](https://ieeexplore.ieee.org/document/8126350)
* 2018-[Radar-based Feature Design and Multiclass Classification for Road User Recognition](https://ieeexplore.ieee.org/abstract/document/8500607)
* 2019-[Radar-based Road User Classification and Novelty Detection with Recurrent Neural Network Ensembles](https://ieeexplore.ieee.org/abstract/document/8813773)
* 2020-[Off-the-shelf sensor vs. experimental radar - How much resolution is necessary in automotive radar classification](https://ieeexplore.ieee.org/abstract/document/9190338)
* 2021-[Deep Learning for Automotive Object Classification with Radar Reflections](https://ieeexplore.ieee.org/abstract/document/9455334) 

### Sparse 2D Point Cloud 
* 2019-[2D Car Detection in Radar Data with PointNets](https://ieeexplore.ieee.org/abstract/document/8917000)
* 2020-[Detection and Tracking on Automotive Radar Data with Deep Learning](https://ieeexplore.ieee.org/document/9190261)
* 2020-[Pointillism Accurate 3D Bounding Box Estimation with Multi-Radars](https://dl.acm.org/doi/abs/10.1145/3384419.3430783)
* 2020-[Radar-based 2D Car Detection Using Deep Neural Networks](https://ieeexplore.ieee.org/abstract/document/9294546)
* 2021-[Radar Voxel Fusion for 3D Object Detection](https://www.mdpi.com/2076-3417/11/12/5598)
* 2021-[Kernel Point Convolution LSTM Networks for Radar Point Cloud Segmentation](https://www.mdpi.com/2076-3417/11/6/2599)

### 4D Point Cloud 
* 2019-[Deep Radar Detector](https://ieeexplore.ieee.org/abstract/document/8835792)
* 2019-[mID Tracking and Identifying People with Millimeter Wave Radar](https://ieeexplore.ieee.org/abstract/document/8804831)
* 2020-[Improved and Optimal DBSCAN for Embedded Applications Using High-Resolution Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9253774)
* 2020-[MmWave Radar Point Cloud Segmentation using GMM in Multimodal Traffic Monitoring](https://ieeexplore.ieee.org/abstract/document/9114662)
* 2020-[Through Fog High Resolution Imaging Using MillimeterWave Radar](https://openaccess.thecvf.com/content_CVPR_2020/html/Guan_Through_Fog_High-Resolution_Imaging_Using_Millimeter_Wave_Radar_CVPR_2020_paper.html)
* 2020-[Deep Learning on Radar Centric 3D Object Detection](https://arxiv.org/abs/2003.00851)
* 2021-[Radar Transformer An Object Classification Network Based on 4D MMW Imaging Radar](https://www.mdpi.com/1424-8220/21/11/3854)
* 2021-[mmPose-NLP A Natural Language Processing Approach to Precise Skeletal Pose Estimation using mmWave Radars](https://arxiv.org/abs/2107.10327)
* 2021-[RPFA-Net: a 4D RaDAR Pillar Feature Attention Network for 3D Object Detection](https://ieeexplore.ieee.org/abstract/document/9564754/)

### SAR & ISAR Imaging
* 2020-[High Resolution Radar Dataset for Semi-Supervised Learning of Dynamic Objects](https://ieeexplore.ieee.org/document/9150648)
* 2021-[MIMO-SAR A Hierarchical High-Resolution Imaging Algorithm for mmWave FMCW Radar in Autonomous Driving](https://ieeexplore.ieee.org/abstract/document/9465646)
* 2021-[Classification Of Automotive Targets Using Inverse Synthetic Aperture Radar Images](https://arxiv.org/abs/2101.12535)

### Pre-CFAR Data
#### Range Azimuth Map
* 2019-[Deep Learning-based Object Classification on Automotive Radar Spectra](https://ieeexplore.ieee.org/abstract/document/8835775)
* 2020-[Image Segmentation and Region Classification in Automotive High-Resolution Radar Imagery](https://ieeexplore.ieee.org/abstract/document/9288850)
* 2020-[YOLO-Based Simultaneous Target Detection and Classification in Automotive FMCW Radar Systems](https://www.mdpi.com/1424-8220/20/10/2897)
* 2020-[300 GHz radar object recognition based on deep neural networks and transfer learning](https://arxiv.org/abs/1912.03157)
* 2020-[2020-Probabilistic Oriented Object Detection in Automotive Radar](https://openaccess.thecvf.com/content_CVPRW_2020/html/w6/Dong_Probabilistic_Oriented_Object_Detection_in_Automotive_Radar_CVPRW_2020_paper.html)
* 2021-[Perception Through 2D-MIMO FMCW Automotive Radar Under Adverse Weather](https://arxiv.org/abs/2104.01639)
* 2021-[Deep-Learning Based Decentralized Frame-to-Frame Trajectory Prediction Over Binary Range-Angle Maps for Automotive Radars]()

#### Range Doppler Map
* 2018-[Single-Frame Vulnerable Road Users Classification with a 77 GHz FMCW Radar Sensor and a Convolutional Neural Network](https://ieeexplore.ieee.org/abstract/document/8448126)
* 2018-[Moving Target Classification in Automotive Radar Systems Using Convolutional Recurrent Neural Networks](https://ieeexplore.ieee.org/abstract/document/8553185)
* 2019-[A Study on Radar Target Detection Based on Deep Neural Networks](https://ieeexplore.ieee.org/abstract/document/8629967)
* 2020-[Object Detection and 3d Estimation Via an FMCW Radar Using a Fully Convolutional Network](https://ieeexplore.ieee.org/abstract/document/9054511)
* 2021-[Detecting High-Speed Maneuvering Targets by Exploiting Range-Doppler Relationship for LFM Radar](https://ieeexplore.ieee.org/abstract/document/9347707)
* 2021-[DeepHybrid: Deep Learning on Automotive Radar Spectra and Reflections for Object Classification]()

#### ROD2021 Challenge Paper
* 2021-[Radar Object Detection Using Data Merging, Enhancement and Fusion](https://dl.acm.org/doi/10.1145/3460426.3463653)
* 2021-[Squeeze-and-Excitation network-Based Radar Object Detection with Weighted Location Fusion](https://dl.acm.org/doi/abs/10.1145/3460426.3463654)
* 2021-[Scene-aware Learning Network for Radar Object Detection](https://dl.acm.org/doi/10.1145/3460426.3463655)
* 2021-[DANet: Dimension Apart Network for Radar Object Detection](https://dl.acm.org/doi/10.1145/3460426.3463656)
* 2021-[Efficient-ROD: Efficient Radar Object Detection based on Densely Connected Residual Network](https://dl.acm.org/doi/abs/10.1145/3460426.3463657)
* 2021-[ROD2021 Challenge: A Summary for Radar Object Detection Challenge for Autonomous Driving Applications](https://dl.acm.org/doi/10.1145/3460426.3463658)

#### Range Azimuth Doppler
* 2019-[Experiments with mmWave Automotive Radar Test-bed](https://ieeexplore.ieee.org/abstract/document/9048939)
* 2019-[Vehicle Detection With Automotive Radar Using Deep Learning on Range-Azimuth-Doppler Tensors](https://openaccess.thecvf.com/content_ICCVW_2019/html/CVRSUAD/Major_Vehicle_Detection_With_Automotive_Radar_Using_Deep_Learning_on_Range-Azimuth-Doppler_ICCVW_2019_paper.html)
* 2020-[CNN Based Road User Detection Using the 3D Radar Cube](https://ieeexplore.ieee.org/abstract/document/8962258)
* 2020-[RAMP-CNN A Novel Neural Network for Enhanced Automotive Radar Object Recognition](https://ieeexplore.ieee.org/abstract/document/9249018)
* 2021-[Multi-View Radar Semantic Segmentation](https://arxiv.org/abs/2103.16214)
* 2021-[High-resolution radar road segmentation using weakly supervised learning](https://www.nature.com/articles/s42256-020-00288-6)
* 2021-[Graph Convolutional Networks for 3D Object Detection on Radar Data](https://openaccess.thecvf.com/content/ICCV2021W/AVVision/html/Meyer_Graph_Convolutional_Networks_for_3D_Object_Detection_on_Radar_Data_ICCVW_2021_paper.html)

#### Raw Signal
* 2018-[Classification of Intra-Pulse Modulation of Radar Signals by Feature Fusion Based Convolutional Neural Networks](https://ieeexplore.ieee.org/abstract/document/8553176)


### Micro-Doppler Spectrogram
* 2018-[Practical classification of different moving targets using automotive radar and deep neural networks](https://eprints.gla.ac.uk/160241/)
* 2018-[DNN Transfer Learning From Diversified Micro-Doppler for Motion Classification](https://ieeexplore.ieee.org/abstract/document/8572732)
* 2020-[Uncertainty Analysis of Deep Neural Network for Classification of Vulnerable Road Users using micro-Doppler](https://ieeexplore.ieee.org/abstract/document/9037574)
* 2021-[A Bayesian Framework for Integrated Deep Metric Learning and Tracking of Vulnerable Road Users using Automotive Radars](https://ieeexplore.ieee.org/abstract/document/9423952)

## Radar Camera Fusion
### Feature-level Fusion
* 2019-[Distant Vehicle Detection Using Radar and Vision](https://ieeexplore.ieee.org/document/8794312)
* 2019-[RVNet: Deep Sensor Fusion of Monocular Camera and Radar for Image-based Obstacle Detection in Challenging Environments](https://link.springer.com/chapter/10.1007/978-3-030-34879-3_27)
* 2019-[Radar and Camera Early Fusion for Vehicle Detection in Advanced Driver Assistance Systems](https://ml4ad.github.io/files/papers/Radar%20and%20Camera%20Early%20Fusion%20for%20Vehicle%20Detection%20in%20Advanced%20Driver%20Assistance%20Systems.pdf)
* 2019-[A Deep Learning-based Radar and Camera Sensor Fusion Architecture for Object Detection](https://ieeexplore.ieee.org/document/8916629)
* 2019-[Deep Learning Based 3D Object Detection for Automotive Radar and Camera](https://ieeexplore.ieee.org/document/8904867)
* 2020-[YOdar Uncertainty-based Sensor Fusion for Vehicle Detection with Camera and Radar Sensors](https://arxiv.org/abs/2010.03320v2)
* 2020-[Radar+ RGB Fusion For Robust Object Detection In Autonomous Vehicle](https://ieeexplore.ieee.org/abstract/document/9191046)
* 2020-[Low-level Sensor Fusion for 3D Vehicle Detection using Radar Range-Azimuth Heatmap and Monocular Image](https://openaccess.thecvf.com/content/ACCV2020/html/Kim_Low-level_Sensor_Fusion_Network_for_3D_Vehicle_Detection_using_Radar_ACCV_2020_paper.html)
* 2021-[Radar Camera Fusion via Representation Learning in Autonomous Driving](https://arxiv.org/abs/2103.07825)
* 2021-[Robust Small Object Detection on the Water Surface through Fusion of Camera and MillimeterWave Radar](https://openaccess.thecvf.com/content/ICCV2021/html/Cheng_Robust_Small_Object_Detection_on_the_Water_Surface_Through_Fusion_ICCV_2021_paper.html)
* 2021-[RVDet:Feature-level Fusion of Radar and Camera for Object Detection](https://ieeexplore.ieee.org/document/9564627)

### Region Proposal Based
* 2019-[RRPN: Radar Region Proposal Network for Object Detection in Autonomous Vehicles](https://ieeexplore.ieee.org/document/8803392)
* 2020-[CenterFusion: Center-based Radar and Camera Fusion for 3D Object Detection](https://arxiv.org/abs/2011.04841)
* 2020-[Radar-Camera Sensor Fusion for Joint Object Detection and Distance Estimation in Autonomous Vehicles](https://arxiv.org/abs/2009.08428)
* 2020-[GRIF Net: Gated Region of Interest Fusion Network for Robust 3D Object Detection from Radar Point Cloud and Monocular Image](https://ieeexplore.ieee.org/document/9341177)
* 2021-[milliEye: A Lightweight mmWave Radar and Camera Fusion System for Robust Object Detection](http://aiot.ie.cuhk.edu.hk/papers/milliEye.pdf)
* 2021-[CFTrack: Center-based Radar and Camera Fusion for 3D Multi-Object Tracking](https://arxiv.org/abs/2107.05150)
* 2021-[3D Detection and Tracking for On-road Vehicles with a Monovision Camera and Dual Low-cost 4D mmWave Radars](https://ieeexplore.ieee.org/document/9564904)

### Weakly Supervised
* 2020-[Radar as a Teacher: Weakly Supervised Vehicle Detection using Radar Labels](https://ieeexplore.ieee.org/document/9196855)
* 2021-[RODNet: A Real-Time Radar Object Detection Network Cross-Supervised by Camera-Radar Fused Object 3D Localization](https://ieeexplore.ieee.org/document/9353210)
* 2020-[RSS-Net: Weakly-Supervised Multi-Class Semantic Segmentation with FMCW Radar](https://ieeexplore.ieee.org/document/9304674)
* 2020-[Warping of Radar Data into Camera Image for Cross-Modal Supervision in Automotive Applications](https://arxiv.org/abs/2012.12809)
* 2020-[Weakly Supervised Deep Learning Method for Vulnerable Road User Detection in FMCW Radar](https://ieeexplore.ieee.org/document/9294399)

### Decision-level Fusion
* 2011-[Integrating Millimeter Wave Radar with a Monocular Vision Sensor for On-Road Obstacle Detection Applications](https://www.mdpi.com/1424-8220/11/9/8992)
* 2017-[Comparative Analysis of RADAR- IR Sensor Fusion Methods for Object Detection](https://ieeexplore.ieee.org/abstract/document/8204237?casa_token=Iclafffn7ZEAAAAA:0zfHdvHe2VXd3mQOW_AMjexp-fL4zfzyTZ7CKesXw7jnKEuWe0Ty-akJBW4HYg8pkfJtzfPhz5k)
* 2019-[People Tracking by Cooperative Fusion of RADAR and Camera Sensors](https://ieeexplore.ieee.org/document/8917238)
* 2019-[A DNN-LSTM based Target Tracking Approach using mmWave Radar and Camera Sensor Fusion](https://ieeexplore.ieee.org/abstract/document/9058168)
* [Autonomous Obstacle Avoidance for UAV based on Fusion of Radar and Monocular Camera](https://ieeexplore.ieee.org/abstract/document/9341432?casa_token=hZJ5haSOVqEAAAAA:UoczK2JQxnrkU_rdXKERsm6oVDtLwtembw1iB-dBrrKuZqfbDjgSA4phgCNRI0H-cxGuj_d8NqY)
* 2019-[Extending Reliability of mmWave Radar Trackingand Detection via Fusion With Camera](https://ieeexplore.ieee.org/abstract/document/8844649)
* 2019-[People Tracking by Cooperative Fusion ofRADAR and Camera Sensors](https://ieeexplore.ieee.org/abstract/document/8917238)
* 2019-[TargetDetection Algorithm Based on MMW Radar and Camera Fusion](https://ieeexplore.ieee.org/abstract/document/8917504)
* 2019-[A DNN-LSTM based Target Tracking Approachusing mmWave Radar and Camera Sensor Fusion](https://ieeexplore.ieee.org/abstract/document/9058168?casa_token=-51KkM4RDJUAAAAA:DiM3jG_heIcHkxgsAmrE5ewfVRSrqbp24ChSzRAKYY-nXboD9KZKOp0G1Jl4B0PKi53UnhBfZCI)
* 2020-[A Roadside Camera-Radar Sensing Fusion System for Intelligent Transportation](https://ieeexplore.ieee.org/abstract/document/9337488?casa_token=4Wws9Vyc4UcAAAAA:ktkw199jc7Wtlk2CjHDxOPMQnPCTWINWTZUqEuuTFuL3TsC-P3_U7wqSEQfOPNj72oNt98KFATY)
* 2020-[Cooperative Multi-Sensor Tracking of VulnerableRoad Users in the Presence of Missing Detections](https://www.mdpi.com/1424-8220/20/17/4817)
* 2020-[Robust Target Detection and Tracking Algorithm Based on Roadside Radar and Camera ](https://www.mdpi.com/1424-8220/21/4/1116)
* 2021-[Full-Velocity Radar Returns by Radar-Camera Fusion](https://arxiv.org/abs/2108.10637)

## Radar Lidar Fusion
* 2017-[Vehicle Tracking Using Extended Object Methods: An Approach for Fusing Radar and Laser](https://ieeexplore.ieee.org/document/7989029)
* 2019-[Automated Ground Truth Estimation of Vulnerable Road Users in Automotive Radar Data Using GNSS](https://ieeexplore.ieee.org/abstract/document/8726801)
* 2019-[Learning to see through haze: Radar-based Human Detection for Adverse Weather Conditions](https://ieeexplore.ieee.org/document/8870954)
* 2020-[LiRaNet: End-to-End Trajectory Prediction using Spatio-Temporal Radar Fusion](https://arxiv.org/abs/2010.00731)
* 2020-[RadarNet: Exploiting Radar for Robust Perception of Dynamic Objects](https://arxiv.org/abs/2007.14366)
* 2021-[Robust Multimodal Vehicle Detection in Foggy Weather Using Complementary Lidar and Radar Signals ](https://openaccess.thecvf.com/content/CVPR2021/html/Qian_Robust_Multimodal_Vehicle_Detection_in_Foggy_Weather_Using_Complementary_Lidar_CVPR_2021_paper.html)

## Radar Lidar Camera Fusion
* 2016-[Multiple Sensor Fusion and Classification for Moving Object Detection and Tracking](https://ieeexplore.ieee.org/document/7283636)
* 2020-[High Dimensional Frustum PointNet for 3D Object Detection from Camera, LiDAR, and Radar](https://ieeexplore.ieee.org/abstract/document/9304655)
* 2020-[Seeing Through FogWithout Seeing Fog: Deep Multimodal Sensor Fusion in Unseen Adverse Weather](https://ieeexplore.ieee.org/abstract/document/9304655)
* 2021-[Radar Voxel Fusion for 3D Object Detection](https://www.mdpi.com/2076-3417/11/12/5598)

## Depth Estimation
* 2020-[Camera-Radar Fusion for 3-D Depth Reconstruction](https://ieeexplore.ieee.org/abstract/document/9304559)
* 2021-[Depth Estimation from Monocular Images and Sparse Radar Data](https://ieeexplore.ieee.org/abstract/document/9340998)
* 2021-[Radar-Camera Pixel Depth Association for Depth Completion](https://openaccess.thecvf.com/content/CVPR2021/html/Long_Radar-Camera_Pixel_Depth_Association_for_Depth_Completion_CVPR_2021_paper.html)
* 2021-[R4Dyn: Exploring Radar for Self-Supervised Monocular Depth Estimation of Dynamic Scenes](https://arxiv.org/abs/2108.04814)


## Radar Tracking
* 2010-[Road Intensity Based Mapping Using Radar Measurements With a Probability Hypothesis Density Filter](https://ieeexplore.ieee.org/document/5677613)
* 2015-[Tracking of Extended Objects with High-Resolution Doppler Radar](https://ieeexplore.ieee.org/document/7355362)
* 2018-[Rfcm for Data Association and Multitarget Tracking Using 3D Radar](https://ieeexplore.ieee.org/document/8461917)
* 2018-[Classification Assisted Tracking for Autonomous Driving Domain](https://ieeexplore.ieee.org/document/8547138)
* 2019-[Extended Object Tracking assisted Adaptive Clustering for Radar in Autonomous Driving Applications](https://ieeexplore.ieee.org/abstract/document/8916658)
* 2020-[BAAS: Bayesian Tracking and Fusion Assisted Object Annotation of Radar Sensor Data for Artificial Intelligence Application](https://ieeexplore.ieee.org/document/9266698)
* 2020-[An RLS-Based Instantaneous Velocity Estimator for Extended Radar Tracking](https://ieeexplore.ieee.org/document/9341127)
* 2020-[Extended Object Tracking Using Hierarchical Truncation Measurement Model with Automotive Radar](https://ieeexplore.ieee.org/document/9054614)
* 2020-[Extended Object Tracking Using Spatially Resolved Micro-Doppler Signatures](https://ieeexplore.ieee.org/document/9247291)
* 2021-[A Graph-Based Track-Before-Detect Algorithm for Automotive Radar Target Detection](https://ieeexplore.ieee.org/document/9276431)
* 2021-[Learning-Based Extended Object Tracking Using Hierarchical Truncation Measurement Model With Automotive Radar](https://ieeexplore.ieee.org/document/9351598)
* 2021-[Road-Map Aided GM-PHD Filter for Multi-Vehicle Tracking with Automotive Radar](https://ieeexplore.ieee.org/document/9403944)
* 2021-[Extended Object Tracking assisted Adaptive Multi-Hypothesis Clustering for Radar in Autonomous Driving Domain](https://ieeexplore.ieee.org/abstract/document/9466233)
