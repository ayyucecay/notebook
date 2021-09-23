# JSON NOTES
- JavaScript has a built in function for converting JSON strings into JavaScript objects:

    JSON.parse()

- JavaScript also has a built in function for converting an object into a JSON string:

    JSON.stringify()
    
__JSON Syntax Rules__

SON syntax is derived from JavaScript object notation syntax:

- Data is in name/value pairs
- Data is separated by commas
- Curly braces hold objects
- Square brackets hold arrays

JSON, keys must be strings

{"name":"John"}<br>
{"age":30}<br>
{"employee":{"name":"John", "age":30, "city":"New York"}}<br>
{"employees":["John", "Anna", "Peter"]}

The file type for JSON files is ".json"

## JSON.parse()
When receiving data from a web server, the data is always a string.

Parse the data with JSON.parse(), and the data becomes a JavaScript object.

__You should avoid using functions in JSON, the functions will lose their scope, and you would have to use eval() to convert them back into functions.__
```html
const text = '{"name":"John", "age":"function () {return 30;}", "city":"New York"}';
const obj = JSON.parse(text);
obj.age = eval("(" + obj.age + ")");
```
## JSON.stringify()
When sending data to a web server, the data has to be a string.

Convert a JavaScript object into a string with JSON.stringify().
```html
const obj = {name: "John", age: 30, city: "New York"};
const myJSON = JSON.stringify(obj);
```

















