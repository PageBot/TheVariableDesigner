~~~
# ----------------------------------------
# designspace.html
# ----------------------------------------
page = page.next
page.applyTemplate(template)  
page.name = '4 masters 2 axis (MM)'
page.url = 'Design space/4-masters-2-axes-mm.html'
content = page.select('Content')
box = content.newBanner()
~~~

# Design space: 4 masters, 2 axes (MM)

~~~
box = content.newIntroduction()
~~~

# Two axes, traditional “Multiple Master” square. No origin in the middle, so pick one of the four. **min** and **max** masters corners of the square. 

~~~
section = content.newSection()
box = section.newMain()
~~~

## Usage examples

### Weight **[wght]** axis with 2 masters in combination with a width **[wdth]** axis with 2 masters and all doubled for optical size **[opsz]**.

~~~
from pagebot.elements.vf.designspacegraph import newDesignSpaceGraph
path = 'resources/fonts/typetr/8-master-3-axes.designspace'
path = 'code/4-masters-2-axes-mm.json'
box = newDesignSpaceGraph(parent=section, path=path, stroke=0, nodeStroke=1, labelSize=doc.rootStyle['labelSize'])
~~~