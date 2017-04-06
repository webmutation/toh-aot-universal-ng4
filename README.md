# toh-aot-universal-ng4
The Angular Tour of Heroes using ng4 with AOT and Universal

To Build AOT version
npm run build:aot

To build Universal version
run npm build:uni

To serve AOT version
run npm serve:aot

To serve Universal version 
run npm serve:uni

Disable the build.js in the index-aot.html file to see only the SSR 

Now you can see the limitations of the Universal app. Navigation using routerLink works correctly: you can go from the Dashboard to the Heroes page and back, and you can click on a hero on the Dashboard page to display the Details page. But you cannot go to the Details from the Heroes page, because that uses a click event rather than a router link. The Hero Search on the Dashboard page does not work, nor does saving changes.
