## Types

- string: Unicode characters representing some text, like "hi terraform" " "hi".
---
- number (like an `int`): a numeric value. The number type can represent both whole numbers like 15 or 54 and fractional values like 6.28.
---
- bool: Either true or false.
---
- list (`tuple`): a sequence of values, like ["us-west-1a", "us-west-1c"]. 
  - Elements in a list or tuple are identified by consecutive whole numbers (indices), starting with zero.
    - Lists are good for ordered collections of elements, like a list of server names.
      - The type in a list must be the same for all elements.
    - Tuples are good for ordered collections of elements when the number of elements is known and fixed.
      - The type in a tuple can be different for each element.
---
- map (or object): a group of values identified by named labels, like {name = "Mabel", age = 52}.
  - Maps are good for loosely related data, like a list of servers with their IP addresses.
  - Objects are good for related data, like a server with a name, IP address, and other attributes.
  
---
- set: a collection of unique elements, like {"us-west-1a", "us-west-1c"}. These are ordered by their hash value, not by their index.
  - Ordering by their hash value means that the order of elements in a set can change when you add or remove elements.
   - A set is unordered, so the order of elements in a set is not guaranteed to be the same between Terraform runs.