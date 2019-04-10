~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '5 masters 2 axis'
page.url = 'Design space/5-masters-2-axis.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: 5 masters, 2 axes

~~~
box = content.newIntroduction()
~~~

# Two axes. Regular as origin, **min** and **max** masters at the ends of both axes. The influence of axes must be independent.

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Weight **[wght]** axis with 3 masters in combination with a grade [GRAD] axis, all with **min** and **max**.

### Width **[wdth]** axis with 3 masters in combination with a grade [GRAD] axis, all with **min** and **max**.

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/2-master-1-axis.designspace'
path = 'code/5-masters-2-axes.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~