~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = 'Design space'
page.url = 'designspace.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Variable design strategy: Design the design space

~~~
box = content.newIntroduction()
~~~

# Design space defines the multi-dimensional interpolating area, including all possible instance of a Variable Font.

~~~
section = content.newSection()
box = section.newMain()
~~~

# Design of design spaces
