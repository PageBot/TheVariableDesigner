~~~
# ----------------------------------------
# tools.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = 'Tools'
page.url = 'tools.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Variable design strategy: The Tools

~~~
box = content.newIntroduction()
~~~

# Skateboard. RoboFont. Fonttools. Scripts. Code.

~~~
section = content.newSection()
box = section.newMain()
~~~

# Skateboard

# RoboFont

# Fonttools

# Scripts

# Code