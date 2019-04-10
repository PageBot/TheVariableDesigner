~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = 'Catalog axes'
page.url = 'Design space/catalog-axes.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: Catalog axes

~~~
box = content.newIntroduction()
~~~

# 2 axes with 3 neighbouring design spaces

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Weight **[wght]** axis and Width **[wdth]** axis on cascading design spaces. 

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/9-master-2-axis.designspace'
path = 'code/12-masters-2-axes-2-catalog.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~