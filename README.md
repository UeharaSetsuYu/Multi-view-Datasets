# Multi-view-Datasets (Comming soon)

In representation learning fields such as multi-view clustering, researchers tend to focus more on algorithms within the feature space, predominantly utilizing public datasets. This offers considerable convenience, as obtaining public datasets is generally free from strict copyright restrictions, sparing us the arduous task of dataset construction. However, existing repositories fail to provide a comprehensive and unified public dataset library specifically dedicated to the field of multi-view representation learning. Therefore, I aim to systematically organize and compile the multi-view datasets I have collected throughout my research process.

| Datasets Name | Sampel num | View_num | Classes_num | Link | 
| :--- | :---: | :---: | :---: | :---: |
| BDGP | 2500 | 2 | 5 | [BDGP](#BDGP)|
| BBCSport | 544 | 5 | 2 | [BBCSport](#BBCsport)|
| NGs | 500 | 3 | 5 |[NGs](#NGs) |
| Cora | 2708 | 2 | 7 |[Cora](#Cora) |
| Movies | 617 | 2 | 17 | [Movies](#Movies) |
|Hdigit| 10000 | 2 | 10 | [Hdigit](#Hdigit) |
|CIFAR-10| 50000|3|10|[CIFAR-10]|
<a name="my-anchor"></a> Datasets with large file sizes can be found in the cloud drive: [MVC_datasets](https://drive.google.com/drive/folders/14TEYr4L82iKSKhTxt70End6ucGlhJTlS?usp=drive_link)

### BDGP
Berkeley Drosophila Genome Project (BDGP): dataset consists of two views: image and text. Common references: Cai, Xiao, et al. "Joint stage recognition and anatomical annotation of drosophila gene expression patterns." Bioinformatics 28.12 (2012): i16-i24. Datasets: [Drive_link](#my-anchor)

### BBCSport
The dataset comprises 544 sports news articles collected from the BBC Sport website, covering five categories: Athletics, Cricket, Football, Rugby, and Tennis. To construct the multi-view data, each document was randomly
partitioned into two segments, and a term frequency matrix was generated for each segment to serve as a distinct view. 

### NGs
The dataset consists of 500 news articles spanning five distinct categories: Sports, Computers,
Science, Politics, and Religion. Three separate views were constructed using term frequency statistics, stemming, and
stop-word filtering, respectively. Each view has a dimensionality of 2,000. 

### Cora
The dataset consists of 2,708 samples sourced from an academic paper database, categorized into seven classes representing different subfields. Two views were constructed: a citation relationship view and a
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


