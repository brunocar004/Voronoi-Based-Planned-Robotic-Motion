# Voronoi-Based-Planned-Robotic-Motion
Research project meant to analyze the computational implications of environment complexity.

## Abstract
This project investigates the application of Voronoi diagrams in robotic motion planning, focusing on the computational implications of environment complexity. Using a Python-based simulation, we explore how obstacle count, shape complexity, and geometric perturbations affect Voronoi diagram generation and path-finding performance using Dijkstra's algorithm. We compare the impact of two obstacle representations—vertices and sampled edge points—on the resulting road map structure and runtime. Our results show that increasing obstacle complexity and edge sampling significantly increase computation time while improving path quality. We also find that Voronoi-based paths are sensitive to small perturbations in obstacle geometry. These findings highlight key trade-offs in geometric planning and underscore the importance of careful site selection in Voronoi-based navigation systems.

## Methodology

Constructed a Python-based simulation using the following libraries:
1. Shapely for geometric modeling of polygonal obstacles.
2. Scipy.spatial for generating Voronoi diagrams from point sites.
3. NetworkX for representing the Voronoi graph and running Dijkstra's algorithm.
4. Matplotlib for visualization.

Three key experimental questions guided the design:
1. How does computation time scale with the number of obstacles and their complexity?
2. How sensitive is the Voronoi diagram to small perturbations in obstacle shape and position?
3. How does using obstacle vertices versus edge sample points affect computation time and pathfinding behavior?
