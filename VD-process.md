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

# Sketching and iterating the design space. 

~~~
section = content.newSection()
box = section.newMain()
~~~

## Sketching the design space

## Exploding dimensions

## Keep it small, test modular, hide unused axes

## MutatorMath vs. Fonttools interpolation

## Managing inflections points

## Instances

## Features

## Spacing, groups and kerning

## Scripting production

## Do’s and don’ts