# Background

The knowledge of the road surface states is essential for improving the safety and the ride comfort of autonomous vehicles. Previewing the road conditions with vision sensor is verified to be an effective solution. However, there is still a lack of a large-scale road surface image dataset. Therefore, we publish this *Road Surface Classification Dataset (RSCD)* with detailed road material, friction and roughness level annotations.

# Dataset Description

## Data acquisition

The original pictures are captured with a USB camera as shown in Figure 1. To ensure a high resolution of the road surface area, the camera is mounted on the bonnet and have a certain depression angle. The pictures are collected and stored with an IPC.

![](img/73700cbe3a4288b07634d10d4e39bed7.png)

Figure 1. Camera installation

Aiming at developing practical driving assistance applications, we conducted real-vehicle image acquisition under as many working conditions as possible. The generalization capability of the classification algorithm to be developed is enlarged at the dataset level. The experiments lasted from January to July, 2022 at Beijing and covered about 600 kilometers of roads.

Considering the fact that only the road area that the tires pass would affect the vehicle response, we crop the road surface area of the original pictures into patches with size 360\*240. The patches are labeled manually according to the class definition below.

## Class definition

The friction level, material, and unevenness properties of roads are essential for chassis control and driving assistance.

-   The friction level property contains six subclasses corresponding to different weather conditions, i.e. dry, wet, water, fresh snow, melted snow, and ice.
-   The road material property consists of asphalt, concrete, mud, and gravel.
-   The road unevenness is divided into smooth, slight unevenness, and severe unevenness according to the amplitude of the road undulation.

The subclasses of the three road properties are combined to form the class definition of the dataset. It should be noted that the road material and unevenness are not annotated when the friction levels are fresh snow, melted snow, or ice. Also, the unevenness is not labeled for mud or gravel roads. Finally, we get 27 combined classes. Also, researchers can use part of the labeled properties to develop their own applications.

![](img/0b21fdac7d360cf991a31a85c384153f.png)

Figure 2. Road properties and the subclasses

Image samples of part of the classes are shown in Figure 3. The number of images for each class is shown in Fig. 4.

![](img/2b96c808d26592eeb217549f150a97fa.jpeg)

Figure 3. Sample images of part of the classes. (a). dry-asphalt-smooth (b). dry-asphalt-slight (c). dry-asphalt-severe (d). water-asphalt-severe (e) wet-asphalt-slight (f). wet-concrete-smooth (g). wet-concrete-severe (h). water-concrete-slight (i). water-mud (j). dry-gravel (k). melted snow (l). ice.

![](img/a069d465da1211286ec077aea196e301.jpeg)

Figure 4. Number of images for each class.

# How to Use

The RSCD is completely open to academic research. To use the dataset, please cite:

Tong Zhao, Yintao Wei, A road surface image dataset with detailed annotations for driving assistance applications, Data in Brief, 2022. doi: 10.1016/j.dib.2022.108483

Any questions, please contact us: zhaot20@mails.tsinghua.edu.cn

# Download RSCD

Google Drive:

[Download](https://drive.google.com/file/d/10lQfIWUy1V1UIabfmyTeR0U5hLE4Mj6K)
