---
layout: page
title: Documentation of the CoAx Dataset
permalink: /doc-coax/
---

<div class="section-t"><b> CoAx: Collaborative Action Dataset for Human Motion Forecasting in an Industrial Workspace.</b>
    <p ><b> Lagamtzis, Dimitrios</b>;  Schmidt, Fabian; Seyler, Jan; and Dang, Thao 
    <br><small><i>accepted at ICAART 2022 - published by SCITEPRESS</i></small>
    <br><a target="_blank" href="https://www2.hs-esslingen.de/public/##/_public/coax-dataset/coax-paper@@pdf" onmouseover="this.href=this.href.replace('@@','.'); this.href=this.href.replace('##','Faculty-IT-Media')">pdf</a>
    <a href="/dataset-coax/">dataset</a>
    <a target="_blank" href="https://doi.org/10.5220/0010775600003116">doi</a>
    </p>
</div>

<div class="section-t" >
<h3>Sequential Task Descriptions</h3>
<h4><b>Task 1: Valve Terminal Plug & Play</b></h4>
<p>In this task a human agent is setting up a valve terminal with a valve. This involves actions like screwing the valve into the valve terminal and also grabbing and installing a hose. The screws are already placed in their position for simplicity reasons. This task is intended to show a typical assembly as it might occur in a collaborative industrial workspace.</p>

<h4><b>Task 2: Valve Assembly</b></h4>
<p>In this particular task, a valve is assembled from its individual parts. The screws belong to the actual objects of the scene and are located in a designated box. Two screws are used to assemble the main modules of the valve. The last step in the assembly is the attachment of the membrane in its designated place, likewise, stored in a box in the scene.</p>

<h4><b>Task 3: Collaborative Soldering</b></h4>
<p>The final task explicitly shows a collaboration between the human actor and the robot in the workspace. The robot assists the human in a soldering task by acting as a third arm. Once the robot recognizes the human's intention to solder, it reaches the soldering board, holding it for the human and aligning it so that the human can solder a capacitor onto it. This task involves the human waiting for the robot in order to continue.</p>
</div>

<div class="section-t" overflow-x="scroll" >
<h3> Object annotation </h3>
<table class="datasetTable">
<thead>
<tr>
<th><b>ID</b></th>
<th><b>Object</b></th>
<th><b>Human Readable</b></th>
</tr>
</thead>
<tbody>
<tr>
<td>0</td>
<td>screwdriver</td>
<td>Screwdriver</td>
</tr>
<tr>
<td>1</td>
<td>hose</td>
<td>Hose</td>
</tr>
<tr>
<td>2</td>
<td>valve</td>
<td>Valve</td>
</tr>
<tr>
<td >3</td>
<td>valve_terminal</td>
<td>Valve terminal</td>
</tr>
<tr>
<td>4</td>
<td>box_w_screws</td>
<td>Box with screws</td>
</tr>
<tr>
<td>5</td>
<td>box_w_membrane</td>
<td>Box with membrane</td>
</tr>
<tr>
<td>6</td>
<td>soldering_station</td>
<td>Soldering station</td>
</tr>
<tr>
<td>7</td>
<td>soldering_iron</td>
<td>Soldering iron</td>
</tr>
<tr>
<td>8</td>
<td>soldering_tin</td>
<td>Soldering tin</td>
</tr>
<tr>
<td>9</td>
<td>soldering_board</td>
<td>Soldering board</td>
</tr>
<tr>
<td>10</td>
<td>capacitor</td>
<td>Capacitor</td>
</tr>
<tr>
<td>11</td>
<td>robot</td>
<td>Robot</td>
</tr>
<tr>
<td>12</td>
<td>human</td>
<td>Human</td>
</tr>
<tr>
<td>13</td>
<td>RightHand</td>
<td>Right hand</td>
</tr>
<tr>
<td>14</td>
<td>eef_robot</td>
<td>Robot's end effector</td>
</tr>
<tr>
<td>15</td>
<td>robot_base</td>
<td>Robot's base</td>
</tr>
</tbody>
</table>
</div>

<div class="section-t" overflow-x="scroll" id="vert">
<h3>Action annotation - sequential order</h3>
<table class="datasetTable">
<thead>
<tr>
<th><b>Task 1</b></th>
<th><b>Task 2</b></th>
<th><b>Task 3</b></th>
</tr>
</thead>
<tbody>
<tr>
<td style="background:#FF4D4F">approach</td>
<td style="background:#FF4D4F">approach</td>
<td style="background:#FF4D4F">approach</td>
</tr>
<tr>
<td style="background:yellow">grab valve</td>
<td style="background:yellow">grab valve</td>
<td style="background:yellow">grab capacitor</td>
</tr>
<tr>
<td style="background:#A9D08E">plug valve</td>
<td style="background:#F4B084">join valve components</td>
<td style="background:#D88FD9">wait for robot</td>
</tr>
<tr>
<td style="background:yellow">grab screwdriver</td>
<td style="background:yellow">grab screws</td>
<td style="background:#A9D08E">plug capacitor</td>
</tr>
<tr>
<td style="background:#BDD7EE">screw valve</td>
<td style="background:#A9D08E">plug screws</td>
<td style="background:#D88FD9">wait for robot</td>
</tr>
<tr>
<td style="background:#D0CECE">release screwdriver</td>
<td style="background:yellow">grab screws</td>
<td style="background:yellow">grab soldering tin</td>
</tr>
<tr>
<td style="background:yellow">grab hose</td>
<td style="background:#A9D08E">plug screws</td>

<td style="background:yellow">grab soldering iron</td>
</tr>
<tr>
<td style="background:#A9D08E">plug hose</td>
<td style="background:yellow">grab screwdriver</td>

<td style="background:#00FFCF">solder capacitor</td>
</tr>
<tr>
<td style="background:#FF8800">retreat</td>
<td style="background:#BDD7EE">screw valve</td>

<td style="background:#D0CECE">release soldering iron</td>
</tr>
<tr>
<td>&nbsp;</td>
<td style="background:#D0CECE">release screwdriver</td>
<td style="background:#D0CECE">release soldering tin</td>
</tr>
<tr>
<td>&nbsp;</td>
<td style="background:#2D54EE">place valve</td>
<td style="background:#FF8800">retreat</td>
</tr>
<tr>
<td>&nbsp;</td>
<td style="background:yellow">grab membrane</td>
<td>&nbsp;</td>
</tr>
<tr>
<td>&nbsp;</td>
<td style="background:#2D54EE">place membrane</td>
<td>&nbsp;</td>
</tr>
<tr>
<td>&nbsp;</td>
<td style="background:#FF8800">retreat</td>
<td>&nbsp;</td>
</tr>
</tbody>
</table>
</div>

<div class="section-t" >
    <h3>Action annotation - encoded with object relations</h3>
<table class="datasetTable" id="enc-ac-center">
    <thead >
        <tr>
        <th id="enc-ac-center" ></th>
        <th id="enc-ac-center" ></th>
        <th  id="enc-ac-center" scope="col">0</th>
        <th  id="enc-ac-center" scope="col">1</th>
        <th  id="enc-ac-center" scope="col">2</th>
        <th  id="enc-ac-center" scope="col">3</th>
        <th  id="enc-ac-center" scope="col">4</th>
        <th  id="enc-ac-center" scope="col">5</th>
        <th  id="enc-ac-center" scope="col">6</th>
        <th  id="enc-ac-center" scope="col">7</th>
        </tr>
        <tr>
        <th  id="enc-ac-center" scope="row">&nbsp;</th>
        <th  id="enc-ac-center" scope="row">&nbsp;</th>
        <th  id="enc-ac-center" scope="row">valve</th>
        <th  id="enc-ac-center" scope="row">capacitor</th>
        <th  id="enc-ac-center" scope="row">screwdriver</th>
        <th  id="enc-ac-center" scope="row">screws</th>
        <th  id="enc-ac-center" scope="row">membrane</th>
        <th  id="enc-ac-center" scope="row">soldering tin</th>
        <th  id="enc-ac-center" scope="row">soldering iron</th>
        <th  id="enc-ac-center" scope="row">hose</th>
        </tr>
    </thead>
    <tr>
      <th scope="row">0</th>
      <th scope="row" style="background:#FF4D4F">approach</th>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
      <td>&nbsp;</td>
    </tr>
    <tr>
      <th scope="row">1</th>
      <th scope="row" style="background:yellow">grab</th>
      <td>X</td>
      <td>X</td>
      <td>X</td>
      <td>X</td>
      <td>X</td>
      <td>X</td>
      <td>X</td>
      <td>X</td>
    </tr>
    <tr>
        <th scope="row">2</th>
        <th scope="row" style="background:#A9D08E">plug</th>
        <td>X</td>
        <td>X</td>
        <td>&nbsp;</td>
        <td>X</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>X</td>
      </tr>
      <tr>
        <th scope="row">3</th>
        <th scope="row" style="background:#F4B084">join</th>
        <td>X</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <th scope="row">4</th>
        <th scope="row" style="background:#D88FD9">wait for robot</th>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <th scope="row">5</th>
        <th scope="row" style="background:#BDD7EE">screw</th>
        <td>X</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <th scope="row">6</th>
        <th scope="row" style="background:#D0CECE">release</th>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>X</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>X</td>
        <td>X</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <th scope="row">7</th>
        <th scope="row" style="background:#00FFCF">solder</th>
        <td>&nbsp;</td>
        <td>X</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <th scope="row">8</th>
        <th scope="row" style="background:#2D54EE">place</th>
        <td>X</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>X</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <th scope="row">9</th>
        <th scope="row" style="background:#FF8800">retreat</th>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
  </table>
</div>

### Encoded Action Object Example:
Example of the approaching action from frame 0 to 50:


`[0,null]` refers to action with `ID == 0`(approach) and no action object (`null`) 

```json
{"right_hand": [0, [0,null], 50]}
```
Example of grabbing capacitor action from frame 75 to 100:

```json
{"right_hand": [75, [1,1], 100]}
```								
<div class="section-t" ></div>

### Derived Data
Information in 2D and 3D for each frame of each recorded sequence for every object in the scene. The 2D bounding boxes are given in pixel coordinates. The 3D bounding box units are in meters; in the robot's coordinate system. To capture the dataset, an Intel RealSense Depth Camera D435 was used, capturing images at 15 fps with a resolution of 640 px × 480 px.

```json
{
    "bounding_box": {
        "x0": -0.6319517876324395,
        "x1": -0.4992021971049271,
        "y0": -0.363614762245568,
        "y1": -0.33810236065083654,
        "z0": -0.29955900722097994,
        "z1": -0.2845506851112529
    },
    "certainty": 1.0,
    "class_index": 0,
    "class_name": "screwdriver",
    "colour": [0.18431, 0.3098, 0.3098],
    "instance_name": "screwdriver_0",
    "past_bounding_box": {
        "x0": -0.6286039463676328,
        "x1": -0.5072747525732543,
        "y0": -0.3633770115164791,
        "y1": -0.3387509672664858,
        "z0": -0.29565532742319667,
        "z1": -0.2746970149582395
    }
}
```

As referenced in our paper, we adapted the format of our dataset from [[1]](/doc-coax/#ref-dreher).

<div class="section-t"></div>


 
### Dataset samples
How you can load the dataset and work with the derived data. Short intro and hands-on by showing a code snippet using a jupyter notebook. Utility functions are encapsulated in a `util.py`, that can be located in the `src` directory of our dataset's [GitHub-Repository](https://github.com/dlgmtzs/coax-dataset).

Here we give a short preview of the repository and its functionalities:

#### Get `images` and `depth images` for selected `identifier` sequence

##### &#10071;it is **important** to set the flag `flags=-1`, when **reading in** the `depth images` with `cv2.imread(file,flags=-1)`


```python
images = [cv2.imread(file) for file in sorted(glob.glob(img_path+identifier+"*.png"))]
depth_images = [cv2.imread(file,flags=-1) for file in sorted(glob.glob(dpth_img_path+identifier+"*.png"))]
```

##### Plot `rgb` and `depth` image


```python
frame_id = 70
```


```python
plt.imshow(cv2.cvtColor(images[frame_id], cv2.COLOR_BGR2RGB ));
```
    
<center><img src="../../assets/output_16_0.png" alt="png" > </center>

    
```python
plt.imshow(depth_images[frame_id]);
```
 
<center><img src="../../assets/output_17_0.png" alt="png" > </center>
    


#### Choose which`frame` you want to investigate closer or loop over all frames


```python
frame_id = 70
```


```python
rgbxyz = coax.get_rgb_xyz_for_frame(frame=frame_id,
                                    images=images,
                                    depth_images=depth_images,
                                    camParams=camParams)
```

#### Get 3D Bounding Boxes of every object for every frame
    - Get processed dataframes for every frame
    - Plot Pointcloud with 3D Object Bounding Boxes and center points


```python
dfs_3d, obj_dfs_3d = coax.get_3d_processed_dfs_per_frame(
                                          derived_data_path=derived_data_path, 
                                          identifier=identifier)
```


```python
%matplotlib inline
coax.plot_rgbxyz_with_bounding_boxes(frame=frame_id,
                                     rgbxyz=rgbxyz,
                                     obj_dfs=obj_dfs_3d,
                                     save=False)
```


<center><img src="../../assets/output_24_0.png" alt="png" > </center>


#### Get 2D Bounding Boxes of every object for every frame
    - Get processed dataframes for every frame
    - Plot Pixel-Image with 2D Object Bounding Boxes and center points


```python
dfs_2d, obj_dfs_2d = coax.get_2d_processed_dfs_per_frame(
                                          derived_data_path=derived_data_path, 
                                          identifier=identifier)
```


```python
%matplotlib inline
coax.plot_rgb_with_bounding_boxes(frame=frame_id,
                                  images=images,
                                  obj_dfs=obj_dfs_2d,
                                  save=False)
```


<center><img src="../../assets/output_27_0.png" alt="png" > </center>
    



You can find further instructions on how to work with the dataset on our  <a target="_blank" href="https://github.com/dlgmtzs/coax-dataset">GitHub-Repository</a>.




<div class="section-t" ></div>


### References

<div id="ref-dreher" style="line-height: 1.35; margin-left: 2em; text-indent:-2em; font-size:12px">
  [1] Dreher, C. R. G., Mirko Wächter, and Tamim Asfour. “Learning Object-Action Relations from Bimanual Human Demonstration Using Graph Networks.” <i>IEEE Robotics and Automation Letters</i> 5, no. 1 (January 2020): 187–194. <a href="https://doi.org/10.1109/LRA.2019.2949221"></a>
</div>
