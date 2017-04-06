# toh-aot-universal-ng4
The Angular Tour of Heroes using ng4 with AOT and Universal

To Build AOT version

```sh
$ npm run build:aot
```

To build Universal version

```sh
$ npm run build:uni
```

To serve AOT version
```sh
$ run npm serve:aot
```

To serve Universal version 
```sh
$ run npm serve:uni
```

By Default the build.js is disabled in the index-aot.html file to see only the SSR running

```javascript
<script src="dist/build.js"></script>

<!--<script src="dist/build.js"></script>-->
```
This will no longer run the CSR/AOT version, all you will see is pure SSR


Now you can see the limitations of the Universal app. Navigation using routerLink works correctly: you can go from the Dashboard to the Heroes page and back, and you can click on a hero on the Dashboard page to display the Details page. But you cannot go to the Details from the Heroes page, because that uses a click event rather than a router link. The Hero Search on the Dashboard page does not work, nor does saving changes.
