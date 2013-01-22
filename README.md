**SASS pie** by @zethussuen
---------------------------------------
A pure HTML/CSS implementation of pie charts using SASS/SCSS.

**USAGE**
---------------------------------------
The CSS is applied through the @mixin pie. To use the mixin, simply create a div with class "pie-container" and the html5 data-attribute of "data-slices" to denote the number of slices this pie chart has:
 
```html
<div id="pie1" class="pie-container" data-slices="5">
  <div class="pie-slice-1 hold"><div class="pie color1"></div></div>
  <div class="pie-slice-2 hold"><div class="pie color1"></div></div>
  <div class="pie-slice-3 hold"><div class="pie color2"></div></div>
  <div class="pie-slice-4 hold"><div class="pie color3"></div></div>
  <div class="pie-slice-5 hold"><div class="pie color4"></div></div>  
</div>
```
 
Then, in your css, include the mixin with the radius option, such as: 
```css
#pie1 {
  @include pie(100px);
}
```

**SUPPORT**
---------------------------------------
So far, Chrome, FF, Safari and IE9 have been tested. IE9 has a bug rendering when there's only one slice. 
Also the mixin only goes up to 10, I haven't tested more than that, but theoretically it *should* work?
