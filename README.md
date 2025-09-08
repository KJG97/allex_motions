# Robot Trajectory Data

This repository contains trajectory data for various robot motions.

## Folder Structure

Each folder represents a specific motion and contains the following CSV files:

### Motion Groups
- `crossarms_group/` - Cross arms motion
- `demo_group/` - Demo motion
- `hero_group/` - Hero pose motion
- `idle1_group/` ~ `idle5_group/` - Idle motions
- `no_group/` - No/rejection motion
- `nod_group/` - Head nodding motion
- `thinking_group/` - Thinking motion
- `thumbsup_group/` - Thumbs up motion
- `wave_group/` - Hand waving motion

### File Format
Each group contains the following CSV files:
- `Arm_L_theOne.csv` - Left arm trajectory
- `Arm_R_theOne.csv` - Right arm trajectory
- `Hand_L_*_wir.csv` - Left hand finger trajectories (index, middle, ring, little, thumb)
- `Hand_R_*_wir.csv` - Right hand finger trajectories (index, middle, ring, little, thumb)
- `theOne_neck.csv` - Neck trajectory
- `theOne_waist.csv` - Waist trajectory

## Data Format

The first row of each CSV file is a header, typically in the following format:
duration,joint_1,joint_2,joint_3,joint_4,joint_5,joint_6,joint_7


Each row represents joint degree values at a specific time.

## Usage

These trajectory data can be used for robot simulation or actual robot control.

## Robot System

This data is designed for use with the ALLEX humanoid robot system and can be integrated with Isaac Sim for simulation purposes.
