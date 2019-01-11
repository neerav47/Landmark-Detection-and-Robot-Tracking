# Project : Landmark Detection & Robot Tracking (SLAM)

## Description

In this project, we implement SLAM (Simultaneous Localization and Mapping for a 2 dimensional world.
We combine robot sensor measurements and movement to create a map of an environment from only sensor and motion
data gathered by a robot, over time. 

SLAM gives us a way to track the location of a robot in the world in real-time and identify the locations of landmarks such as buildings, trees, rocks, and other world features.

## Files

- `Notebook 1` : Robot moving and sensing
- `Notebook 2` : Omega and Xi, Constraints
- `Notebook 3` : Landmark detection and tracking
- `robot_class.py` : Robot object with its world
- `helpers.py` : helper functions

## Graph SLAM

To implement Graph SLAM, a matrix and a vector (omega and xi, respectively) are introduced. 
The matrix is square and labelled with all the robot poses (xi) and all the landmarks (Li).

Every time we make an observation, for example as we move between two poses by some distance
`dx` and can relate those two positions, you can represent this as a numerical relationship in these
matrices.

We are referring to robot poses as Px, Py and landmark positions as Lx, Ly, and one way to approach this challenge is to add both x and y locations in the constraint matrices.

