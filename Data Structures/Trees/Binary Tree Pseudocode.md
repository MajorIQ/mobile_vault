Node class
```python
class Node:
	def __init__(self, value):
		self.value = value
		self.left = None
		self.right = None
```

```python
class BST:
	def __init__(self):
		self.root = None

	def add(self, current, value):
		if self.root == None:
			self.root = Node(value)
		else:
			if value < current.value:
				if current.left == None:
					current.left = Node(value)
				else:
					self.add(current.left, value)
			else:
				if current.right == None:
					current.right = Node(value)
				else:
					self.add(current.right, value)
				
```


```python


class Node:
	def __init__(self, value):
		self.value = value
		self.left = None
		self.right = None


class BST:
	def __init__(self):
		self.root = None

	def add(self, current, value):
		if self.root == None:
			self.root = Node(value)
		else:
			if value < current.value:
				if current.left == None:
					current.left = Node(value)
				else:
					self.add(current.left, value)
			else:
				if current.right == None:
					current.right = Node(value)
				else:
					self.add(current.right, value)
```
Time complexity: log<sub>2</sub>(n)



