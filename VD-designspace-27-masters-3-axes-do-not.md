~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '27 masters 3 axes (Do not)'
page.url = 'Design space/27-masters-3-axes-do-not.html'
content = page.select('Content')
box = content.newBanner()
~~~

# 27 masters, 3 axes (How not to do it)

~~~
box = content.newIntroduction()
~~~

# 3D cube, with middle Regular as origin. Masters on all corners, all middle ribs and all **min** and **max** axis endpoints.

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Don’t do this, unless you have too much time at hand.

### Or if there is a real reason and possibility to automate the generating of masters from a core set of sources.

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/27-master-3-axis.designspace'
path = 'code/27-masters-3-axes.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~