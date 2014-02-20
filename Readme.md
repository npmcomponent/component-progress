*This repository is a mirror of the [component](http://component.io) module [component/progress](http://github.com/component/progress). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-progress`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# Progress

  Circular progress indicator using canvas.

  ![js progress indicator component](http://f.cl.ly/items/1i0B0D1i1D1Y1e1M1S08/Screen%20Shot%202012-08-10%20at%2011.48.22%20AM.png)

## Installation

```
$ npm install progress-component
```

## Example

```js
var Progress = require('progress');

var progress = new Progress;
document.body.appendChild(progress.el);

var n = 0;
var id = setInterval(function(){
  if (n == 100) clearInterval(id);
  progress.update(n++);
}, 50);
```

## API
  
### Progress#update(n)

  Update the indicator to `n` and re-draw.

### Progress#font(family)

  Change the font to `family`.

### Progress#fontSize(n)

  Change the font size to `n`.

### Progress#size(n)

  Change the indicator diameter to `n`, defaults to 50.

## License

  MIT