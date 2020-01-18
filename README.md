# Python--nested_json-to-normalized_csv
A python script that converts nested json to normalized csv

### Description ###
The script helps convert nested json to a csv file -

* Normalizes the json
* Checks if a csv already exists
  * If not creates a new csv file
  * If yes, appends the new json data to existing csv columns without copying the header row again
  
  
##### Example: #####

Input: 
```
{
  "name":"John",
  "age":30,
  "cars": {
    "car1":"Ford",
    "car2":"BMW",
    "car3":"Fiat"
  }
}
```

Output:

| name | age  | cars.car1  | cars.car2  | cars.car3  |
| :---: | :-: | :-: | :-: | :-: |
| John | 30 | Ford |BMW|Fiat

