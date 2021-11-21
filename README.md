# Solar-Panel-Detection-using-MaskRCNN

PHOTOVOLTAIC (PV) solar energy conversion has become one of the most promising renewable power generation sources (i.e., solar energy and wind energy) in the energy sector to drive low-carbon energy provisioning across the world. Much of this growth is from distributed residential solar, which is most often solar panels on the roofs of houses. This distributed solar energy has been historically difficult to integrate into the electrical grid due to the two-way electricity flow created between times of high and low solar irradiance. Accurate real time predictions of the net energy added to the grid could be helpful for utility companies to manage the distributed solar energy contribution, especially in areas where solar energy can account for a significant portion of the daytime power production. As the number of solar installations continues to increase, they will become more difficult to track and monitor. The goal of this project is to develop a tool to locate solar panels in high resolution satellite images, which could passively and automatically monitor the size and location of distributed residential solar panels. In particular, high-resolution satellite remote sensing images and artificial intelligence (AI) algorithms will be leveraged. More detailed objectives of this project are summarized as below. 

1.	Summarize the existing open-access satellite/UAV remote sensing datasets on solar panel mapping with details. 

2.	Learn how to download high-resolution satellite images (e.g. google earth images) and do the labelling by using some solar panel examples in Colchester area (choose labelling tools of your interest). 

3.	Building deep learning (e.g. transfer learning) models from the labelled datasets and verify its performance. 

4.	Apply the built model in different areas of interest in Colchester to generate the solar panel mapping and make a comparison for them. 

**Mask RCNN**

Object detection is one of the foremost vital areas in the field of Computer vision. Significant
number of results has been produced in this field by many researchers around the world by the
rise of Convnets and transfer learning techniques. But more advanced techniques incorporate
Region proposal methods, Single shot methods, Anchor box methods and so on. We are
curious to know more about Mask RCNN, but, before that we need to touch slight basics
about segmentation.

What actually is Image Segmentation?

“In computer vision, image segmentation is the process of dividing an image into different regions based on the characteristics of the pixels to identify objects or boundaries to simplify an image and analyze it more efficiently.” 

The Mask RCNN is further continuation with Faster RCNN, which has an additional branch to predict the segmentation masks on each RoI in a pixel-to-pixel manner.

Mask RCNN consists of two parts.

 Region proposal network to propose bounding boxes around the object of interest.

 A binary mask classifier to generate mask for every classes in the image.
Mask RCNN is built on top of the Faster RCNN model. In addition, Mask RCNN will return
object mask.

Compared to the ConvNet that is being used in Faster RCNN to extricate the feature maps, ResNet101 architecture is used to extract the features in the Mask RCNN.

**Labelling Software: LabelMe**

The labelling tool plays a crucial role in object detection. The purpose of the labelling is to
highlight the object of interest in the image, so that the machine will be able to read it. The
highlighted images are then trained and then make the model to learn what each highlighted
object in the image are. With the help of labelling software, we can develop a functional deep
learning model. Pixel wise annotation is followed in segmentation tasks, where every pixel in
the image is assigned to a class. 
The software used for labelling the images in this project is ‘LabelMe’. Using this software,
the image data are annotated with the class for solar panel detection. A sample of the
annotated image from the labelling tool is shown below: 

![image](https://user-images.githubusercontent.com/75327547/142772473-cf567036-4ed6-4892-abfb-3dbdf14e7bd4.png)

**Algorithm Design:**

![image](https://user-images.githubusercontent.com/75327547/142772510-211412c5-9bc3-445f-a630-c75d133f8292.png)

**Folder Structure:**

Test label
![image](https://user-images.githubusercontent.com/75327547/142772569-7677fa69-85d2-4648-ae10-5052dc71b590.png)


