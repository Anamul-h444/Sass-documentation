# Inheritence with @extend 
By @extend we inheritence any code block.  

#### Process of inheritenc
1. Write @extend parentsCodeBlockName as Css.

#### Example
In below code I inheritence .btn class code in .btn-one & .btn-two
```css
.btn{
    color: #fff;
    padding: 10px 15px;
    font-size: 18px;
    font-weight: 700;
    border-radius: 8px;
};
.btn-one{
    @extend .btn;
    background-color: blue;
};

.btn-two{
    @extend .btn;
    background-color: red;  
}
```