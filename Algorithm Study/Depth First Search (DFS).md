
## Graph Traversal
- algorithm to visit every vertex of a graph 

## Intuition behind DFS

- traverses node, by going through unexplored nodes, and returning to that node to see future unexplored nodes

```ad-note
title: Definition
Continuing to explore new vertices as we see them until we hit a dead end is depth first search 
```


## DFS Implementation 

### Recursive Implementation

- Cleaner and easier to read

```python
def dfs(G,v):
	visit(v)
	for w in G.neighbours(v):
		dfs(G,w)
```

Limitation: 
- seen/checked neighbours aren't removed resulting in checked nodes being re-checked and thus creating a infinite loop.
Fix: 
- mark nodes which have been checked/seen 

Fixed code:

```python
marked = [False] * G.size()
def dfs(G,v):
	visit(v)
	marked[v] = True
	for w in G.neighbours(v):
		if not marked[w]:
			dfs(G,w)
```

### Iterative Implementation 

- More generalizable 

```python
marked = [Flase] * G.size()
def dfs_iter(G,v):
	stack = [v]
	while stack len(stack) > 0:
		v = stack.pop()
		if not marked[v]:
			visit(v)
			marked[v] = True
			for w in G.neighbours(v):
				if not marked[w]:
					stack.append(w)
```

Run Time/ Time Complexity: O(V + E)

#### Pre-order vs post-order

![[DFS graph image.png]]

Pre-order:  0 1 2 3 5 6 7 8 9 4
Post-order: 2 6 9 8 7 5 3 4 1 0 

Pre-order, order in search 
post-order, order in dead-ends

Pre-order code:
```python
marked = [False] * G.size()
def dfs_pre(G,v):
	visit(v)
	marked[v] = True
	for w in G.neighbours(v):
		if not marked[w]:
			dfs(G,w)
```

Post-order code:
```python
marked = [False] * G.size()
def dfs_post(G,v):
	marked[v] = True
	for w in G.neighbours(v):
		if not marked[w]:
			dfs(G,w)
	vist()v
```
## DFS Application
- Cycle Detection
- Finding Connected Components
- Topological Sort 
- Maze Generation

https://www.youtube.com/watch?v=PMMc4VsIacU