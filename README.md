# Stylus position mixin
A Bourbon like mixin for the position property.

### Dependencies
  * [stylus](https://github.com/LearnBoost/stylus)

Example:
```stylus
@import "position"

.Div__one
  pos(relative, null, auto, null, auto)

.Div__two
  pos(relative, 0, 10px, 100px, 10px)

.Div__three
  pos(absolute, 10px, 10px, 10px, 10px)

.Div__four
  pos(static, 0, 0, null, 0)
```

Will output:
```css
.Div__one {
  margin-right: auto;
  margin-left: auto;
  position: relative;
}
.Div__two {
  margin: 0 10px 100px 10px;
  position: relative;
}
.Div__three {
  top: 10px;
  right: 10px;
  bottom: 10px;
  left: 10px;
  position: absolute;
}
.Div__four {
  top: 0;
  right: 0;
  left: 0;
  position: static;
}
```

## Credits

Developed by [Alexis Gaillard](https://alexisgaillard.com/). Licensed under [MIT](http://opensource.org/licenses/mit-license.php).
