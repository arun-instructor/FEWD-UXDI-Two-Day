#HTML Review and Introduction to CSS

##HTML Review

#####What tag is it?
- Below is a mockup of a HTML page we will be building today.
- Think about which tags may be used to create this layout.

![Betty White Resume](starter_code/WendyBite_AboutMe.png)

##HTML `img` Tag
- Images are placed on the page by the `img` tag.
- Let's take a look at how it works:

```
<img src="img/imageName.jpg" />
```

- We will try a few examples together.

##Working with Directories
- In order to link files correctly it's important to understand how directories work.
- Let's take an example of an image called puppies.jpg that is located inside of a folder called img. Let's see how the `img` tag changes as the files get moved around.
- It's also important to note that if you move a file after you make changes to it in Sublime Text you should exit Sublime Text and re-open the file.

##Using CSS with HTML
- There are three main ways to use CSS - inline styles, the `style` tag in the `head`, and a separate .css file that is linked to the HTML.
- Linking a stylesheet to the HTML document is the best-practice way to use CSS styles.
- Here is the syntax for the `link` tag:

```
<link rel="stylesheet" href="style.css" />
```

##CSS Breakdown
- Each CSS style set starts with a selector.
- Selectors allow you to identify which elements you want to apply styles to.
- Here is an example of a selector with a couple rules:

```
p {
	color: red;
	font-weight: bold;
	background-color: blue;
}
```

- This example selects all paragraph tags on the page and applies the below styles to them.

##CSS Selectors
- There are three common basic selectors in CSS.
- The first is the element selector. This is not a very specific selector:

```
div {
	color: red;
}

table {
	color: red;
}

p {
	color: red;
}
```

- The second is the id selector. By convention id's should not be used more than once per page:

```
#my-div {
	background-color: #990000;
}
```

- The third is the class selector. Classes by convention can be used multiple times throughout the page:

```
.my-divs {
	background-color: #EBEBEB;
}
```

##CSS Colors
- Colors in CSS can be defined in a few different ways.
- The first we have already seen - calling them out by their name symantically (red, green, blue, etc.)
- The second way is by using HEX colors. HEX codes represent shades of red, green, and blue.

![HEX Colors](img/hex_colors.png)

- You can find color codes on a number of websites and other programs like Photoshop. [Colorpicker.com](http://www.colorpicker.com/) is a good example.
- Another way of defining CSS colors is via `rgba()`. Rgba accepts values for red, green, and blue as well as an alpha value for transparency.
- Each RGB value is from 0 to 255. Alpha values are from 0 to 1.

##CSS Review
- Where should CSS styles go?
- How does the CSS syntax work?
- Give examples of 3 different CSS selectors.

##About Me Code-Along
- We will now work on coding the about me page that we showed earlier.
- We will be incorporating our HTML knowledge with CSS styles to accomplish this.

##Twitter Bootstrap
- Bootstrap is a front-end framework that incorporates a grid system, UI components, JavaScript widgets and more.
- Let's take a look at the documentation: [http://getbootstrap.com](http://getbootstrap.com/).
- The framework consists of one main CSS file, an optional theme CSS file, and a main JS file.
- Bootstrap requires jQuery to work, which is a JavaScript framework.

##Using Bootstrap
- To use Bootstrap you have to include the three required files.
- Bootstrap files can be linked via the CDN provided, or downloaded locally onto the computer.
- Remember to place your reference to the jQuery library above your reference to the Boostrap JS code.

##Bootstrap Columns
- Columns are written in this format as a class attribute: col-(breakpoint)-(offset).
- An example of a three-column layout may be to use the class col-sm-4.
- All columns should be wrapped into an element with a class of row.
- So the complete three-column layout may look something like this:

```
<div class="row">
	<div class="col-sm-4">
		Content Here
	</div>
	<div class="col-sm-4">
		Content Here
	</div>
	<div class="col-sm-4">
		Content Here
	</div>
</div>
```

##Breakpoints
- The way that Bootstrap works is to dynamically reduce column size according to the window size.
- To be mobile-friendly, the columns will break into a stack layout after a minimum width is detected.
- The breakpoints you can select in your columns control at which point this happens.
- Check out their documentation [here](http://getbootstrap.com/css/#grid) to see what these breakpoints are in terms of size.

##Code-Along
- Let's see the grid system in action.
- We will be coding the Bootstrap grid example:

![Grid Example](img/grid_template.png)

- Let's also make sure to practice using different breakpoints.

##UI Elements
- Bootstrap wraps in a myriad of great UI elements that you can drop in anywhere on your site.
- With Bootstrap you can make really pretty things quickly.
- Let's look at some [examples](http://getbootstrap.com/components/).

##Putting it Together
- Let's take a look at some of the bootstrap examples located [here](http://getbootstrap.com/getting-started/#examples).
- We will code together the "Jumbotron Narrow" template located [here](http://getbootstrap.com/examples/jumbotron-narrow/).
- Before we start, let's also plan out our grid system.

##Calling Bootstrap to the Stage
- In this code-along exercise we will use a wireframe/mockup that you create to develop a layout using Bootstrap.
- Your task is to come up with a wireframe based on a redesign of an existing website that you think needs some work.
- In groups of two research a website that needs help and draw out a wireframe that makes the site look better.
- We will all take a vote and finally choose one wireframe to develop together with Bootstrap.

##Lab Time
- The last part of the class will be dedicated to letting you play with layouts in HTML and CSS for your own projects.
- I would recommend trying out some of the layouts you have created as wireframes throughout the class and see what you can develop.
- Have some fun with it! Try out some cool fonts, use Bootstrap if you like, and make something pretty.