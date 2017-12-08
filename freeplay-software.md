Re-using the Free-Play Sandbox paradigm
=======================================

You might want to first familiarize yourself with the paradigm by reading the
[reference article *The Free-play Sandbox: a Methodology for the Evaluation of
Social Robotics and a Dataset of Social
Interaction*](https://arxiv.org/abs/1712.02421).

To use the *Free-play Sandbox* paradigm yourself, run your own studies, and
acquire new data, you need a sandtray (essentially, a large touchscreen -- in
our experiments, we use a 27" one -- used as an interactive table), and the
following pieces of open-source software:

1. The [user interface](https://github.com/freeplay-sandbox/qt-gui) (written in Qt QML);

2. The [core](https://github.com/freeplay-sandbox/core) acquisition and robot
  control pipeline, written in C++ and Python, and using extensively
  [ROS](https://www.ros.org);

3. The [supervisor](https://github.com/freeplay-sandbox/web-supervisor) for the
  experimenter to control the whole system and conveniently record participants
  (Python + HTML).

(1) is meant to run directly on the sandtray computer; (2) can run on the sandtray
computer or on another external computer; (3) has a 'server' component that must
run on the same computer as (2) and a experimenter interface that runs in a
browser (a tablet is especially convenient for this purpose).


**Note that all the provided code has been developped and tested on Linux** (Ubuntu
16.04). Since we rely on [ROS](https://www.ros.org), we **can not support
Windows or macOS**.

Visit each of the projects listed above (in that order) for installation notes.

Annotations of Social Interactions
----------------------------------

The reference coding scheme, as well as our custom tool to annotate recordings,
[is explained here](coding-scheme).

Analysis of the recorded data
-----------------------------

See [dataset analysis](analyse) for an overview of the tools and code snippets
we provide.

