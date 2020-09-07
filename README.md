# Unity Sparse Voxel Octrees

A new, currently in-development method of rendering voxels using Sparse Voxel Octrees as seen in [Nvidia's paper: "Efficient Sparse Voxel Octrees – Analysis, Extensions, and Implementation"](https://www.nvidia.com/docs/IO/88972/nvr-2010-001.pdf).

## Installation

Currently the only way to use the library is to download the files and compile them yourself in unity.

## QuickStart

Attach OctreeModel to a GameObject. The model can be edited from a script by using the SetData() method along with the OctreeData class. The OctreeModel can be rendered by creating a material which uses the Custom/Octree shader.

## Limitations

- Deformations, such as vertex deformations commonly used to animate characters or other objects, are not implemented, and are not planned (If its even possible).
- No collider support. Unlike normal meshes, there is no built-in collider for representing an Octree. Any octree-based object will need to be represented using an approximate collider. This is not a huge deal, as an approximate collider is generally the more performant approach with traditional triangle-based meshes anyways. Theoretically, an exact octree collider could be made by recreating the octree using box colliders, but this would be memory intensive, and implementation would take time, so this is not planned.

## TODO

- When a branch is changed, optimize it as well as its parent.
