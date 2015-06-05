# EasyGrid
An intuitive, flexible CSS grid with minimal footprint

## Usage
This grid system requires a parent element with the class `grid` applied to it. It will then treat all children as grid items (no asterisk selector used).  
The grid will have as many columns as it has child elements, but you can override the columns (think of the `colspan` attribute). Media queries are in place to resize the rows for smaller screens, but you should expand these based on your use case.  
Demo is available on [JSFiddle](http://jsfiddle.net/0ocxpxte/)

To use *EasyGrid* in your project, include it in your HTML:  

    <link href="assets/css/grid.css" rel="stylesheet" type="text/css" />

<br />

## Examples

Example base grid markup:
```html
    <div class="grid">
      <div>1/2</div>
      <aside>1/2</aside>
    </div>
```  
<br />

Example using override classes:
```html
    <div class="grid">
      <div class="1-3">1/3</div>
      <div class="2-3">2/3</div>
    </div>
```
<br />
  
Example with a form (oh yes):
```
    <form class="grid" method="get" action="">
      <input type="text" name="name" placeholder="1/3" />
      <input type="email" name="email" placeholder="1/3" />
      <input type="submit" placeholder="1/3" />
    </form>
```
