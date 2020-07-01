**VARIABLES**

```css
@width: 10px;
@height: @width + 10px;

#header {
  width: @width;
  height: @height;
}
```



**MIXINS**

```css
.bordered {
    border-top: dotted 1px black;
    border-bottom: solid 2px black;
}

#menu a {
    color: #111;
    .bordered();
  }
  
  .post a {
    color: red;
    .bordered();
}
```


**NESTING**

```css
#header {
  color: black;
}
#header .navigation {
  font-size: 12px;
}
#header .logo {
  width: 300px;
}

#header {
  color: black;
  .navigation {
    font-size: 12px;
  }
  .logo {
    width: 300px;
  }
}
```