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

#### Use of Nested CSS in Sass

##### Regular Css
```css
nav ul li{
    list-style: none;
            display: inline-block;
}
nav ul li a{
    text-decoration: none;
                color:black;
                margin: 0 15px;
                transition: all 0.4s ease;
}
nav ul li a:hover{
   background-color: black;
                color: #fff;
                padding: 4px 6px;
                border-radius: 2px; 
}
```

##### Nested Css
```css
nav{
    ul{
        li{
            list-style: none;
            display: inline-block;
            a{
                text-decoration: none;
                color:black;
                margin: 0 15px;
                transition: all 0.4s ease;
            }
            a:hover{
                background-color: black;
                color: #fff;
                padding: 4px 6px;
                border-radius: 2px;
            }
        }
    }
}
```