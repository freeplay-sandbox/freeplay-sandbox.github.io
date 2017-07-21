The Freeplay Sandbox Dataset
============================

![The two conditions](media/setup-illustration.png)

The **Freeplay Sandbox Dataset** (also called _PInSoRo dataset_) is a large (120
children, 45h+ of RGB-D video recordings), open-data dataset of chid-child and
child-robot interactions.

These interactions are recorded during little-constrained **free play**
episodes. They emcompass a rich and diverse set of social behaviours.

<video src="media/bestof.mp4" controls>
Sorry, your browser doesn't support embedded videos, 
but don't worry, you can <a href="media/bestof.mp4">download it</a>
and watch it with your favorite video player!
</video>

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


Acquisition Procedure
---------------------

The 

![Acquisition setup in the child-child condition](media/setup.png)

Dataset Content
---------------

### Recorded data

![Screenshot of the dataset, viewed in RViz](media/3d-point-cloud-facial-features.jpg)

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

### Annotation of social interactions

![Screenshot of the annotation tool](media/annotator.jpg)

Using an [annotation tool](https://github.com/freeplay-sandbox/annotator/) specifically developped for this purpose, we are currently annotating the entire dataset with **high level social constructs**.

Specifically, the following constructs are annotated:


| **Task Engagement**   | goal-oriented play |
|                       | aimless play       |
|                       | adult seeking      |
|                       | no play            |
|-----------------------|--------------------|
| **Social Engagement** | solitary play      |
|                       | onlooker           |
|                       | parallel play      |
|                       | associative play   |
|                       | cooperative play   |
|-----------------------|--------------------|
| **Social attitude**   | pro-social         |
|                       | adversarial        |
|                       | assertive          |
|                       | frustrated         |
|                       | passive            |


Commonly observed social dynamics are mapped to these constructs.
For instance, a sequence during which a child appears to be bored is annotated
as *passive*; an annoyed child would be *frustrated*, and the child being
annoying can be labelled as exhibiting an *adversarial* behaviour.

Other example include: a gentle hand grabbing would be *assertive* vs a
not-so-gentle hand grabbing that would be *adversarial*; manipulative or bossy
behaviours are labelled as *assertive*; when children laugh together, they
exhibit a *pro-social* attitude, etc.






