# Unity Sparse Voxel Octrees

A new, currently in-development method of rendering voxels using Sparse Voxel Octrees as seen in [Nvidia's paper: "Efficient Sparse Voxel Octrees – Analysis, Extensions, and Implementation"](https://www.nvidia.com/docs/IO/88972/nvr-2010-001.pdf).

## Installation

Currently the only way to use the library is to download the files and compile them yourself in unity.

## Setup

Any camera that renders SVOs must have the SvoRenderer script attached with the appropriate shaders attached.

## TODO

- When a branch is changed, optimize it as well as its parent. (High Priority)
- Make Octree rendering work alongside Unity's normal rendering system. (Low Priority)
- Implement Beam Optimization as described in the Nvidia paper on pg. 13. (Low Priority)
