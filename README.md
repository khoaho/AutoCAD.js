AutoCAD.js
==========

Develop Autodesk AutoCAD in JavaScript, with different APIs from Autodesk. AutoCAD.js makes JavaScript in AutoCAD as easy to use as possible.

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

Run AutoCAD command:

    db().runCommand("LINE");
    
Zoom extents:

    db().zoomExtents();

Register an event handler:
    db().addEvent("commandEnded", function () {
    	// Do extra work after the command is ended
    });
    
Remove an event handler:
    db().removeEvent("beginQuit");

More APIs and demos are in development...
