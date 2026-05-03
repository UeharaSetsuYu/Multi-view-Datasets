# Multi-view-Datasets (Comming soon)

In representation learning fields such as multi-view clustering, researchers tend to focus more on algorithms within the feature space, predominantly utilizing public datasets. This offers considerable convenience, as obtaining public datasets is generally free from strict copyright restrictions, sparing us the arduous task of dataset construction. However, existing repositories fail to provide a comprehensive and unified public dataset library specifically dedicated to the field of multi-view representation learning. Therefore, I aim to systematically organize and compile the multi-view datasets I have collected throughout my research process.

<div align="center">
 
| Datasets Name | Sampel num | View_num | Classes_num | Link | 
| :--- | :---: | :---: | :---: | :---: |
| BDGP | 2500 | 2 | 5 | [BDGP](#BDGP)|
| BBCSport | 544 | 2 | 5 | [BBCSport](#BBCsport)|
| NGs | 500 | 3 | 5 |[NGs](#NGs) |
| Cora | 2708 | 2 | 7 |[Cora](#Cora) |
| Movies | 617 | 2 | 17 | [Movies](#Movies) |
|Hdigit| 10000 | 2 | 10 | [Hdigit](#Hdigit) |
|CIFAR-10| 50000|3|10|[CIFAR-10](#CIFAR-10 )|
|100Leaves| 1600|3|16|[100Leaves](#100Leaves)|
|CCV | 6773 | 3 | 20 | [CCV](#CCV)|
|CiteSeer| 3312 | 2| 6| [CiterSeer](#CiterSeer)|
|LandUse_21|2100|3|21|[LandUse_21](#LandUse_21)|
|Wiki_fea|2866|2|10|[Wiki_fea](#Wiki_fea)|
|CUB|600|2|10|[CUB](#CUB)|
|synthetic3d|600|3|3|[synthetic3d](#synthetic3d)|
|Caltech101-7|1474|6|7|[Caltech101-7](#Caltech101-7)|
|Reuters_dim10|18758|5|6|[Reuters_dim10](#Reuters_dim10)|
|Scene_15|4485|3|15|[Scene_15](#Scene_15)|
|prokaryotic|551|3|4|[prokaryotic](#prokaryotic)|
|proteinFold|694|12|27|[proteinFold](#proteinFold)|
|WebKB|1051|2|2|[WebKB](#WebKB)|
|ACM|3025|5|3|[ACM](#ACM)|
|OutdoorScene|2688|3|8|[OutdoorScene](#OutdoorScene)|
|ACM|3025|5|3|[ACM](#ACM)|
|OutdoorScene|2688|4|8|[OutdoorScene](#OutdoorScene)|
|yale|165|3|15|[yale](#yale)|
</div>

<img src="./img/megaphone.png" alt="icon" width="20" /> <b> Update Datasets (Apr.29.2026) </b>
<div align = "center">  
 <b>Large-scale datasets are available on the cloud drive. Update ALOI_1K, Animal, AwAfea, Caltech101-20, Caltech101-all, Caltech102, CIFAR10, CIFAR100, Fashion, MNIST_USPS, NUS_WIDE, nuswide_deep_2, NUSWIDEOBJ, ORL, STL10_fea</b> 
</div> 
<br>
 
<a name="my-anchor"></a> <img src="./img/cloud.png" alt="icon" width="20" /> <b> Datasets with large file sizes can be found in the cloud drive: [MVC_datasets](https://drive.google.com/drive/folders/14TEYr4L82iKSKhTxt70End6ucGlhJTlS?usp=drive_link)  </b>




### BDGP
Berkeley Drosophila Genome Project (BDGP): dataset consists of two views: image and text. Common references: Cai, Xiao, et al. "Joint stage recognition and anatomical annotation of drosophila gene expression patterns." Bioinformatics 28.12 (2012): i16-i24. Datasets: [Drive_link](#my-anchor)

### BBCSport
The dataset comprises 544 sports news articles collected from the BBC Sport website, covering five categories: Athletics, Cricket, Football, Rugby, and Tennis. To construct the multi-view data, each document was randomly
partitioned into two segments, and a term frequency matrix was generated for each segment to serve as a distinct view. 

### NGs
The dataset consists of 500 news articles spanning five distinct categories: Sports, Computers,
Science, Politics, and Religion. Three separate views were constructed using term frequency statistics, stemming, and
stop-word filtering, respectively. Each view has a dimensionality of 2,000. 

### Cora
The dataset consists of 2,708 samples sourced from an academic paper database, categorized into seven classes representing different subfields. Two views were constructed: a citation relationship view and a
content attribute view. The content attribute view is represented by a feature matrix with dimensions of [2,708, 1,433].

### Movies
The dataset contains 617 samples belonging to 17 categories, which typically correspond to different movie
genres. It consists of two views: (1) the first view is composed of keywords extracted from movie descriptions, with a
feature dimension of 1878; (2) the second view represents the cast information of movies, with a feature dimension of
1398. Its cited for [Movies dataset link](https://lig-membres.imag.fr/grimal/data.html)

### Hdigit
This handwritten digit dataset consists of 10,000 samples. It is organized into two views: the first view comprises
784-dimensional raw pixel features, while the second view consists of 256-dimensional morphological texture features.


### CIFAR-10 
The dataset consists of 50,000 samples categorized into 10 classes. We constructed three views by extracting
features from different layers of a ResNet-50 backbone. View 1 (512 dimensions) captures low-level information such as
textures and edges; View 2 (1,024 dimensions) encodes mid-level features representing object parts; and View 3 (2,048
dimensions) encapsulates high-level global semantic features.

### 100Leaves
Includes three views: shape features, texture features, and edge features.
 

### CCV
It incorporates Spatio-Temporal Interest Points (STIP), Scale-Invariant Feature Transform (SIFT), and Mel-Frequency Cepstral Coefficients (MFCC). Essentially, these represent multimodal data from video—comprising images, motions, and audio—characterized by significant view discrepancies and true heteromodality.



### CiteSeer
It comprises content features and structural features (represented by the adjacency matrix), both of which are embedded within a graph structure.


### LandUse_21
Refer to the paper [DCP](#DCP) and the corresponding open-source repository [2022-TPAMI-DCP](https://github.com/XLearning-SCU/2022-TPAMI-DCP).


### Wiki_fea
Cross-modal data, comprising both image and text features, presents significant challenges for alignment. 

### CUB
Avian features, comprising cross-modal data of both images and text.

### synthetic3d
Refer to the paper [DFL-NET](#DFL-NET) and the corresponding open-source repository [2025-TKDE-DFLNET](https://github.com/chenzhe207/DFL-NET).

### Caltech101-7
Caltech101-7 is a subset of the Caltech101 dataset, consisting of multi-view representations of image data derived through various feature engineering techniques. These views include HOG, GIST, LBP, Gabor, CENTRIST, and WM features.

### Reuters_dim10
The dataset comprises five languages—English, French, German, Spanish, and Italian—treated as distinct views, with each view reduced to a 10-dimensional representation through feature engineering. Refer to the paper [DDMVC](#DDMVC) and the corresponding open-source repository [2025-PR-DDMVC](https://github.com/xujunpeng832/DDMVC)).
 
### Scene_15
Refer to [LandUse_15](#LandUse_15).

### prokaryotic
The dataset represents prokaryotic information and comprises three views: text data, proteome composition, and genomic representation. These correspond to features extracted via the Bag-of-Words (BoW) model, encoded features, and binary-encoded representations, respectively.
 
### proteinFold
Refer to the paper [MVC-LFA](#MVC-LFA)

### WebKB
It primarily comprises two views: the sparse text of the webpage content and the inbound anchor text.

### ACM
This dataset consists of research paper data from a database, featuring both a text feature view and a graph node view. For further details, please refer to the following paper: [OMC-DVM](OMC-DVM)

### OutdoorScene
This dataset uses images processed by different feature engineering techniques as distinct views, including GIST, HOG, LBP, and Gabor features. For details, please refer to the paper: [Mask-IMvC](#Mask-IMvC). 

### yale
The image features extracted for this dataset include Intensity, LBP, and Gabor features. For details, please refer to the paper: [CSMCS](#CSMCS)


## Reference
### DCP 
@article{lin2022dual,
  title={Dual contrastive prediction for incomplete multi-view representation learning},
  author={Lin, Yijie and Gou, Yuanbiao and Liu, Xiaotian and Bai, Jinfeng and Lv, Jiancheng and Peng, Xi},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
  volume={45},
  number={4},
  pages={4447--4461},
  year={2022},
  publisher={IEEE}
}
### DFL-NET
@article{chen2025dfl,
  title={DFL-Net: Disentangled Feature Learning Network for Multi-View Clustering},
  author={Chen, Zhe and Wu, Xiao-Jun and Xu, Tianyang and Kittler, Josef},
  journal={IEEE Transactions on Knowledge and Data Engineering},
  year={2025},
  publisher={IEEE}
}

### DDMVC
@article{xu2025deep,
  title={Deep multi-view clustering with diverse and discriminative feature learning},
  author={Xu, Junpeng and Meng, Min and Liu, Jigang and Wu, Jigang},
  journal={Pattern Recognition},
  volume={161},
  pages={111322},
  year={2025},
  publisher={Elsevier}
}

### MVC-LFA
@inproceedings{wang2019multi,
  title={Multi-view clustering via late fusion alignment maximization.},
  author={Wang, Siwei and Liu, Xinwang and Zhu, En and Tang, Chang and Liu, Jiyuan and Hu, Jingtao and Xia, Jingyuan and Yin, Jianping},
  booktitle={Ijcai},
  pages={3778--3784},
  year={2019}
}

### OMC-DVM
@inproceedings{zhu2026online,
  title={Online Multi-Relational Clustering with Dominant View Mining},
  author={Zhu, Zhengzhong and Zhou, Pei and Wang, Dongsheng and Cheng, Li and Zhu, Jiangping},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
  volume={40},
  number={34},
  pages={29232--29240},
  year={2026}
}

### Mask-IMvC
@article{li2025mask,
  title={Mask-informed deep contrastive incomplete multi-view clustering},
  author={Li, Zhenglai and Shi, Yuqi and He, Xiao and Tang, Chang},
  journal={IEEE Transactions on Circuits and Systems for Video Technology},
  year={2025},
  publisher={IEEE}
}

### CSMCS
@inproceedings{luo2018consistent,
  title={Consistent and specific multi-view subspace clustering},
  author={Luo, Shirui and Zhang, Changqing and Zhang, Wei and Cao, Xiaochun},
  booktitle={Proceedings of the AAAI conference on artificial intelligence},
  volume={32},
  number={1},
  year={2018}
}

