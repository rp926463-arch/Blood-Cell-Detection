
### Problem Statement:
We will be working on a healthcare related dataset and the aim here is to solve a Blood Cell Detection problem. Our task is to detect all the Red Blood Cells (RBCs), White Blood Cells (WBCs), and Platelets in each image taken via 
microscopic image readings. Below is a sample of what our final predictions should look like:

#### Overview of dataset

* You can see a example of the labeled cell image.

  We have three kind of labels :

  * RBC (Red Blood Cell)
  * WBC (White Blood Cell)
  * Platelets (Platelets)

  ![image5](./research/data/BLOOD_CELLS_output/image5.png)

### Data preparation
Data preparation is important to use machine learning. In this project, the SSD algorithm for Object Detection is used.

* The structure of the `BCCD_dataset`

  ```
  ├── images
  │   ├── train
  │   │   |___BloodImage_00XYZ.jpg (312 items including annotations for respective images)
  │   |
  │   └── test
  │       |___BloodImage_00XYZ.jpg (52 items)
  ├── LICENSE
  └── README.md
  ```



* The `Annotations` : The VOC format `.xml` for Object Detection, automatically generate by the label tools. Below is an example of `.xml` file.

  ```xml
  <annotation>
  	<folder>JPEGImages</folder>
  	<filename>BloodImage_00000.jpg</filename>
  	<path>/home/pi/detection_dataset/JPEGImages/BloodImage_00000.jpg</path>
  	<source>
  		<database>Unknown</database>
  	</source>
  	<size>
  		<width>640</width>
  		<height>480</height>
  		<depth>3</depth>
  	</size>
  	<segmented>0</segmented>
  	<object>
  		<name>WBC</name>
  		<pose>Unspecified</pose>
  		<truncated>0</truncated>
  		<difficult>0</difficult>
  		<bndbox>
  			<xmin>260</xmin>
  			<ymin>177</ymin>
  			<xmax>491</xmax>
  			<ymax>376</ymax>
  		</bndbox>
  	</object>
      ...
  	<object>
  		...
  	</object>
  </annotation>
  ```


"# Blood-Cell-Detection" 
