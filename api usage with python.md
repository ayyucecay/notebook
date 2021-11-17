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
data2 = json.loads(json_string2)   -----> this use to be deserialize that json format 
```
# Python API
- If use the data from API, then make the request. 
- If use request then download request library:
```html
pip install requests
```
- Then, where use to request, should import request
```html
import requests
```
- Data from the endpoint is retrieved with the following method
```html
response = requests.get("https://api.open-notify.org/this-api-doesnt-exist")
```
- See the status of the response with the following method 
```html
response.status_code
```











