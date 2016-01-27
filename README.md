# Stylus position mixin
A Bourbon like mixin for the position property.

### Dependencies
  * [stylus](https://github.com/LearnBoost/stylus)

Example:
```stylus
.Div__0
  pos(relative)

.Div__1
  pos(relative auto)

.Div__2
  pos(relative 10px auto)

.Div__3
  pos(relative null 10px null 10px)
  
.Div__5
  pos(relative 10px 10px 10px 10px)
  
.Div__6
  pos(absolute 0 0 0 0)

.Div__7
  pos(fixed 0 0 null 0)
```

Will output:
```css
.Div__0 {
  position: relative;
}
.Div__1 {
  margin: 0 auto;
  position: relative;
}
.Div__2 {
  margin: 10px auto;
  position: relative;
}
.Div__3 {
  margin-right: 10px;
  margin-left: 10px;
  position: relative;
}
.Div__5 {
  margin: 10px;
  margin-top: 10px;
  margin-right: 10px;
  margin-bottom: 10px;
  margin-left: 10px;
  position: relative;
}
.Div__6 {
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  position: absolute;
}
.Div__7 {
  top: 0;
  right: 0;
  left: 0;
  position: fixed;
}
```

## Credits

Developed by [Alexis Gaillard](https://alexisgaillard.com/). Licensed under [MIT](http://opensource.org/licenses/mit-license.php).
