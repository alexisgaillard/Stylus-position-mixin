# Stylus position mixin
A Bourbon like mixin for the position property.

### Dependencies
  * [stylus](https://github.com/LearnBoost/stylus)

Example:
```stylus
.Div__0
  pos(relative)

.Div__1
  pos(relative null auto null auto)
  
.Div__2
  pos(relative 10px 10px 10px 10px)
  
.Div__3
  pos(absolute 0 0 0 0)

.Div__4
  pos(fixed 0 0 null 0)
```

Will output:
```css
.Div__0 {
  position: relative;
}
.Div__1 {
  margin-right: auto;
  margin-left: auto;
  position: relative;
}
.Div__2 {
  margin: 10px;
  position: relative;
}
.Div__3 {
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  position: absolute;
}
.Div__4 {
  top: 0;
  right: 0;
  left: 0;
  position: fixed;
}
```

## Credits

Developed by [Alexis Gaillard](https://alexisgaillard.com/). Licensed under [MIT](http://opensource.org/licenses/mit-license.php).
