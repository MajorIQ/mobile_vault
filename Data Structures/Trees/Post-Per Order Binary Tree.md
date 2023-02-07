
```python
def visit(self, node):
	print(node.value)



def preorder(self, current):
	self.visit(current)
	self.preorder(current.left)
	self.preorder(current.right)


def inorder(self, current):
	self.inorder(current.left)
	self.visit(current)
	self.ineorder(current.right)


def postorder(self, current):
	self.postorder(current.left)
	self.postorder(current.right)
	self.visit(current)
```
