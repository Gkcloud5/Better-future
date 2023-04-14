#Advanced #Generators

#### Source: [Generators](https://www.learnpython.org/en/Generators)

**Generators are very easy to implement but a bit difficult to understand

**Generators are simple functions which return an iterable set of items, one at a time, in a special way.

##### iterable: 
__ iter_()
 To access a object and print it
```
a  = "apple" 
for i in a:
  print(i)
```

##### iterator:
 It help to move next next object in list or string while applying condition.

##### Iteration:
```
iterable + iterator
```

##### Generators example:
```
import random

def lottery()
    for i in range(6):
        yield random.randint(1,40)

     yield random.randint(1,15)
```