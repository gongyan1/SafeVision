# Safe 2.0: Redundant Perception
This repository presents a curated collection of multi-camera and multimodal pure vision systems in autonomous driving, with a focus on sensor fusion strategies that enhance perception reliability and safety.

🔍Overview Single-camera systems suffer from limited field of view and blind spots at high speeds, compromising situational awareness in dynamic driving scenarios. Multi-camera and multimodal setups address these issues by expanding coverage and reducing blind zones. To better understand these approaches, sensor fusion strategies are categorized into two main types:  
📌Homogeneous Sensor: Uses multiple cameras of the same type to improve spatial resolution, perception stability, and redundancy.  
📌Heterogeneous Sensor: Combines different vision sensors to maintain robust perception under challenging environmental conditions.  

## Homogeneous Sensor
### Multiple RGBs
#### 2D-to-3D methods
##### ``Pseudo-LiDAR'' methods.
* Pseudo-LiDAR++: Accurate Depth for 3D Object Detection in Autonomous Driving / [paper](https://arxiv.org/abs/1906.06310) / [project](https://github.com/mileyan/Pseudo_Lidar_V2/) / ICLR 2020 / Pseudo-LiDAR++  
* Pseudo-LiDAR point cloud magnification / [paper](https://www.sciencedirect.com/science/article/pii/S0925231220314569) / Neurocomputing 2021
* Real-time pseudo-lidar 3d object detection with geometric constraints / [paper](https://ieeexplore.ieee.org/document/9922503) / [project](https://github.com/mileyan/Pseudo_Lidar_V2/) / ITSC 2022
##### Depth distribution methods.
* Lift, Splat, Shoot: Encoding Images From Arbitrary Camera Rigs by Implicitly Unprojecting to 3D / [paper](https://arxiv.org/abs/2008.05711) / [project](https://github.com/nv-tlabs/lift-splat-shoot/) / ECCV 2020 / LSS 
* BEVDet: High-performance Multi-camera 3D Object Detection in Bird-Eye-View / [paper](https://arxiv.org/abs/2112.11790) / [project](https://github.com/HuangJunJie2017/BEVDet/) / arXiv 2021 / BEVDet  
* BEVDepth: Acquisition of Reliable Depth for Multi-view 3D Object Detection / [paper](https://arxiv.org/abs/2206.10092) / [project](https://github.com/Megvii-BaseDetection/BEVDepth/) / AAAI 2023 / BEVDepth  
* SA-BEV: Generating Semantic-Aware Bird's-Eye-View Feature for Multi-view 3D Object Detection / [paper](https://arxiv.org/abs/2307.11477) / [project](https://github.com/mengtan00/SA-BEV/) / ICCV 2023 / SA-BEV  
* GaussianLSS - Toward Real-world BEV Perception: Depth Uncertainty Estimation via Gaussian Splatting / [paper](https://arxiv.org/html/2504.01957v1) / [project](https://github.com/HCIS-Lab/GaussianLSS/) / CVPR 2025 / GaussianLSS  


#### 3D-to-2D methods
##### MLP-based methods.
* NEAT: Neural Attention Fields for End-to-End Autonomous Driving / [paper](https://arxiv.org/abs/2109.04456) / [project](https://github.com/autonomousvision/neat/) / ICCV 2021 / NEAT  
* Robust Multi-Camera BEV Perception: An Image-Perceptive Approach to Counter Imprecise Camera Calibration / [paper](https://ieeexplore.ieee.org/document/10802840) / IROS 2024  
##### Transformer-based methods.
* DETR3D: 3D Object Detection from Multi-view Images via 3D-to-2D Queries / [paper](https://arxiv.org/abs/2110.06922) / [project](https://github.com/WangYueFt/detr3d/) / CoRL 2021 / DETR3D  
* PETR: Position Embedding Transformation for Multi-View 3D Object Detection / [paper](https://arxiv.org/abs/2203.05625) / [project](https://github.com/megvii-research/PETR/) / ECCV 2022 / PETR  
* PolarFormer: Multi-camera 3D Object Detection with Polar Transformer / [paper](https://arxiv.org/abs/2206.15398) / [project](https://github.com/fudan-zvg/PolarFormer/) / AAAI 2023 / PolarFormer  
* CoBEVT: Cooperative Bird's Eye View Semantic Segmentation with Sparse Transformers / [paper](https://arxiv.org/abs/2207.02202) / [project](https://github.com/DerrickXuNu/CoBEVT/) / CoRL 2022 / CoBEVT  
* Far3D: Expanding the Horizon for Surround-view 3D Object Detection / [paper](https://arxiv.org/abs/2308.09616) / [project](https://github.com/megvii-research/Far3D/) / AAAI 2024 / Far3D  
* DA-BEV: Unsupervised Domain Adaptation for Bird's Eye View Perception / [paper](https://arxiv.org/abs/2401.08687) / [project](https://github.com/xdjiangkai/DA-BEV/) / ECCV 2024 / DA-BEV  

### Multiple Fisheyes
#### Geometry-based modeling methods

* Surround-view fisheye camera viewpoint augmentation for image semantic segmentation / [paper](https://ieeexplore.ieee.org/abstract/document/10128129) / IEEE Access 2023  
* Easy calibration of a blind-spot-free fisheye camera system using a scene of a parking space / [paper](https://ieeexplore.ieee.org/abstract/document/5645687) / IEEE T-ITS 2011  
* Panoramic SLAM from a multiple fisheye camera rig / [paper](https://www.sciencedirect.com/science/article/abs/pii/S0924271619302758) / [project](http://study.rsgis.whu.edu.cn/pages/download/) / ISPRS Journal of Photogrammetry and Remote Sensing 2020  
* Dual-fisheye omnidirectional stereo / [paper](https://ieeexplore.ieee.org/abstract/document/8206587) / IROS 2017  
* Real-time variational fisheye stereo without rectification and undistortion / [paper](https://arxiv.org/abs/1909.07545) / arXiv 2019  
* 3D visual perception for self-driving cars using a multi-camera system: Calibration, mapping, localization, and obstacle detection / [paper](https://www.sciencedirect.com/science/article/abs/pii/S0262885617301117) / [project](https://github.com/hengli/camodocal) / Image and Vision Computing 2017  
* Automatic parking based on a bird's eye view vision system / [paper](http://dx.doi.org/10.1155/2014/847406) / Advances in Mechanical Engineering 2014  


#### Deep learning-based methods
##### CNN-based methods.
* Soilingnet: Soiling detection on automotive surround-view cameras / [paper](https://ieeexplore.ieee.org/abstract/document/8917178) / ITSC 2019 / SoilingNet  
* FisheyeSuperPoint: Keypoint detection and description network for fisheye images / [paper](https://arxiv.org/abs/2103.00191) / arXiv 2021 / FisheyeSuperPoint  
* Restricted deformable convolution-based road scene semantic segmentation using surround view cameras / [paper](https://ieeexplore.ieee.org/abstract/document/8842620) / IEEE T-ITS 2019 / RDC    
* Deformable convolution based road scene semantic segmentation of fisheye images in autonomous driving / [paper](https://digital-library.theiet.org/doi/abs/10.1049/icp.2024.3270) / IET Conference 2024  
* Fisheyebevseg: Surround view fisheye cameras based bird's-eye view segmentation for autonomous driving / [paper](https://openaccess.thecvf.com/content/CVPR2024W/OmniCV2024/papers/Yogamani_FisheyeBEVSeg_Surround_View_Fisheye_Cameras_based_Birds-Eye_View_Segmentation_for_CVPRW_2024_paper.pdf) / CVPR 2024 / FisheyeBEVSeg  
* Sweepnet: Wide-baseline omnidirectional depth estimation / [paper](https://ieeexplore.ieee.org/abstract/document/8793823) / ICRA 2019 / SweepNet  
* Fisheyedepth: A real scale self-supervised depth estimation model for fisheye camera / [paper](https://ieeexplore.ieee.org/abstract/document/11127840) / [project](https://github.com/guoyangzhao/FisheyeDepth) / ICRA 2025 / FisheyeDepth  

##### Transformer-based methods.
* Lightweight fisheye object detection network with transformer-based feature enhancement for autonomous driving / [paper](https://ieeexplore.ieee.org/abstract/document/10802087) / IROS 2024  
* F2BEV: Bird's Eye View Generation from Surround-View Fisheye Camera Images for Automated Driving / [paper](https://ieeexplore.ieee.org/abstract/document/10341862) / [project](https://github.com/volvo-cars/FB-SSEM-dataset) / IROS 2023 / F2BEV  
* ArticuBEVSeg: Road Semantic Understanding and Its Application in Bird's Eye View from Panoramic Vision System of Long Combination Vehicles / [paper](https://ieeexplore.ieee.org/abstract/document/11014516) / IEEE Robotics and Automation Letters 2025 / ArticuBEVSeg  
* Omnividar: Omnidirectional depth estimation from multi-fisheye images / [paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Xie_OmniVidar_Omnidirectional_Depth_Estimation_From_Multi-Fisheye_Images_CVPR_2023_paper.pdf) / CVPR 2023 / OmniVidar  


## Heterogeneous Sensor
### RGB & Thermal
#### Dual-modality inference
##### RGB as the primary.
* Learning cross-modal deep representations for robust pedestrian detection / [paper](https://openaccess.thecvf.com/content_cvpr_2017/papers/Xu_Learning_Cross-Modal_Deep_CVPR_2017_paper.pdf) / CVPR 2017 / CMT-CNN     
* Deep Learning Based Human Detection Using Thermal-RGB Data Fusion for Safe Automotive Guided-Driving / [paper](https://ieeexplore.ieee.org/abstract/document/10503400) / PerCom Workshops 2024    

##### Thermal as the primary.
* RANUS: RGB and NIR urban scene dataset for deep scene parsing / [paper](https://ieeexplore.ieee.org/abstract/document/8279453) / IEEE Robotics and Automation Letters 2018  
* MS-UDA: Multi-spectral unsupervised domain adaptation for thermal image semantic segmentation / [paper](https://ieeexplore.ieee.org/abstract/document/9468936) / [project](https://github.com/yeong5366/MS-UDA) / IEEE Robotics and Automation Letters 2021 / MS-UDA  

##### Dual branch.
* Complementary random masking for rgb-thermal semantic segmentation / [paper](https://ieeexplore.ieee.org/abstract/document/10611200) / [project](https://github.com/UkcheolShin/CRM_RGBTSeg) / ICRA 2024 / CRM  
* Temporal consistency for RGB-thermal data-based semantic scene understanding / [paper](https://ieeexplore.ieee.org/abstract/document/10675452) / [project](https://github.com/lab-sun/Temporal-Consistent-RGBT-Segmentation) / IEEE Robotics and Automation Letters 2024  
* Multimodal object detection via probabilistic ensembling / [paper](https://arxiv.org/pdf/2104.02904) / [project](https://github.com/Jamie725/RGBT-detection) / ECCV 2022 / ProbEn  
* Deep multimodal detection in reduced visibility using thermal depth estimation for autonomous driving / [paper](https://www.mdpi.com/1424-8220/22/14/5084) / Sensors 2022 / YOLORT+DN-RTD  
* Deep cross spectral stereo matching using multi-spectral image fusion / [paper](https://ieeexplore.ieee.org/abstract/document/9723634) / IEEE Robotics and Automation Letters 2022 / SMN  

#### Single-modality inference
* Enhancing autonomous driving by exploiting thermal object detection through feature fusion / [paper](https://link.springer.com/article/10.1007/s13177-024-00385-5) / International Journal of Intelligent Transportation Systems Research 2024 / MDFFTDet  
* Borrow from anywhere: Pseudo multi-modal object detection in thermal imagery / [paper](https://openaccess.thecvf.com/content_CVPRW_2019/papers/PBVS/Devaguptapu_Borrow_From_Anywhere_Pseudo_Multi-Modal_Object_Detection_in_Thermal_Imagery_CVPRW_2019_paper.pdf) / CVPR Workshops 2019 / MMTOD  



### RGB \& Event
#### Image-based methods
* Rgb-event fusion for moving object detection in autonomous driving / [paper](https://ieeexplore.ieee.org/abstract/document/10161563) / [project](https://github.com/ZZY-Zhou/RENet) / ICRA 2023 / RENet  
* Visevent: Reliable object tracking via collaboration of frame and event flows / [paper](https://ieeexplore.ieee.org/abstract/document/10284004) / [project](https://github.com/wangxiao5791509/VisEvent_SOT_Benchmark) / IEEE Transactions on Cybernetics 2024 / VisEvent  
* Embracing events and frames with hierarchical feature refinement network for object detection / [paper](https://arxiv.org/pdf/2407.12582) / [project](https://github.com/HuCaoFighting/FRN) / ECCV 2024  
• Enhancing traffic object detection in variable illumination with rgb-event fusion / [paper](https://ieeexplore.ieee.org/abstract/document/10682110) / [project](https://github.com/YN-Yang/SFNet) / IEEE Transactions on Intelligent Transportation Systems 2024 / SFNet  

#### Event stream-based methods
* Event-based vision enhanced: A joint detection framework in autonomous driving / [paper](https://ieeexplore.ieee.org/abstract/document/8784777) / ICME 2019 / JDF  
* Low-latency automotive vision with event cameras / [paper](https://www.nature.com/articles/s41586-024-07409-w) / [project](https://github.com/uzh-rpg/dagr) / Nature 2024 / DAGr  
* Revisiting color-event based tracking: A unified network, dataset, and metric / [paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320325013810) / [project](https://github.com/Event-AHU/COESOT) / Pattern Recognition 2025 / CEUTrack  
* Efficient Spiking Neural Network for RGB--Event Fusion-Based Object Detection / [paper](https://www.mdpi.com/2079-9292/14/6/1105) / Electronics 2025 / SFDNet  