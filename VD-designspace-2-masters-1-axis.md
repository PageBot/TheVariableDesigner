~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '2 masters 1 axis'
page.url = 'Design space/2-masters-1-axis.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: 2 masters, 1 axis

~~~
box = content.newIntroduction()
~~~

# Single axis with 2 masters. One of them must be origin. The other is **min** or **max**.

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Single weight **[wght]** axis interpolating Regular to Bold 

### Single weight **[wght]** axis interpolating Light to Regular

### Single width **[wght]** axis interpolating Regular to Condensed

### Single optical size **[opsz]** axis interpolating Regular-Display to Regular-Text


~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/2-master-1-axis.designspace'
path = 'code/2-masters-1-axis.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~

