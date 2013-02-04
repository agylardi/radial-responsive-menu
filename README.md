Radial Responsive Menu - RRM (Alpha 1.0)
======================

jQury plugin menu as alternative solution of navigation menu system for responsive website.
Inspired and based on Path apps, and research on Radial Menu by Krystian Samp (http://krystiansamp.com).
The menu system is customizable with some options. Built using jQuery version 1.8.3 and CSS 3

## Author
Agyl Rahmadi / Gyl (agyl.ardi@gmail.com)<br />
**Notes**: *This is my first attemp to make a JQuery plugin. Any feedback will be much appreciated*

## Usage 
Download the package and link the JS file (jquery .js file and this plugin file: `jquery.radialresponsivemenu.js`) and 
CSS file (`radial-responsive-menu.css`) in your HTML.
Also put *images* folder at the same directory with your HTML file.

There are 3 menu levels available in the menu (class): `level-1`, `level-2`, `level-3`.
The usage in basic HTML structure is as shown below: 
```html
<nav id="radial-menu">
  <input type="button" id="toggle-radial" value="" >
  <ul class="level-1">
    <li><a href="#">Menu Item #1</a></li>
		<li><a href="#">Menu Item #2</a></li>
		<li><a href="#">Menu Item #3</a></li>
		<li><a href="#">Menu Item #4</a></li>
		<li><a href="#">Menu Item #5</a>
			 <ul class="level-2">
				<li><a href="#">Sub-Menu Item #5.1</a></li>
				<li><a href="#">Sub-Menu Item #5.2</a></li>
				<li><a href="#">Sub-Menu Item #5.3</a>
					<ul class="level-3">
						<li><a href="#">Sub-Menu Item #5.3.1</a></li>
						<li><a href="#">Sub-Menu Item #5.3.2</a></li>
						<li><a href="#">Sub-Menu Item #5.3.3</a></li>
						<li><a href="#">Sub-Menu Item #5.3.4</a></li>
						<li><a href="#">Sub-Menu Item #5.3.5</a></li>
						<li><a href="#">Sub-Menu Item #5.3.6</a></li>
						<li><a href="#">Sub-Menu Item #5.3.7</a></li>
						<li><a href="#">Sub-Menu Item #5.3.8</a></li>
					</ul>
				</li>
				<li><a href="#">Sub-Menu Item #5.4</a></li>
				<li><a href="#">Sub-Menu Item #5.5</a></li>
				<li><a href="#">Sub-Menu Item #5.6</a></li>
				<li><a href="#">Sub-Menu Item #5.7</a></li>
				<li><a href="#">Sub-Menu Item #5.8</a></li>
			 </ul>
		</li>
		<li><a href="#">Menu Item #6</a></li>
		<li><a href="#">Menu Item #7</a></li>
		<li><a href="#">Menu Item #8</a></li>						
	</ul>
</nav>
```
For initiation of the plugin, just include the following script tag in your HTML:
```html
<script type="text/javascript">
  $(document).ready(function(){
		$('#radial-menu').radialResponsiveMenu();
	});	
</script>
```

## Options
There are 9 options for this plugin. They are as the following:

### circleRadius
`circleRadius` is the size of menu items (circle radius) in pixel.
<br />*Default value*: `60`

----

### lv1_outerRing, lv2_outerRing & lv3_outerRing
There are 2 *rings* which contains menu items in each menu levels: **Inner Ring** and **Outer Ring**.
`lv1_outerRing`, `lv2_outerRing` & `lv3_outerRing` are options for disabling (false) or enabling (true) Outer Ring.
If disabled then the menu level will only have 1 ring to be shown.
<br />*Default value for those options*: `true`

----

### innerRing_items
`innerRing_items` is the amount of menu items in **Inner Ring** on each menu level.
<br />*Default value*: `3`

----

### outerRing_items
`outerRing_items` is the amount of menu items in **Outer Ring** on each menu level.
<br />*Default value*: `5`

----

### innerRing_radius
`innerRing_radius` is the radius (in pixel) of **Inner Ring** from toggle object on each menu level.
<br />*Default value*: `85`

----

### outerRing_radius
`outerRing_radius` is the radius (in pixel) of **Outer Ring** from toggle object on each menu level.
<br />*Default value*: `170`

----

### togglePosition
`togglePosition` is the position of toggle button on screen. As the menu is targeted to be used in mobile screen, there
are 4 value for this options: `top-left`, `top-right`, `bottom-right` and `bottom-left`.
This option determine the appearance direction of menu items.
<br />*Default value*: `top-left`

