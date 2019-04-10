~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '8 masters 3 axis (MM)'
page.url = 'Design space/8-masters-3-axis-mm.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: 8 masters, 3 axes

~~~
box = content.newIntroduction()
~~~

# Three axes, traditional “Multiple Master” cube. No origin in the middle, so pick one. **min** and **max** masters corners of the cube. 

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Weight **[wght]** axis with 2 masters in combination with a width **[wdth]** axis with 2 masters and all doubled for optical size **[opsz]**.

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/8-master-3-axes.designspace'
path = 'code/8-masters-3-axes.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~