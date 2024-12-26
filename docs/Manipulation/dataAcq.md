# Data Acquisition Methods

In order to carry out the learning from demonstrations process, it is necessary to have processes that are able to collect data directly from the user. With this data, the necessary learning processes can be carried out to apply to manipulation tasks with our robotic platform ADAM. In the following, we present the work focused on the field of data acquisition for the training of the different algorithms created in our laboratory.


## TAICHI (Tracking Algorithm for Imitation of Complex Human Inputs)

This project presents the TAICHI algorithm. This algorithm is focused on the tracking of people to collect data for the Imitation Learning technique. TAICHI is composed of a detection of the significant points of the human arm and its extraction and mapping to the robot, a Gaussian filtering process to smooth the movements and filter the sensor noise and an optimization algorithm that seeks to obtain through the inverse kinematics of the model the configuration that is closest to the human one and that does not generate collisions with its environment or with itself. The algorithm follows the following workflow:

[![SchemeTAICHI](../fig/SchemeTACIHI.png)](https://ieeexplore.ieee.org/abstract/document/10256343)

The method allows data to be taken on the simulated ADAM model and subsequently evaluated on the real robot. The algorithm can be used with a single RGBD camera and by users of different ages and builds. The algorithm has been tested with a variety of users and has shown good results in the tracking of the human arm and the generation of trajectories that can be used for imitation learning.

[![TAICHI](../fig/TAICHI.png)](https://ieeexplore.ieee.org/abstract/document/10256343)


