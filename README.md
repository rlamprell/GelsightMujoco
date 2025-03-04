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

## Quick Start
- install mujoco - https://mujoco.org/
- git clone the repo
- cd into repo_path/Test_bed
- run python main.py
- download any missing packages

## Settings
<html>
<body>
<table>
  <tr>
    <th>Parameter</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>env</td>
    <td>Choose an environment to run</td>
  </tr>
  <tr>
    <td>render</td>
    <td>Draw the environment as it runs?</td>
  </tr>
  <tr>
    <td>random_spawns</td>
    <td>Randomize the placement of objects in the environment</td>
  </tr>
  <tr>
    <td>gelsight_dims</td>
    <td>Resolution of the internal GelSight camera</td>
  </tr>
  <tr>
    <td>envcam_dims</td>
    <td>Resolution of the agent's (and yours if render=True) view of the environment</td>
  </tr>
  <tr>
    <td>image_rescale</td>
    <td>Should the images be scaled down?</td>
  </tr>
  <tr>
    <td>image_grayscale</td>
    <td>Should the images be grayscale?</td>
  </tr>
  <tr>
    <td>image_normalise</td>
    <td>Should the images be normalized?</td>
  </tr>
  <tr>
    <td>framestack</td>
    <td>Should the frames be stacked when passed to the neural network</td>
  </tr>
  <tr>
    <td>k_frames</td>
    <td>How many frames should be in the stack</td>
  </tr>
  <tr>
    <td>agent</td>
    <td>The deep reinforcement learning algorithm to run</td>
  </tr>
  <tr>
    <td>mode</td>
    <td>Are we training or testing?</td>
  </tr>
  <tr>
    <td>number_of_episodes</td>
    <td>Episodes that must be completed before the agent and environment stop</td>
  </tr>
  <tr>
    <td>model_weights0</td>
    <td>Are you loading any weights for the first neural network?</td>
  </tr>
<tr>
    <td>model_weights1</td>
    <td>Are you loading any weights for the second neural network (hddqn)?</td>
  </tr>
  <tr>
    <td>replay_buffer_size</td>
    <td>How many memories do you want to store?</td>
  </tr>
  <tr>
    <td>batch_size</td>
    <td>How many states do you want to select at a time to learn from</td>
  </tr>
  <tr>
    <td>alpha_lr</td>
    <td>The learning rate</td>
  </tr>
  <tr>
    <td>beta_lr</td>
    <td>The learning rate for the second neural network (hddqn)</td>
  </tr>
  <tr>
    <td>nn_dense</td>
    <td>The density of layers in the neural network post concatenation - following conv2d and any kinematics</td>
  </tr>
  <tr>
    <td>nn_num_dense</td>
    <td>The density of layers for any kinematic inputs</td>
  </tr>
  <tr>
    <td>ext_nn_dense</td>
    <td>(hddqn) The density of layers in the neural network post concatenation - following conv2d and any kinematics</td>
  </tr>
  <tr>
    <td>ext_nn_num_dense</td>
    <td>(hddqn) The density of layers for any kinematic inputs</td>
  </tr>
  <tr>
    <td>transfer_model</td>
    <td>Transfer learning from another model - conv2d only</td>
  </tr>
  <tr>
    <td>type_</td>
    <td>What type of data should be included? [vision, tactile, kinematics, raw]</td>
  </tr>
  <tr>
    <td>extrinsic_type2_</td>
    <td>(hddqn) What type of data should be included? [vision, tactile, kinematics, raw]</td>
  </tr>
  <tr>
    <td>seed</td>
    <td>Randomization seed</td>
  </tr>
</table>
</body>
</html>


## Architecture

## Results

## Next Steps:
- create requirements.txt
- create gitignore
- refactor and optimise code
  

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://www.tensorflow.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"/> </a> </p>


