# SCL
SCL or Smart Content Layout is a smarter way to write CSS.

## Example:
### SCL code:
``` 
.title {
  font-family: "Times New Roman", Times, serif;
  font-size: !fontSize();
}

!fontSize(){ //This is Javascript
  var x = 0;
  x += 1;
  return x + "%";
}.run = "init" <-- This means that the code will only run on page load.
```

When you run that code throo the compiler you will get a JavaScript file and a CSS file.

### CSS code:
```
.title {
  font-family: "Times New Roman", Times, serif;
}
```
### Javascript code:
```
function run(){
  var a document.getElementsByClassName("title");
  for(int b = 0; b < a.length; b++){
    a[b].style.fontSize = b();
  }
}

function b(){
  var x = 0;
  x += 1;
  return x + "%";
}

run();
```
