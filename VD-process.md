~~~
# ----------------------------------------
# process.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = 'Process'
page.url = 'process.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Variable design strategy: The Process

~~~
box = content.newIntroduction()
~~~

# Skateboard. RoboFont. Fonttools. Scripts. Code.

~~~
section = content.newSection()
box = section.newMain()
~~~

# Skateboard
