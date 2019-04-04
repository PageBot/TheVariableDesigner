~~~
doc.title = 'The&nbsp;Variable&nbsp;Designer'

# Page (Home)
#	Wrapper
#		Header 
#			Logo (+BurgerButton)
#			Navigation/TopMenu/MenuItem(s)
#      Content
#  			Banner
#  			SlideShow (on Home)
#      		Slides
#      		SlideSide
#			Section(s)
#				Introduction
#				Main
#				Mains
#					Main
#				Side
#				Sides
#					Side
#		Footer
#
# ----------------------------------------
# index.html
# ----------------------------------------
page.name = 'Home'
page.url = 'index.html'
content = page.select('Content')
box = content.newBanner()
~~~

# The Variable Designer

~~~
box = content.newIntroduction()
~~~

# Cases, best practices, opinions and optical sizes.

~~~
section = content.newSection()
box = section.newMain()
~~~

# Design paths for Variable Fonts

* “Simple” 2-masters-1-axis
* “Simple” 3-masters-1-axis
* 4-masters-2-axes
* 5-masters-2-axes
* 9-masters-2-axes
* Arbitrary set of existing master files
* Super-in-position
* Parametric axes
* Catalog axes
* Axis by hierarchy
* Supporting masters
* Indendent axes
* Delta-absorbers
* In-axis masters

# Instances

# Features

# Spacing, groups and kerning

# Scripting production

# Do’s and dont’s


