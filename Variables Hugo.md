# Variables in Hugo
## Few Example of Variable
```
{{ .Titel }} fetches the title of PAGE
{{ .Date }}
{{ .URL }}
```

## creating variable inside a markdown file
```
---
myVar: "myValue"
---
```
To access this variable from inside a markdown file
``` 
{{ .Params.myVar }}
```

## creating a custom variable in html file and using it
```html
{{ $myVarName := "string or numeric or boolean"}} you are defining the variable here
{{ $myVarName = "updated string"}} you are updating the variable here
{{ $myVarName }} <!--accessing the above variable-->
```

Example 1 of using variable
```
{{ $color := "red" }}
<h1 style="color: {{ $color }};">Change my color</h1>
```
