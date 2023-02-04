```ad-note
used to find the shortest path form a starting vertex/node to another vertex/node. 
```
## Intuition behind BFS 

![[BFS grpah image 1.png]]
- visits each vertex distance 1, then increments to 2; so forth until end of graph has been reached or vertex/node has been found.

Shortest path 0 -> 7: 0 1 3 5 7 

## BFS Implementation 

```python
marked = [False] * G.size()
def bfs(G,v):
	queue = [v]
	while len(queue) > 0:
		v = queue.pop(0)
		if not marked[v]:
			visit(v)
			marked[v] = True 
			for w in G.neighbors(v):
				if not marked[w]:
					queue.append(w)
```


## BFS Problem 

### Flood Fill Problem


![[Flood Fill Problem .png]]

```python
def floodFill(img, row, col, p):
	start = img[row][col]
	queue = [(row, col)]
	visited = set()
	while len(queue) > 0:
		row, col = queue.pop(0)
		visited.add((row, col))
		img[row][col] = p
		for row, col in neighbours(img, row, col, start):
			 if (row, col) not in visited:
				 queue.append((row, col))
	return img

def neighbours(img, row, col, start):
	indicees = [(row, -1, col), (row + 1, col), (row, col - 1), (row, col + 1)]
	return [(row, col) for row, col in indices if isValid(img, row, col) and img[row][col] == start]

def isValid(img, row, col):
	return row > 0 and col col > 0 and row < len(img) and col < len(img[0])
```
