<h1 align="left">OpenAI Test-Bed of Contact Based Grasping for Reinforcement Learning</h1>

<h3 align="left">Project Description</h3>
<p align="left">
    This repo is a clone of my dissertation, which was submitted to the University of Liverpool 
    as required for my Masters in Computer Science.  Within it, two optical-tactile-based-sensors (GelSight)
    are simulated and appended to a UR5 arm.  Mujoco is used as the simulation environment - a physics extension to
    OpenAi's gym. This platform was utilised to construct the environments Reach, Push, Slide and PickandPlace
    (similar to those found within gym).  Which in turn act as a test-bed for training a deep reinforcement 
    learning agent using both Double Deep Q-Learning (DDQN) and Hierarchical Double Deep Q-Learning (HDDQN).
</p>

<p>
GelSightMujoco/  
<br>├── MUJOCO_LOG.TXT
<br>├── main.py
<br>├── agents/
<br>│   ├── __init__.py
<br>│   ├── bot_ddqn.py
<br>│   ├── bot_hddqn.py
<br>│   ├── utils/
<br>│   ├── __init__.py
<br>│   └── plotter.py
<br>├── envs/
<br>│   ├── __init__.py
<br>│   ├── RobotArm__BaseEnv.py
<br>│   ├── RobotArm__pick_and_place.py
<br>│   ├── RobotArm__push.py
<br>│   ├── RobotArm__reach.py
<br>│   ├── RobotArm__slide.py
<br>│   ├── models/
<br>│   │   ├── gripper_testbed_PickandPlace.xml
<br>│   │   ├── gripper_testbed_push.xml
<br>│   │   ├── gripper_testbed_reach.xml
<br>│   │   ├── gripper_testbed_slide.xml
<br>│   │   ├── temp_xml.xml
<br>│   │   ├── assets/
<br>│   │   ├── meshes/
<br>│   ├── utils/
<br>├── outputs/
<br>│   ├── design_documents/
<br>│   ├── design_documents/
<br>├── rl_algos/
<br>│   ├── design_documents/
<br>│   └── user_manuals/
</p>


<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://www.tensorflow.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"/> </a> </p>
