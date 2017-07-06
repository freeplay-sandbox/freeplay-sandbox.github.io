The Freeplay Sandbox Dataset
============================

![Screenshot of the dataset, viewed in RViz](media/3d-point-cloud-facial-features.jpg)

The **Freeplay Sandbox Dataset** (also called _PInSoRo dataset_) is a large, open-data dataset of chid-child and child-robot interactions.

Obtaining the dataset
---------------------

For legal and ethical reasons, the dataset is only available to **academics**.

The dataset exists in two flavours:

- the anonymised version, **with no video streams**, that can be freely
  downloaded once you fill in a short ethics declaration online and provide an
  academic email address.

- the full dataset, **include raw video streams**, that can be obtained after
  getting suitable **ethical clearance from your university ethics committee**.
  Due to the size of the full dataset (several terabytes), we share this
  version by shipping to you an (encrypted) harddrive with the data.

**The dataset will be available Autumn 2017**

### Dataset excerpt

For evaluation purpose, you can download a short excerpt (10 seconds) of the full dataset here:

_link to be added before the end of July 2017_

Dataset details
---------------

### Recorded data

Each play episode includes the following datastreams:

| **Domain**    | **Type**                                                           | **Details**                   |
|---------------|--------------------------------------------------------------------|-------------------------------|
| _child 1_     | audio                                                              | 16kHz, mono, semi-directional |
|               | face (RGB)                                                         | qHD (960x540), 30Hz           |
|               | face (depth)                                                       | VGA (640x480), 30Hz           |
|               | facial features                                                    | 68 3D points, 30Hz            |
| _child 2_     | audio                                                              | 16kHz, mono, semi-directional |
|               | face (RGB)                                                         | qHD (960x540), 30Hz           |
|               | face (depth)                                                       | VGA (640x480), 30Hz           |
|               | facial features                                                    | 68 3D points, 30Hz            |
| _environment_ | RGB                                                                | qHD (960x540), 29.7Hz         |
| _touchscreen_ | background drawing (RGB)                                           | 4Hz                           |
|               | touches                                                            | 6 points multi-touch, 10Hz    |
|               | items position and orientation                                     | (x,y,theta), 10Hz             |
| _annotations_ | timestamped annotations of social behaviours and remarkable events |                               |
| _other_       | static transforms between touchscreen and facial cameras           |                               |
|               | cameras calibration informations                                   |                               |

### Acquisition procedure


![Acquisition setup in the child-child condition](media/setup.png)




