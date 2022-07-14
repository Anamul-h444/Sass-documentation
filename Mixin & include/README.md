# Mixin and include documentation
1. You create a code block by @mixin and access any codey by @include.    
2. @mixin same as function.  
3. In @include function call by name.  
4. In mixin value pass direct or parameter.  

#### Without parameter @mixin & @include
```css
@mixin style1(){
    background-color: aqua;
    font-size: 18px;
    font-weight: 600;
};

h1{
    @include style1();
}
```

#### With parameter @mixin & @include
```css
@mixin style2($color, $size, $weight){
    background-color:$color;
    font-size: $size;
    font-weight: $weight;
};

p{
    @include style2(blue,16px ,500 )
}
```