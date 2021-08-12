# Pathfinding
Unity pathfinding course using graphs and trees

Hello this is from a Udemy course on Unity using pathfinding algorithms from graphs and trees, such as the A* algorithm to navigate AI or the player through a maze or obstacles.

Here are the list of methods to search through the map:
1. BFS - Uses a queue to search all the present neighbor nodes at a certain depth before moving to the next cluster of neighbor nodes. However it will only find the shortest path in an unweighted graph (which isn't the case for this project). 
2. Dijsktra - Finds the shortest path in a weighted graph (which is our case in this project) by using a queue as well but focuses/replaces the current path with the shortest path found while searching. 
3. Greedy Best first search - A greedy algorithm (an algorithm that always tries to find the best solution despite there being an optimal solution), that uses the heuristic (educated guess) and priority queue. Nodes with the closest distance to the goal will be prioritized first. So we use a priority queue and navigate through the queue, we place the cheaper node cost to the front, repeat this until all the neighboring nodes are visted and until we reach the goal. 
4. A* algorithm - is very similar to the Dijsktra algorithm. It uses the f(n) = g(n) + h(n) formula, g(n) is the distance from the start and the h(n) is the estimated distance to the goal. So the priority node in the queue is the best fscore that is calculating the distance from the start to the distance to the goal. The A* algorithm is currently the industry standard for pathfinding in video games. 

Also note that in this project, Unity allows the user to place in 2D psd images that splits those image pixels into their respective colored coded tiles into the scene. This also gives the ability to use terrain data, so that certain search algorithms will need to focus on the easier path instead of just the shortest path. 
