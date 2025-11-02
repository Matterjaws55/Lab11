BFS calculates and prioritizes paths by giving all moves an equal cost and expanding the nearest unvisited cell first, finding the shortest path in an unweighted grid. the Dijkstra’s Algorithm uses a priority queue to always explore the lowest-cost node next. It guarantees the shortest path in weighted grids. A* prioritizes nodes based on cost + heuristic, where the heuristic estimates remaining distance to the goal.

Dynamically updating obstacles in real-time can cause performance issues on larger more complicated grids as it recalculates and if an obstacle blocks the current path, the agent’s navigation data may become outdated during movement.

I would like to use A* for large open world maps depending on the type of game as it has spatial partitioning for specific regions.

If I were to add weighted cells like difficult terrain areas, I would store a movement cost for each grid, rather than making it just walkable or not walkable.