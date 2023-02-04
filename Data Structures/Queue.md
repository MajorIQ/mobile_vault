
FIFO Principle

**F**irst
**I**n
**F**irst
**O**ut

insert = Enqueue
delete = Dequeue

python 

collections.deque = double linked list

```java
from collections import deque 
// represented internally as a double linked list

class Queue:

	def __int__(self):
		self.data = deque()

	// append the element to the end 
	def enqueue(self, node):
		self.data.append(node)

	// use popleft to remove the element at the front of the queue
	def dequeue(self):
	self.data.popleft()
```

Time complexity: O(1) (contestant time) 

Use cases:

- Operating systems
	- CPU and disk scheduling
- Spotify
- Breadth-first search