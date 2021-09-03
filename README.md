# Awesome Radar Perception
A curated list of radar datasets, detection, tracking and fusion. <br>Keep updating.<br>Author: Yi Zhou<br>Contact: zhouyi1023@tju.edu.cn
<br>Update some public-available codes, see [useful_codes.md](./useful_codes.md)

## Imaging Radar Products

* [TI AWR2243](https://www.ti.com/tool/MMWCAS-RF-EVM?keyMatch=AWR2243%20CASCADE&tisearch=search-everything)
* [Arbe Phoenix](https://arberobotics.com/product/)
* [Continental ARS 540](https://www.continental-automotive.com/en-gl/Passenger-Cars/Autonomous-Mobility/Enablers/Radars/Long-Range-Radar/ARS540)
* [Oculli Falcon](https://www.oculii.com/falcon)
* [Oculli Eagle](https://www.oculii.com/eagle)
* [Vayyar](https://vayyar.com/auto/)
* [Astyx (Acquired by Cruise)](https://www.astyx.com/technology.html)
* Huawei 4D radar [news](https://sparrowsnews.com/2021/04/20/huawei-4d-imaging-radar/)
* ZF PREMIUM [news](https://www.just-auto.com/news/zf-secures-saic-production-contract-for-full-range-radar_id201221.aspx)
* Waymo [news](https://blog.waymo.com/2020/03/introducing-5th-generation-waymo-driver.html)
* A list of automotive radar companies [link](https://mp.weixin.qq.com/s/JP6dOljpCiyGny4y-nmGqw)

## Radar Datasets

### Detection / Tracking
| Dataset      | Affiliation | Links     |    
| ---------- | :-----------: | :-----------: |
| nuScenes | Aptiv | [Website](https://scale.com/open-datasets/nuscenes); [Paper](https://openaccess.thecvf.com/content_CVPR_2020/html/Caesar_nuScenes_A_Multimodal_Dataset_for_Autonomous_Driving_CVPR_2020_paper.html) |
|DENSE| Ulm University |[Website](https://www.uni-ulm.de/en/in/driveu/projects/dense-datasets); [Paper](https://openaccess.thecvf.com/content_CVPR_2020/html/Bijelic_Seeing_Through_Fog_Without_Seeing_Fog_Deep_Multimodal_Sensor_Fusion_CVPR_2020_paper.html)|
| CRUW | University of Washington |[Website](https://www.cruwdataset.org/home); [Paper](https://arxiv.org/abs/2105.05207); [Github](https://github.com/yizhou-wang/RODNet)|
| CARRADA | Valeo | [Website](https://arthurouaknine.github.io/codeanddata/carrada); [Paper](https://arxiv.org/abs/2005.01456); [Github](https://github.com/valeoai/carrada_dataset)|
| RaDICaL | UIUC | [Website](https://publish.illinois.edu/radicaldata/); [Papers](https://ieeexplore.ieee.org/document/9361086); [Github](https://moodoki.github.io/radical_sdk/) |
| RADDet | University of Ottawa | [Paper](https://arxiv.org/abs/2105.00363); [Github](https://github.com/ZhangAoCanada/RADDet) |
| Hires2019 (4D) | Astyx | [Dateset](https://github.com/under-the-radar/radar_dataset_astyx); [Paper](https://ieeexplore.ieee.org/document/8904734) |
| Radar Scenes | Mercedes-Benz AG | [Website](https://radar-scenes.com/); [Paper](https://arxiv.org/abs/2104.02493) ; [Github](https://github.com/oleschum/radar_scenes/) |
| HawkEye | UIUC | [Website](https://jaydeng1019.github.io/HawkEye/); [Github](https://github.com/JaydenG1019/HawkEye-Data-Code); [Paper](https://openaccess.thecvf.com/content_CVPR_2020/html/Guan_Through_Fog_High-Resolution_Imaging_Using_Millimeter_Wave_Radar_CVPR_2020_paper.html) |
| PREVENTION | Universidad de Alcalá | [Website](https://prevention-dataset.uah.es/); [Paper](https://ieeexplore.ieee.org/abstract/document/8917433) |

### Odometry / SLAM / Place Recognition
| Dataset      | Affiliation | Links     |    
| ---------- | :-----------: | :-----------: |
| Oxford Radar Robocar | University of Oxford | [Website](https://oxford-robotics-institute.github.io/radar-robotcar-dataset/); [Paper](https://ieeexplore.ieee.org/abstract/document/9196884); [Github](https://github.com/oxford-robotics-institute/radar-robotcar-dataset-sdk) |
|RADIATE| Heriot Watt University|[Website](http://pro.hw.ac.uk/radiate/doc/dataset/); [Paper](https://arxiv.org/abs/2010.09076); [Github](https://github.com/marcelsheeny/radiate_sdk/tree/master/vehicle_detection)|
| MulRan | KAIST |[Website](https://sites.google.com/view/mulran-pr/dataset); [Paper](https://ieeexplore.ieee.org/abstract/document/9197298); [Github](https://github.com/irapkaist/file_player_mulran)|
| ColoRadar | University of Colorado Boulder |  [Website](https://arpg.github.io/coloradar/); [Paper](https://arxiv.org/abs/2103.04510) |
| USVInland | Orca-Tech | [Website](http://www.orca-tech.cn/datasets/USVInland/Introduction); [Paper](https://ieeexplore.ieee.org/abstract/document/9381638) |
|Zendar SAR |Zendar|[Website](https://www.zendar.io/dataset.html); [Paper](https://ieeexplore.ieee.org/document/9150648); [Github](https://github.com/ZendarInc/ZendarSDK) |
| SCORP | University of Ottawa | [Website](https://sensorcortek.ai/paper-and-datasets/); [Paper](https://arxiv.org/abs/2004.03449) |

### Micro-doppler Signature / Motion
| Dataset      | Affiliation | Links     |    
| ---------- | :-----------: | :-----------: |
| DopNet | UCL | [Website](http://dop-net.com/); [Paper](https://digital-library.theiet.org/content/journals/10.1049/el.2019.4153) |
| Open Radar Datasets | Norwegian Defence Research Establishment etc. | [Paper](https://ieeexplore.ieee.org/abstract/document/9455239); [Github](https://github.com/openradarinitiative/open_radar_datasets) |
| Radar signatures of human activities  | University of Glasgow | [Paper](https://ietresearch.onlinelibrary.wiley.com/doi/10.1049/el.2019.2378); [Dataset](http://researchdata.gla.ac.uk/848/) |
| Solinteraction Data | University of St Andrews | [Paper](https://dl.acm.org/doi/abs/10.1145/3287078); [Github](https://github.com/tcboy88/solinteractiondata) |

## Workshop

* [2021 ICRA Radar Perception for All-Weather Autonomy](https://sites.google.com/view/radar-robotics/home)
* [2021 ICASSP Recent Advances in mmWave Radar Sensing for Autonomous Vehicles](https://www.2021.ieeeicassp.org/Papers/ViewSession_MS.asp?Sessionid=1280)

## Fundamental Books
| Book Title      | Author     |    
| ---------- | :-----------: |
| Fundamentals of Radar Signal Processing | Mark A. Richard |
| Radar Systems Analysis and Design using Matlab | Bassem R. Mahafza| 
| The Micro-Doppler Effect in Radar | Victor C. Chen |
| Robotic Navigation and Mapping with Radar | Martin Adams etc. |

## TI Tutorials
* [Introduction to mmwaveSensing: FMCW Radars](https://training.ti.com/sites/default/files/docs/mmwaveSensing-FMCW-offlineviewing_0.pdf)
* [The fundamentals of millimeter wave sensors](https://www.ti.com/lit/wp/spyy005a/spyy005a.pdf?ts=1619205965675)
* [Using a complex-baseband architecture in FMCW radar systems](https://www.ti.com/lit/wp/spyy007/spyy007.pdf)
* [MIMO radar](https://www.ti.com/lit/an/swra554a/swra554a.pdf)

## Review Papers
* IEEE Signal Processing Magazine Special Issues<br>
Autonomous Driving [Part I Sensing and Perception](https://ieeexplore.ieee.org/xpl/tocresult.jsp?isnumber=9127839&punumber=79)<br>
Radar Systems for Modern Civilian Applications [Part I](https://ieeexplore.ieee.org/xpl/tocresult.jsp?isnumber=8746851&punumber=79) [Part II](https://ieeexplore.ieee.org/xpl/tocresult.jsp?isnumber=8827988&punumber=79)
* [Antenna Concepts for Millimeter-Wave Automotive Radar Sensors](https://ieeexplore.ieee.org/document/6165323)
* [Micro-Doppler Effect in Radar: Phenomenon, Model, and Simulation Study](https://ieeexplore.ieee.org/document/1603402)
* [Application of Deep Learning on Millimeter-Wave Radar Signals: A Review](https://www.mdpi.com/1424-8220/21/6/1951)
* [A Comprehensive Survey of Machine Learning Applied to Radar Signal Processing](https://arxiv.org/abs/2009.13702)
* [Automotive Radar Signal Processing: Research Directions and Practical Challenges](https://ieeexplore.ieee.org/document/9369027)
* [Millimeter-Wave Technology for Automotive Radar Sensors in the 77 GHz Frequency Band](https://ieeexplore.ieee.org/document/6127923)
* [Recent Evolution of Automotive ImagingRadar and Its Information content](https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/iet-rsn.2018.0026)
* [MMW Radar-Based Technologies in Autonomous Driving: A Review](https://www.mdpi.com/1424-8220/20/24/7283)
* [State-of-the-Art Review on Automotive Radars and Passive Radar Reflectors](https://www.theseus.fi/bitstream/handle/10024/144521/LapinAMK%20State-of-the-Art%20Review%20on%20Automotive%20Radars%20and%20Passive%20Radar%20Reflectors.%20paivitetty%2018.5.2018.pdf?sequence=5)
* [Automotive Radars A review of signal processing techniques](https://ieeexplore.ieee.org/abstract/document/7870764)
* [A Review of Recent Advancements Including Machine Learning on Synthetic Aperture Radar using Millimeter-Wave Radar](https://ieeexplore.ieee.org/abstract/document/9266501)
* [Application of Deep Learning on Millimeter-Wave Radar Signal A Review](https://www.mdpi.com/1424-8220/21/6/1951)
* [A Comprehensive Survey of Machine Learning Applied to Radar Signal Processing](https://arxiv.org/abs/2009.13702)


## SAR&ISAR
* 2021-[Classification Of Automotive Targets Using Inverse Synthetic Aperture Radar Images](https://arxiv.org/abs/2101.12535)
* 2021-[MIMO-SAR A Hierarchical High-Resolution Imaging Algorithm for mmWave FMCW Radar in Autonomous Driving](https://ieeexplore.ieee.org/abstract/document/9465646)

## Signature
* 2017-[Radar Reflection Characteristics of Vehicles for Contour and Feature Estimation](https://ieeexplore.ieee.org/abstract/document/8126352)
* 2018-[Radar and Lidar Target Signatures of Various Object Types and Evaluation of Extended Object Tracking Methods for Autonomous Driving Applications](https://ieeexplore.ieee.org/abstract/document/8455395)

## Simulation
* [There and Back Again: Learning to Simulate Radar Data for Real-World Applications](https://arxiv.org/abs/2011.14389)
* [Diversified Radar Micro-Doppler Simulations as Training Data for Deep Residual Neural Networks](https://ieeexplore.ieee.org/document/8378629)
* [Measurements revealing Challenges in Radar Sensor Modeling for Virtual Validation of Autonomous Driving](https://link.springer.com/chapter/10.1007/978-3-030-58523-5_29)
* [Virtual Radar: Real-Time Millimeter-Wave Radar Sensor Simulation for Perception-Driven Robotics](https://ieeexplore.ieee.org/abstract/document/9387149)
* [Vid2Doppler: Synthesizing Doppler Radar Data from Videos for Training Privacy-Preserving Activity Recognition](https://dl.acm.org/doi/abs/10.1145/3411764.3445138)
* [Scalable and Physical Radar Sensor Simulation for Interacting Digital Twins](https://ieeexplore.ieee.org/abstract/document/9205224)

## Calibration
#### Radar & Multi Radars
* [Auto-Calibration of Automotive Radars in Operational Mode Using Simultaneous Localisation and Mapping](https://ieeexplore.ieee.org/document/9353252)
* [Multi-Radar Self-Calibration Method using High-Definition Digital Maps for Autonomous Driving](https://ieeexplore.ieee.org/document/8569272/)
#### Radar-Camera
* [Obstacle Detection Using Millimeter-wave Radar and Its Visualization on Image Sequence](https://ieeexplore.ieee.org/document/1334537/)
* [Radar and vision sensors calibration for outdoor 3D reconstruction]()
* [Spatio-Temporal Multisensor Calibration Based on Gaussian Processes Moving Object Tracking](https://arxiv.org/abs/1904.04187)
* [Targetless Rotational Auto-Calibration of Radar and Camera for Intelligent Transportation Systems](https://ieeexplore.ieee.org/document/8917135)
* [A Continuous-Time Approach for 3D Radar-to-Camera Extrinsic Calibration](https://arxiv.org/abs/2103.07505)
#### Radar-Lidar
* [Extrinsic 6DoF calibration of 3D LiDAR and radar](https://ieeexplore.ieee.org/document/8098688)
* [Extrinsic and Temporal Calibration of Automotive Radar and 3D LiDAR](https://ieeexplore.ieee.org/document/9341715)
* [Automatic Targetless Extrinsic Calibration of Multiple 3D LiDARs and Radars](https://ieeexplore.ieee.org/document/9340866/)
#### Radar-Lidar-Camera
* [Extrinsic 6DoF Calibration of a Radar – LiDAR– Camera System Enhanced by Radar Cross Section Estimates Evaluation](https://www.sciencedirect.com/science/article/pii/S0921889018301994)
* [An Joint Extrinsic Calibration Tool for Radar, Camera and Lidar](https://ieeexplore.ieee.org/document/9380784)
* [Online multi-sensor calibration based on moving object tracking](https://www.tandfonline.com/doi/full/10.1080/01691864.2020.1819874)

## Detection Stastic
* 1996-[An evidentiaI approach to probabilistic map-building](https://ieeexplore.ieee.org/abstract/document/503863)
* 2016-[Potential of Radar for Static Object Classification using Deep Learning Methods](https://ieeexplore.ieee.org/abstract/document/7533931)
* 2017-[Object Classification in Radar Using Ensemble Methods](https://ieeexplore.ieee.org/abstract/document/7918863)
* 2018-[Semantic Segmentation on Radar Point Clouds](https://ieeexplore.ieee.org/abstract/document/8455344)
* 2018-[Radar Characteristics Study For The Development Of Surrogate Roadside Objects](https://scholarworks.iupui.edu/handle/1805/17772)
* 2019-[Probably Unknown Deep Inverse Sensor Modelling Radar](https://ieeexplore.ieee.org/abstract/document/8793263)
* 2019-[Occupancy Grids Generation Using Deep Radar Network for Autonomous Driving](https://ieeexplore.ieee.org/abstract/document/8916897)
* 2019-[Scene Understanding With Automotive Radar](https://ieeexplore.ieee.org/abstract/document/8911477)
* 2019-[Road Scene Understanding by Occupancy Grid Learning from Sparse Radar Clusters using Semantic Segmentation](https://openaccess.thecvf.com/content_ICCVW_2019/html/CVRSUAD/Sless_Road_Scene_Understanding_by_Occupancy_Grid_Learning_from_Sparse_Radar_ICCVW_2019_paper.html)
* 2020-[Kidnapped Radar Topological Radar Localisation using Rotationally-Invariant Metric Learning](https://ieeexplore.ieee.org/abstract/document/9196682)
* 2021-[Cross-Modal Contrastive Learning of Representations for Navigation using Lightweight, Low-Cost Millimeter Wave Radar for Adverse Environmental Conditions](https://ieeexplore.ieee.org/abstract/document/9362209)
* 2020-[Deep Learning for Autonomous and Driver Assistant Systems](https://ruor.uottawa.ca/handle/10393/40852)
* 2020-[1795-RadarSLAM Radar Based Large-Scale SLAM in All Weathers](https://ieeexplore.ieee.org/abstract/document/9341287)
* 2020-[Semantic Segmentation on 3D Occupancy Grids for Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9229096)
* 2020-[Deep Open Space Segmentation using Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9299052)
* 2020-[Statistical Image Segmentation and Region Classification Approaches for Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9337399)
* 2021-[Unsupervised Place Recognition with Deep Embedding Learning over Radar Videos](https://arxiv.org/abs/2106.06703)
* 2021-[PolarNet Accelerated Deep Open Space Segmentation Using Automotive Radar in Polar Domain](https://arxiv.org/abs/2103.03387)
* 2021-[Do We Need to Compensate for Motion Distortion and Doppler Effects in Spinning Radar Navigation](https://ieeexplore.ieee.org/abstract/document/9327473)

## Detection Dynamic
#### Classical
* 2012-[Grid-Based DBSCAN for Clustering Extended Objects in Radar Data](https://ieeexplore.ieee.org/abstract/document/6232167)
* 2015-[Making Bertha See Even More](https://ieeexplore.ieee.org/abstract/document/7161279)
* 2016-[Adaptive Clustering for Contour Estimation of Vehicles for High-Resolution Radar](https://ieeexplore.ieee.org/abstract/document/7533930)
* 2017-[Comparison of Random Forest and Long Short-Term Memory Network Performances in Classification Tasks Using Radar](https://ieeexplore.ieee.org/document/8126350)
* 2018-[Supervised Clustering for Radar Applications On the Way to Radar Instance Segmentation](https://ieeexplore.ieee.org/abstract/document/8443534)
* 2018-[Radar-based Feature Design and Multiclass Classification for Road User Recognition](https://ieeexplore.ieee.org/abstract/document/8500607)
* 2019-[Radar-based Road User Classification and Novelty Detection with Recurrent Neural Network Ensembles](https://ieeexplore.ieee.org/abstract/document/8813773)
* 2019-[Robust and Adaptive Radar Elliptical Density-Based Spatial Clustering and labeling for mmWave Radar Point Cloud Data](https://ieeexplore.ieee.org/abstract/document/9048869)
* 2019-[A Multi-Stage Clustering Framework for Automotive Radar Data](https://ieeexplore.ieee.org/abstract/document/8916873)
* 2020-[Off-the-shelf sensor vs. experimental radar - How much resolution is necessary in automotive radar classification](https://ieeexplore.ieee.org/abstract/document/9190338)
* 2021-[Deep Learning for Automotive Object Classification with Radar Reflections](https://ieeexplore.ieee.org/abstract/document/9455334)

#### Point Cloud Sparse
* 2019-[2D Car Detection in Radar Data with PointNets](https://ieeexplore.ieee.org/abstract/document/8917000)
* 2020-[Pointillism Accurate 3D Bounding Box Estimation with Multi-Radars](https://dl.acm.org/doi/abs/10.1145/3384419.3430783)
* 2020-[Radar-based 2D Car Detection Using Deep Neural Networks](https://ieeexplore.ieee.org/abstract/document/9294546)
* 2021-[Radar Voxel Fusion for 3D Object Detection](https://www.mdpi.com/2076-3417/11/12/5598)

#### Point Cloud 4D
* 2019-[Deep Radar Detector](https://ieeexplore.ieee.org/abstract/document/8835792)
* 2019-[mID Tracking and Identifying People with Millimeter Wave Radar](https://ieeexplore.ieee.org/abstract/document/8804831)
* 2020-[Improved and Optimal DBSCAN for Embedded Applications Using High-Resolution Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9253774)
* 2020-[MmWave Radar Point Cloud Segmentation using GMM in Multimodal Traffic Monitoring](https://ieeexplore.ieee.org/abstract/document/9114662)
* 2020-[Through Fog High Resolution Imaging Using MillimeterWave Radar](https://openaccess.thecvf.com/content_CVPR_2020/html/Guan_Through_Fog_High-Resolution_Imaging_Using_Millimeter_Wave_Radar_CVPR_2020_paper.html)
* 2020-[Deep Learning on Radar Centric 3D Object Detection](https://arxiv.org/abs/2003.00851)
* 2021-[Radar Transformer An Object Classification Network Based on 4D MMW Imaging Radar](https://www.mdpi.com/1424-8220/21/11/3854)
* 2021-[mmPose-NLP A Natural Language Processing Approach to Precise Skeletal Pose Estimation using mmWave Radars](https://arxiv.org/abs/2107.10327)

#### Range Azimuth Map
* 2019-[Deep Learning-based Object Classification on Automotive Radar Spectra](https://ieeexplore.ieee.org/abstract/document/8835775)
* 2020-[Image Segmentation and Region Classification in Automotive High-Resolution Radar Imagery](https://ieeexplore.ieee.org/abstract/document/9288850)
* 2020-[YOLO-Based Simultaneous Target Detection and Classification in Automotive FMCW Radar Systems](https://www.mdpi.com/1424-8220/20/10/2897)
* 2020-[300 GHz radar object recognition based on deep neural networks and transfer learning](https://arxiv.org/abs/1912.03157)
* 2020-[2020-Probabilistic Oriented Object Detection in Automotive Radar](https://openaccess.thecvf.com/content_CVPRW_2020/html/w6/Dong_Probabilistic_Oriented_Object_Detection_in_Automotive_Radar_CVPRW_2020_paper.html)
* 2021-[Perception Through 2D-MIMO FMCW Automotive Radar Under Adverse Weather](https://arxiv.org/abs/2104.01639)
* 2021-[Deep-Learning Based Decentralized Frame-to-Frame Trajectory Prediction Over Binary Range-Angle Maps for Automotive Radars]()


#### Range Azimuth Dopper
* 2019-[Experiments with mmWave Automotive Radar Test-bed](https://ieeexplore.ieee.org/abstract/document/9048939)
* 2019-[Vehicle Detection With Automotive Radar Using Deep Learning on Range-Azimuth-Doppler Tensors](https://openaccess.thecvf.com/content_ICCVW_2019/html/CVRSUAD/Major_Vehicle_Detection_With_Automotive_Radar_Using_Deep_Learning_on_Range-Azimuth-Doppler_ICCVW_2019_paper.html)
* 2020-[2020-CNN Based Road User Detection Using the 3D Radar Cube](https://ieeexplore.ieee.org/abstract/document/8962258)
* 2020-[RAMP-CNN A Novel Neural Network for Enhanced Automotive Radar Object Recognition](https://ieeexplore.ieee.org/abstract/document/9249018)
* 2021-[Multi-View Radar Semantic Segmentation](https://arxiv.org/abs/2103.16214)
* 2021-[High-resolution radar road segmentation using weakly supervised learning](https://www.nature.com/articles/s42256-020-00288-6)


#### Range Doppler Map
* 2018-[Single-Frame Vulnerable Road Users Classification with a 77 GHz FMCW Radar Sensor and a Convolutional Neural Network](https://ieeexplore.ieee.org/abstract/document/8448126)
* 2018-[Moving Target Classification in Automotive Radar Systems Using Convolutional Recurrent Neural Networks](https://ieeexplore.ieee.org/abstract/document/8553185)
* 2019-[A Study on Radar Target Detection Based on Deep Neural Networks](https://ieeexplore.ieee.org/abstract/document/8629967)
* 2020-[Object Detection and 3d Estimation Via an FMCW Radar Using a Fully Convolutional Network](https://ieeexplore.ieee.org/abstract/document/9054511)
* 2021-[Detecting High-Speed Maneuvering Targets by Exploiting Range-Doppler Relationship for LFM Radar](https://ieeexplore.ieee.org/abstract/document/9347707)


#### Raw
* 2018-[On the Deployment and Noise Filtering of Vehicular Radar Application for Detection Enhancement](https://www.mdpi.com/1424-8220/18/3/837)
* 2018-[2018-Classification of Intra-Pulse Modulation of Radar Signals by Feature Fusion Based Convolutional Neural Networks](https://ieeexplore.ieee.org/abstract/document/8553176)
* 2019-[Robust CFAR Detection for Multiple Targets in K-Distributed Sea Clutter Based on Machine Learning](https://www.mdpi.com/2073-8994/11/12/1482)



#### Spectrogram
* 2018-[Practical classification of different moving targets using automotive radar and deep neural networks](https://eprints.gla.ac.uk/160241/)
* 2018-[DNN Transfer Learning From Diversified Micro-Doppler for Motion Classification](https://ieeexplore.ieee.org/abstract/document/8572732)
* 2020-[New Radar Micro-Doppler Tag for Road Safety Based on the Signature of Rotating Backscatters](https://ieeexplore.ieee.org/abstract/document/9311635)
* 2020-[Uncertainty Analysis of Deep Neural Network for Classification of Vulnerable Road Users using micro-Doppler](https://ieeexplore.ieee.org/abstract/document/9037574)
* 2021-[A Bayesian Framework for Integrated Deep Metric Learning and Tracking of Vulnerable Road Users using Automotive Radars](https://ieeexplore.ieee.org/abstract/document/9423952)

## Ego Motion
* 2018-[Precise Ego-Motion Estimation with Millimeter-Wave Radar under Diverse and Challenging Conditions](https://ieeexplore.ieee.org/abstract/document/8460687)
* 2019-[An Instantaneous 3D Ego-Velocity Measurement Algorithm for Frequency Modulated Continuous Wave Doppler Radar Data](https://www.proquest.com/openview/0354baf8a7e55480288b5abc6bb52677/1?pq-origsite=gscholar&cbl=18750&diss=y)
* 2020-[Radar-Inertial Ego-Velocity Estimation for Visually Degraded Environments](https://ieeexplore.ieee.org/abstract/document/9196666)

## Muti-Path
* 2017-[A Novel Target-Height Estimation Approach Using Radar-Wave Multipath Propagation for Automotive Applications](https://ars.copernicus.org/articles/15/61/2017/)
* 2018-[Automotive Radar Multipath Propagation in Uncertain Environments](https://ieeexplore.ieee.org/abstract/document/8570016)
* 2018-[Analysis of Multipath and DOA Detection Using a Fully Polarimetric Automotive Radar](https://www.cambridge.org/core/journals/international-journal-of-microwave-and-wireless-technologies/article/analysis-of-multipath-and-doa-detection-using-a-fully-polarimetric-automotive-radar/C3659FC550A9A4CDDE9ED420B97A6587)
* 2020-[Using Machine Learning to Detect Ghost Images in Automotive Radar](https://ieeexplore.ieee.org/abstract/document/9294631)
* 2020-[Seeing Around Street Corners Non-Line-of-Sight Detection and Tracking In-the-Wild Using Doppler Radar](https://openaccess.thecvf.com/content_CVPR_2020/html/Scheiner_Seeing_Around_Street_Corners_Non-Line-of-Sight_Detection_and_Tracking_In-the-Wild_Using_CVPR_2020_paper.html)
* 2021-[Ghost Target Detection in 3D Radar Data using Point Cloud based Deep Neural Network](https://ieeexplore.ieee.org/abstract/document/9413247)


## Polarimetric
* 2016-[A Polarimetric 76-79 GHz Radar-Frontend for Target Classification in Automotive Use](https://ieeexplore.ieee.org/abstract/document/7824638)
* 2018-[Performance Analysis of 79 GHz Polarimetric Radar Sensors for Autonomous Driving](https://ieeexplore.ieee.org/abstract/document/8249142)
* 2018-[Autonomous Driving Features based on 79 GHz Polarimetric Radar Data](https://ieeexplore.ieee.org/abstract/document/8546632)
* 2019-[Polarimetric Signatures of a Passenger Car](https://ieeexplore.ieee.org/abstract/document/8890117)



## Radar Camera Fusion
### Weakly Supervised
* 2020-[Radar as a Teacher: Weakly Supervised Vehicle Detection using Radar Labels](https://ieeexplore.ieee.org/document/9196855)
* 2019-[Automotive radar and camera fusion using Generative Adversarial Networks](https://www.sciencedirect.com/science/article/abs/pii/S1077314219300530)
* 2021-[RODNet: A Real-Time Radar Object Detection Network Cross-Supervised by Camera-Radar Fused Object 3D Localization](https://ieeexplore.ieee.org/document/9353210)
* 2020-[RSS-Net: Weakly-Supervised Multi-Class Semantic Segmentation with FMCW Radar](https://ieeexplore.ieee.org/document/9304674)
* 2020-[Warping of Radar Data into Camera Image for Cross-Modal Supervision in Automotive Applications](https://arxiv.org/abs/2012.12809)
* 2020-[Weakly Supervised Deep Learning Method for Vulnerable Road User Detection in FMCW Radar](https://ieeexplore.ieee.org/document/9294399)

#### Radar Vision Fusion 
* 2019-[Distant Vehicle Detection Using Radar and Vision](https://ieeexplore.ieee.org/document/8794312)
* 2019-[Radar and Camera Early Fusion for Vehicle Detection in Advanced Driver Assistance Systems](https://ml4ad.github.io/files/papers/Radar%20and%20Camera%20Early%20Fusion%20for%20Vehicle%20Detection%20in%20Advanced%20Driver%20Assistance%20Systems.pdf)
* 2019-[A Deep Learning-based Radar and Camera Sensor Fusion Architecture for Object Detection](https://ieeexplore.ieee.org/document/8916629)
* 2020-[Depth Estimation from Monocular Images and Sparse Radar Data](https://arxiv.org/abs/2010.00058)
* 2019-[Deep Learning Based 3D Object Detection for Automotive Radar and Camera](https://ieeexplore.ieee.org/document/8904867)
* 2019-[RRPN: Radar Region Proposal Network for Object Detection in Autonomous Vehicles](https://ieeexplore.ieee.org/document/8803392)
* 2020-[CenterFusion: Center-based Radar and Camera Fusion for 3D Object Detection](https://arxiv.org/abs/2011.04841)
* 2020-[Radar-Camera Sensor Fusion for Joint Object Detection and Distance Estimation in Autonomous Vehicles](https://arxiv.org/abs/2009.08428)
* 2019-[People Tracking by Cooperative Fusion of RADAR and Camera Sensors](https://ieeexplore.ieee.org/document/8917238)
* 2019-[A DNN-LSTM based Target Tracking Approach using mmWave Radar and Camera Sensor Fusion](https://ieeexplore.ieee.org/abstract/document/9058168)
* 2021-[Radar Camera Fusion via Representation Learning in Autonomous Driving](https://arxiv.org/abs/2103.07825)
* 2020-[Radar+ RGB Fusion For Robust Object Detection In Autonomous Vehicle](https://ieeexplore.ieee.org/abstract/document/9191046)
* 2021-[milliEye: A Lightweight mmWave Radar and Camera Fusion System for Robust Object Detection](http://aiot.ie.cuhk.edu.hk/papers/milliEye.pdf)

#### Radar Lidar Vision Fusion
* 2020-[High Dimensional Frustum PointNet for 3D Object Detection from Camera, LiDAR, and Radar](https://ieeexplore.ieee.org/abstract/document/9304655)
* 2020-[Seeing Through FogWithout Seeing Fog: Deep Multimodal Sensor Fusion in Unseen Adverse Weather](https://ieeexplore.ieee.org/abstract/document/9304655)
* 2016-[Multiple Sensor Fusion and Classification for Moving Object Detection and Tracking](https://ieeexplore.ieee.org/document/7283636)
* 2021-[Radar Voxel Fusion for 3D Object Detection](https://www.mdpi.com/2076-3417/11/12/5598)
