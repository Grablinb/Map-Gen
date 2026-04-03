# Map Generation (Procedural Terrain)

## Description
This project is a procedural terrain generation system built in Unity.  
It generates 3D terrain meshes using multiple layers of Perlin noise to simulate natural landscapes.

## Core Features
- Terrain generation using layered Perlin noise
- Multiple noise layers (octaves) with different strength and scale
- Mesh-based terrain generation (custom mesh, not Unity Terrain)
- Height-based texturing system
- Configurable terrain parameters

## Technical Highlights
- Combined multiple Perlin noise layers to create more complex and natural terrain
- Used noise as a heightmap to generate mesh vertices
- Implemented height-based texture blending (e.g. water / ground / mountains)
- Adjustable parameters: scale, amplitude, frequency, seed
- Structured generation pipeline: noise → heightmap → mesh → textures

## Tech Stack
- Unity
- C#
- Mathf.PerlinNoise()

## How it Works
1. Generate multiple Perlin noise layers
2. Combine them using different weights (octaves)
3. Convert noise values into height values
4. Generate mesh vertices based on heightmap
5. Apply textures depending on height

## What I Learned
- How Perlin noise works and why it is used for terrain generation
- How to combine multiple noise layers for realistic results
- Mesh generation and vertex manipulation in Unity
- Converting mathematical data into visual geometry

## Future Improvements
- Infinite terrain (chunk system)
- Biome system (different terrain types)
- Better texture blending
- GPU-based generation for performance

## Links
- GitHub: https://github.com/Grablinb/Map-Gen
