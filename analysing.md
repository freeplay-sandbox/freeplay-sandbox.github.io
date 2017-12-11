Dataset analysis
================

Writing software to analyse the dataset
---------------------------------------

We provide [software
templates](https://github.com/freeplay-sandbox/analysis-templates) to access the
dataset. If you are not familiar with ROS and `rosbag` in particular, we
recommend you to start from here.


Provided tools
--------------


Tools to analyse the dataset are split into two:

- basic scripts are available to generate quick statistics on the dataset
  (lengths of recordings, demographics...) and manipulate the dataset files
  (check integrity, copy, etc.). These scripts can be found [in the /tools
  directory of the dataset meta-data
  repository](https://github.com/freeplay-sandbox/dataset/).

- more advanced [analysis tools](https://github.com/freeplay-sandbox/analysis)
  that typically require compilation are also available.

*More documentation to be added soon -- if you have specific questions/needs,
please [open a ticket here](https://github.com/freeplay-sandbox/analysis/issues).*

Annotations of Social Interactions
----------------------------------

The reference coding scheme, as well as our custom tool to annotate recordings,
[is explained here](coding-scheme).


