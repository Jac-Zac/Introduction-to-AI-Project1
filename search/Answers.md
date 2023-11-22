# Small supplementary file

## Question 1

The exploration is exactly what I expected since the nodes get expanded in a depth wise manner. No pacman doesn't go to all the explored state it just follow the solution he found with dfs.

## Question 2

BFS finds the least cost solution assuming all cost are equal which is also what happens in the eight-puzzle problem

## Question 4

On the _OpenMaze_ word dfs doesn't find the optimal solution and actually finds a really inefficient path to the goal which leads to a miserable score of 212 on the other hand bfs does find the optimal path (with score of 456) but expands 682 nodes. Furthermore the same behavior is observed with ucs since the cost are all equal. With regard to A\* we can see that when paired with the manhattanHeuristics it achieve the same result but by expanding only 535 nodes

## Question 8

I provided an example with this layout [counter_exampleSearch.lay](layouts/counter_exampleSearch.lay).

You can test it by running those two commands:

- #### Closest Agent Search

```bash
python pacman.py -l counter_exampleSearch.lay -p ClosestDotSearchAgent -z .5
```

- #### AStart Agent

```bash
python pacman.py -l counter_exampleSearch.lay -p AStarFoodSearchAgent -z .5
```
