# weblog
storing my thoughts and bookmarks about code related content

**Thought 1 - 9 Dec 2015**

Flocking is a cool web based realtime SC inspired environment:  
http://flockingjs.org/next/demos/playground/live/#granulator

I'd like to think something like this can be done for sverchok/grasshopper/dynamo like apps.

**Thought 2 - 27 Dec 2015**

i'm tired of it all.

**Thought 3 - 28 Dec 2015**

today is no different.

**Thought 4 - 2 Jan 2016**

"The Quiet Earth" movie has cool intro music + visual. Deep swelling pads.

**Thought 5 - 6 jan 2016**

```python
import bpy

def smart_bevel():

    obj = bpy.context.active_object
    spline = obj.data.splines.active

    if spline.type in {'NURBS', 'POLY'}:
        points = obj.data.splines.active.points
        part = [True for i in points]
        points.foreach_get("select", part)
        
        if not (part.count(True) == 1):
            print('pick only one point')
            return
        else:
            print('one point selected, go go go go !')

smart_bevel()
```

**Thought 6 - 11 jan 2016**

make todo. todo made: https://github.com/zeffii/weblog/issues/3

**Thought 7 - 12 jan 2016**

inverted vertex cols

**Thought 8 - 16 jan 2016**

 more people talking about bmesh boolean op = good
 
 ........
 
 **Thought 9 - 24 jan 2016**
 
The desktop machine died two days ago, more specifically the linux HD. Lukily anything that I value is backed up and it's probably time to say goodbye to the behemoth. (Carillon AC-1 audio computer - June 2007 - Jan 2016). So now i'm looking for a low spec / low power consumption machine to keep programming with optimization in mind.

**Thought 10 - 25 jan 2016**

modified the path structure of mesh_tinyCAD. now now longer has nested dir and a head dir called ` cad tools ` or whatever. GitHub still doesn't allow full control over filenames of the releases. so I can not foce the path to be a correct python path ( ie  `-` is discouraged in favour of `_` ) 

------------------

**10 feb wed**  

http://www.gluco-wise.com/ - looks interesting, or is it just marketing hype. The statement that it requires no blood is awesome.
