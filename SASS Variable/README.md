# Sass Variable
Variables are a way to store information that you can re-use later.  
With Sass, you can store information in variables, like:  
-strings
-numbers
-colors
-booleans
-lists
-nulls
#### Sass Vaiable Syntax:
`$variablename: value;`

#### Example
```css
<-- Color variable-- >
$header-background :#ff0000;
$paragraph-background:#0000ff;

<--Font size variable-->
$header-font-size:18px;
$paragraph-font-size:14px;

<--Implement of variable-->
h1{
    background-color: $header-background;
    font-size: $header-font-size;
}

p{
    background-color: $paragraph-background;
    font-size: $paragraph-font-size;
}
```