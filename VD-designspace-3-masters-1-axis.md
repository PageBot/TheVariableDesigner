~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '3 masters 1 axis'
page.url = 'Design space/3-masters-1-axis.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: 3 masters, 1 axis

~~~
box = content.newIntroduction()
~~~

# Single axis. Regular as origin, **min** and **max** masters on the sides.

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Single width **[wdth]** axis with 3 masters

### Single weight **[wght]** axis with 3 masters

### Single grade **[GRAD]** axis with 3 masters

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/3-master-1-axis.designspace'
path = 'code/3-masters-1-axis.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~

