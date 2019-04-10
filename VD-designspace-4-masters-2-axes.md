~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '4 masters 2 axis'
page.url = 'Design space/4-masters-2-axes.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: 4 masters, 2 axes 

~~~
box = content.newIntroduction()
~~~

# Two axes. Regular as origin, **min** and **max** masters on both sides. One independent master on second axis.

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Weight **[wght]** axis with 3 masters in combination with a one-direction axis of independent local influence.

### Width **[wdth]** axis with 3 masters in combination with a one-direction axis of independent local influence.

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/4-master-2-axes.designspace'
path = 'code/4-masters-2-axes.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~