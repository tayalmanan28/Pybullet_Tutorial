# Pybullet Tutorial

## Setup

### Conda Environment Setup

To install Anaconda follow the instructions in this [webpage](https://www.digitalocean.com/community/tutorials/how-to-install-the-anaconda-python-distribution-on-ubuntu-20-04-quickstart)

Create a conda environment for the PyBullet tutorial:  
```
$ conda create --name pyb  
```
Switch to the newly create environment (you will notice the name of the environment on the command line in the extreme left):  
```
$ conda activate pyb  
```

Then, clone the repository on your system:
```
git clone https://github.com/tayalmanan28/Biped-Pybullet.git
```
Install the following required packages:
```
pip install -r requirements.txt
```

### Checking Pybullet Installation

To check the installation launch:  
```
$ python  
```

Inside the python environment import the pybullet and matplotlib libraries:  
```
>> import pybullet
>> import matplotlib
```
If this command executes without any error then the installation is successful. 

## Description of Files

* Kinematics of a serial-2R manipulator (notebook: [kinematics.ipynb](https://github.com/tayalmanan28/Pybullet_Tutorial/blob/main/kinematics.ipynb))
    * Forward kinematics  
    * Inverse kinematics  
    * Verification of the FK and IK modules against each other  .


* Introduction to PyBullet (notebook: [sim_env_setup.ipynb](https://github.com/tayalmanan28/Pybullet_Tutorial/blob/main/sim_env_setup.ipynb))
    * How to start a PyBullet session  
    * Settings the simulation parameters in PyBullet  
    * Loading URDF files in PyBullet  


* Torque control of robot state in PyBullet (notebook: [torque_control.ipynb](https://github.com/tayalmanan28/Pybullet_Tutorial/blob/main/kinematics.ipynb))
    * Obtaining joint information  
    * Setting the control mode (and enabling the motors)  
    * Control of joint torque  


* PID control of robot (notebook: [torque_control.ipynb](https://github.com/tayalmanan28/Pybullet_Tutorial/blob/main/kinematics.ipynb))
    * Reading the joint state  
    * Determining the control action  
    * Setting the required control torque  


* Point-to-point tracking of end-effector (notebook: [torque_control.ipynb](https://github.com/tayalmanan28/Pybullet_Tutorial/blob/main/kinematics.ipynb))
    * Obtaining the required joint angles to reach the desired end-effector position  
    * Simulating a PID position control loop to reach the desired end-effector position  
