# objVertexColors
Three.js obj loader with vertex color support


See example usage at 
https://biizii.com/objVertexColors.html

Note that at this time, the objVertexColors.js only supports the meshlab obj export option for 'color',
deselect the 'normal' option when exporting a new obj from meshlab.


To use,
Reference the js in your html after where you referenced three.js
```html
<script src="OBJVertexColorLoader.js" type="text/javascript"></script>
```

Then, very similar to how you would normally load a standard obj, but 
```javascript
var loader = new THREE.OBJVertexColorLoader(manager);
loader.load('example.obj', function (object) {
  scene.add(object);
}, onProgress, onError);

```

Sean

