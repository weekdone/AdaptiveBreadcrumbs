# Adaptive/Responsive Breadcumbs by [Weekdone](http://weekdone.com/)

Adaptive/Responsive Breadcumbs CSS styles with FLEX, just copy and paste to your project. 

## [Preview demo](http://htmlpreview.github.io/?https://github.com/weekdone/AdaptiveBreadcrumbs/blob/master/index.html)

[![Preview](https://dl.dropboxusercontent.com/s/eh3uo3931q5jdt4/weekdone-charts.png?dl=0&preview=weekdone-breadcrumbs.png)](http://htmlpreview.github.io/?https://github.com/weekdone/AdaptiveBreadcrumbs/blob/master/index.html)

### Features
* plug-and-play
* LESS and CSS

### How to use
1. Set up breadcrumbs in HTML
2. Copy and paste the CSS file or parse LESS
3. Enjoy adaptive breadcrumbs

Useful for: 
* web apps
* online stores
* anything 

### TL;DR — give me the code
```html
<ul class="crumbs">
  <li><a href="#">Company</a></li>
  <li><a href="#">Department</a></li>
  <li><a href="#">Team</a></li>
  <li><a href="#">User</a></li>
</ul>

```

```css
.crumbs {
  display: flex;
  margin: 1em 0;
  padding: 0;
  clear: both;
  overflow: hidden;
}
.crumbs:hover li:last-child {
  flex-shrink: 10;
}
.crumbs li {
  flex: 0 10 auto;
  min-width: 0;
  list-style: none;
  transition: all 0.2s cubic-bezier(0, 0, 0.2, 1);
}
.crumbs li:hover,
.crumbs li:last-child:hover {
  flex-shrink: 0;
}
.crumbs li a {
  display: block;
  position: relative;
  box-sizing: border-box;
  padding: 1em;
  width: 100%;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  color: #90a4ae;
}
.crumbs li a:hover {
  color: #78909c;
}
.crumbs li a:after {
  font-family: FontAwesome;
  content: "\f0da";
  position: absolute;
  right: 0;
}
.crumbs li:last-child {
  flex-shrink: 0;
}
.crumbs li:last-child a {
  color: #607d8b;
  text-decoration: none;
}
.crumbs li:last-child a:after {
  content: "";
}


```