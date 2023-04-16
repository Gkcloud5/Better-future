#Advanced #Serialization

#### Source:
[Serialization](https://www.learnpython.org/en/Serialization)
[youtube](https://www.youtube.com/watch?v=hkYz-WJjf4U)

**usually image is a file for computer read it easily, pickle method used to add a content to that file.**

**Pickle only works on list or sequence of character**


```
import pickle

cars=["audi", "benz", "BMW"]
file="mycars.pkl"

fileobject=open(file, "wb") //wb-->write binary

pickle.dump(cars, fileobject) //dump helps to add a content in file
fileobject.close()
```