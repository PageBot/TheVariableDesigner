~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '9 masters 2 axis'
page.url = 'Design space/9-masters-2-axis.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: 9 masters, 2 axes

~~~
box = content.newIntroduction()
~~~

# 2 axes with full set of masters

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Weight **[wght]** axis and Width **[wdth]** axis by a full set of 9 masters. 

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/9-master-2-axis.designspace'
path = 'code/9-masters-2-axes.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~