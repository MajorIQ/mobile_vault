dictionary = generic way to map keys to values
hash table  = implementation of a dictionary using a hash function

Key = Against which we store the value
Value = The value we need to store against a key 

Hashing function = Takes the input and gives back the hash code/ index in array

handle collisions = gives same key for different value

Handling collisions
- Separate chaining 
- Open addressing

Separate chaining 
- Creates an array or an linked list that stores the values

Time Complexity
average = o(1)


![[direct-acess tables.png]]
insert/ delete/ search O(1)

Hash tables


![[hash tables.png]]

chaining 
![[chaining.png]]

Goals: 
- maximize randomness
- produces the least amount of collisions
Example:
- division 
- multiplication
- universal hashing
- dynamic perfect hashing
- static perfect hashing 