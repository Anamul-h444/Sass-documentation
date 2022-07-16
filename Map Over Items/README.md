# Map over items documentation

##### First Syntax:  
@each $PropertyName in PropertyvalueList{  
    .#{$PropertyName}-Add Any Name{  
        CssPropertyName : $PropertyName  
    }  
}  

##### Second Sytem
First Declare Variable.  
Must use ; after declare variable.  

Declare Variable:    
$varName:(  
    AnyName : value then use ,  
    AnyName:....  
)

syntax:    
@each $key @PropertyName in $varName{  
   .#{$PropertyName}-Add Any Name{  
        CssPropertyName : $PropertyName  
    }   
}  





#### Exmample:
```css
###### First process
@each $color in red, blue, green {
   .#{$color}-text{
    color:$color}
}

###### Second Process
$colors:(
    color1:red,
    color2:blue,
    color3:green
);

@each $key, $color in $colors {
    .#{$color}-text{
     color:$color}
 }

 ```
 ##### Implement of Css

 ```html
    <body>
    <div class="red-text">div1</div>
    <div class="green-text">div2</div>
    <div class="div3">div3</div>
    
</body>
 ```