Javascript-Quadtree
===================

A js quad tree designed for nearest neighbor point search in fastest possible runtime.

####To use:

```
<script src="./quadtree.js"></script>
```

####Create a tree in one line:
```
var points = [[1,2],[3,8],[4,2],[0,3],[1,1],[6,7]] //points in form [[x,y],[x1,y1],...]
var qtree = new quadtree(points,0,0,10,10)
```
Note that 10,10 is just the size in x and y of your plot. If you don't know the plot size, just make both values slightly larger than the highest x or y coordinate from your list of points.

####View the tree if you want:
```
console.log(qtree.tree)
```

####Find the point nearest to any given point:
```
var nearest = qtree.findNearestPoint([1,2])
console.log(nearest) //will yield [1,1] (does not count itself as nearest)
```


###License

MIT
