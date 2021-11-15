# JSON Data in Python

- import json 
- dump() = dumps() -----> this method can write the data in files
```html
with open("data_file.json", "w") as write_file:
    json.dump(data, write_file)    -----> dumb has two argument 1: data object to be serialized 2: data bytes will be written
```
```html
json_string = json.dumps(data)     -----> serialized JSON data export the python str object 
```
```html
data2 = json.loads(json_string2)        -----> this use to be deserialize that json format 
```
