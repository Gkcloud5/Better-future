---
creation date: 2023-06-23 14:11
modification date: Friday 23rd June 2023 14:11:20
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/chap_08.html)

--------------------------------------

#### Explanation about it:

##### Interactive or not?

* Some scripts run without any interaction from the user at all.
	* Script runs in a predictable way every time.
	* Script can run in the background.
* Some scripts required user input
	* More flexible scripts can be built
	* Users can customize the script as it runs or make it behave in different ways
	* Script can report its progress as it runs

##### Using "echo" built-in command:

```
cat feed.sh

#!/bin/bash
# This script acts upon the exit status given by penguin.sh

if [ "$#" != "2" ]; then
  echo -e "Usage of the feed script:\t$0 food-on-menu animal-name\n"
  exit 1
else

  export menu="$1"
  export animal="$2"

  echo -e "Feeding $menu to $animal...\n"

  feed="/nethome/anny/testdir/penguin.sh"

  $feed $menu $animal

result="$?"

  echo -e "Done feeding.\n"

case "$result" in

  1)
    echo -e "Guard: \"You'd better give'm a fish, less they get violent...\"\n"
    ;;
  2)
    echo -e "Guard: \"No wonder they flee our planet...\"\n"
    ;;
  3)
    echo -e "Guard: \"Buy the food that the Zoo provides at the entry, you ***\"\n"
    echo -e "Guard: \"You want to poison them, do you?\"\n"
    ;;
  *)
    echo -e "Guard: \"Don't forget the guide!\"\n"
    ;;
  esac

fi

echo "Leaving..."
echo -e "\a\a\aThanks for visiting the Zoo, hope to see you again soon!\n"
```

```
cat penguin.sh

#!/bin/bash

# This script lets you present different menus to Tux.  He will only be happy
# when given a fish.  To make it more fun, we added a couple more animals.

if [ "$menu" == "fish" ]; then
  if [ "$animal" == "penguin" ]; then
    echo -e "Hmmmmmm fish... Tux happy!\n"
  elif [ "$animal" == "dolphin" ]; then
    echo -e "\a\a\aPweetpeettreetppeterdepweet!\a\a\a\n"
  else
    echo -e "*prrrrrrrt*\n"
  fi
else
  if [ "$animal" == "penguin" ]; then
    echo -e "Tux don't like that.  Tux wants fish!\n"
    exit 1
  elif [ "$animal" == "dolphin" ]; then
    echo -e "\a\a\a\a\a\aPweepwishpeeterdepweet!\a\a\a"
    exit 2
  else
    echo -e "Will you read this sign?!  Don't feed the "$animal"s!\n"
    exit 3
  fi
fi

```


![[Pasted image 20230623151325.png]]

