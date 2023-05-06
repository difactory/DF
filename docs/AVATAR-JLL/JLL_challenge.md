# Challenges of AVATAR Joint Learning Lab - VR & Robotics Lab 


This document presents the challenges for the AVATAR JLL, making reference to the general [workflow documentation](JLL_doc#2-workflow). 
The aim of the challange is to make practice with digital twin and VR technologies addressing a simplified problem that still makes sense from an industrial perspective while using real data.

## Scene Configutation

The [PERFORM Lab](JLL_doc#1-perform-lab) is considered for the setup of the challenges. The scene is configured as described in the main documentation, with the addition of one or more workpieces on the conveyor.
Each challenge makes reference to its own scene configuration, thus highlighting the reconfigurability of the digital twin.

## Goal of robot task

The goal of the robot task (for all challenges) is to place the end effector inside the hole of **Workpiece_1**.

## Personalization of VEB.js

It is reminded that the [configuration of VEB.js](JLL_doc#23-visualization-in-vr-environment) can be personalized using 1) local files or 2) specifying [URL parameters](https://virtualfactory.gitbook.io/vlft/tools/vebjs#url-parameters) pointing to remote files. In particular, the challenges will ask to personalize the animation. 

This is a full example showing the setting of all relevant URL parameters, if the second option is chosen:

http://ec2-54-174-51-194.compute-1.amazonaws.com/vebjs/?inputscene=https://difactory.github.io/repository/scenes/VL/PERFORM.json&repoMod3d=https://difactory.github.io/repository/models/VL/PERFORM/&inputanim=https://difactory.github.io/repository/scenes/VL/PERFORM_anim.json&inputenv=https://difactory.github.io/repository/scenes/VL/PERFORM_env.json

It is recommended to keep unchanged the value of parameters **repoMod3d** and **inputenv**. The value of **inputscene** will change according to the setup of the challenge. The value of **inputanim** must be personalized according to the results of the development tasks.



# Challenge #1 - Visualize Trajectories

Scene configuration:
- [spreadsheet](https://difactory.github.io/repository/spreadsheets/VL_STIIMA_PERFORM-C1.xlsx)
- [json file](https://difactory.github.io/repository/scenes/VL/PERFORM-C1.json)

[VEB.js visualization](http://ec2-54-174-51-194.compute-1.amazonaws.com/vebjs/?inputscene=https://difactory.github.io/repository/scenes/VL/PERFORM-C1.json&repoMod3d=https://difactory.github.io/repository/models/VL/PERFORM/&inputanim=linkToBeAdded&inputenv=https://difactory.github.io/repository/scenes/VL/PERFORM-C1_env.json) (without setting of the animation, the string "linkToBeAdded" must be replaced accordingly).


The following trajectories are provided as [list of joint states](JLL_doc#241-robot-monitoring) defined in a JSON file:
- [trajectory_1.json](files/trajectory_1.json)
- [trajectory_2.json](files/trajectory_2.json)
- [trajectory_3.json](files/trajectory_3.json)
- [trajectory_4.json](files/trajectory_4.json)


# Challenge #2 - Receive a Trajectory via MQTT

Scene configuration:
- [spreadsheet](https://difactory.github.io/repository/spreadsheets/VL_STIIMA_PERFORM-C2.xlsx)
- [json file](https://difactory.github.io/repository/scenes/VL/PERFORM-C2.json)

[VEB.js visualization](http://ec2-54-174-51-194.compute-1.amazonaws.com/vebjs/?inputscene=https://difactory.github.io/repository/scenes/VL/PERFORM-C2.json&repoMod3d=https://difactory.github.io/repository/models/VL/PERFORM/&inputanim=linkToBeAdded&inputenv=https://difactory.github.io/repository/scenes/VL/PERFORM-C2_env.json) (without setting of the animation, the string "linkToBeAdded" must be replaced accordingly).

# Challenge #3 - Generate a Trajectory

Scene configuration:
- [spreadsheet](https://difactory.github.io/repository/spreadsheets/VL_STIIMA_PERFORM-C3.xlsx)
- [json file](https://difactory.github.io/repository/scenes/VL/PERFORM-C3.json)

[VEB.js visualization](http://ec2-54-174-51-194.compute-1.amazonaws.com/vebjs/?inputscene=https://difactory.github.io/repository/scenes/VL/PERFORM-C3.json&repoMod3d=https://difactory.github.io/repository/models/VL/PERFORM/&inputanim=linkToBeAdded&inputenv=https://difactory.github.io/repository/scenes/VL/PERFORM-C3_env.json) (without setting of the animation, the string "linkToBeAdded" must be replaced accordingly).


