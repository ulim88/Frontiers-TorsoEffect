# Frontiers_TorsoEffect

We identify the effect of torso information on gait phase estimation using long short-term memory (LSTM).

The details of the proposed idea are described in the manuscript, "Effect of Torso Kinematics on Gait Phase Estimation for Enhancing Speed Adaptability."

This repository mainly contains two contents: (1) dataset and (2) Frontiers_gait_estimation.py.

(1) dataset

    This contains the processed data of 50 subjects in 5 different walking speeds: C1-C5.
    Each csv file is named as 'Combined_20XXXXX_YY_ZZ.csv.'
    20XXXXX refers to the subject id, and YY refers to the walking speed, while ZZ refers to the number of trials.
    In each dataset, 11 columns are contained.
        - Index: data index
        - LeftHS: linear label based on left heel-strike
        - RightHS: linear label based on right heel-strike
        - LThighAngle: calculated left thigh angular position
        - RThighAngle: calculated right thigh angular position
        - TorsoAngle: calculated torso angular position
        - LThighVelocity: calculated left thigh angular velocity
        - RThighVelocity: calculated right thigh angular velocity
        - TorsoVelocity: calculated torso angular velocity
    
(2) Frontiers_gait_estimation.py

    This is the main code for training the given dataset using the proposed networks.
