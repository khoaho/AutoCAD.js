AutoCAD.js
==========

Develop Autodesk AutoCAD in JavaScript, with different APIs from Autodesk.

AutoCAD.js should come with .NETScript for AutoCAD which is downloaded at www.NetOnApp.com


**JavaScript APIs of AutoCAD.js:**

Select all layers in the current AutoCAD database:

    var layers = db("layer");

Select all lines:

    var lines = db("line");

Select all circles with specified radius:

    var circles = db("circle[radius=10]");

Update layer name of all blocks:

    db("block").update("layer", "0");
