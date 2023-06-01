#### Exercise:
**Print the value of key 'history' from the below dict**
```
sampleDict = {
    "class": {
        "student": {
            "name": "Mike",
            "marks": {
                "physics": 70,
                "history": 80
            }
        }
    }
}
```

#### Sample output:

![[Pasted image 20230423140702.png]]

#### Logic think:
* In above exercise `history` is under a 
	* sampleDict --> class --> student --> marks --> history
*  So we need to call from beginning of Dictionary

#### Program:

```
sampleDict = {
    "class": {
        "student": {
            "name": "Mike",
            "marks": {
                "physics": 70,
                "history": 80
            }
        }
    }
}

print(sampleDict['class']['student']['marks']['history'])
```

#### Output:

![[Pasted image 20230423141141.png]]

