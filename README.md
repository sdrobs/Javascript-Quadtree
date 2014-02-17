Javascript-Quadtree
===================

A js quad tree designed for nearest neighbor point search in fastest possible runtime.

To use:

```
<script src="./quadtree.js"></script>
```
```
var points = [[1,2],[3,8],[4,2],[0,3],[1,1],[6,7]] //points in form [[x,y],[x1,y1],...]
var qtree = new quadtree(points,0,0,10,10) //10 is just the size in x and y of your plot

console.log(qtree.tree) //view the tree if you want
```
```
var nearest = qtree.findNearestPoint([1,2]) //find the point nearest to any given point
console.log(nearest) //will yield [1,1] (does not count itself as nearest)
```


###License

MIT
