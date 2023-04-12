#Basics #modules #packages

#### Source: [module](https://www.learnpython.org/en/Modules_and_Packages)

**Module is a piece of software that has a specific functionality.

##### Writing module:
* Module can have a set of functions, classes or variables defined and implemented.

```
##game.py
import draw

def play_game():
    ...

def main():
    result = play_game()
    draw.draw_game(result)

if __name__ == '__main__'
     main()
```


```
###draw.py
def draw_game():
    ...

def clear_screen(screen):
    ...
```

