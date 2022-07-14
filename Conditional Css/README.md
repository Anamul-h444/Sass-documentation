# Applying CSS by Condition
1. CSS apply by condition.
2. In this system us @ as @if, @else if & @else. 
3. Write $ as $value.   
4. Code block has been executed which condition is matchd.  

#### Example
```css
@mixin font-size($value) {
    @if $value==small{
        font-size: 16px;
        font-weight: 400;
    }@else if $value==medium{
        font-size: 18px;
        font-weight: 500;
    }@else if $value==large{
        font-size:20px;
        font-weight: 600;
    }@else{
        font-size: 17px;
    }
};

h1{
    @include font-size(large)
};

h3{
    @include font-size(medium)
};

p{
    @include font-size(small)
}
```