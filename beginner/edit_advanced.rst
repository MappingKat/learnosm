============================
Advanced Editing
============================

Introduction
____________
In the previous chapters you have learned how to draw points, lines, and shapes in JOSM, how to open your GPS waypoints and tracks in JOSM, and how to download, edit, and upload your changes on OpenStreetMap. In this chapter, we will describe in more detail some of the features of JOSM, so that you can beyond the simple editing tools and have a better understanding of the software. Note that while this chapter is not extremely advanced, it is a step higher than the previous chapters. If you don’t feel like you fully understand the lessons leading up to this, you may wish to practice a little bit more before continuing.

A Tour of JOSM
_________________

.. image:: ../_static/josm_tour.png
   :align: center
   :width: 520px

- JOSM has many different features. The main window in JOSM you are already familiar with – this is the map window, and it is where most of the action takes place. Here you view, edit, and add to the OpenStreetMap data.
- To the right of the map window are a series of panels, which each do something different. Typically when you first install JOSM several panels are shown by default, such as Layers, Properties, and Selection. When you select a point, line, or shape in the map window, it will be shown in the Selection panel. Information about the object will be shown in the Properties panel, and the username of the author of that object will be shown in the Authors panel.
- On the left side of JOSM, there are several toolbars, which consist of many buttons. At the top of this bar are different buttons which change what you can do with your mouse. You are already familiar with the first two, the Select tool and the Draw tool. The other tools make it easier to zoom in, delete an object, draw a shape, or create a line that is parallel to another line.
- Below these tools are many more buttons. These buttons control what you see on the right side of JOSM. Using these buttons you can open and close the boxes on the right, such as properties, selection, and author.

JOSM Layers
______________

- Open your GPS file and download data from OpenStreetMap, if you haven’t already. You may notice that when you open a file, or add Walking Papers, or download from OpenStreetMap, another item is added to the Layers panel on the right side of JOSM. Your Layers panel may look something like this:

.. image:: ../_static/josm_layers.png
   :align: center
   :width: 318px

- Each item in this list represents a different source of data that you have open in your map window. In the example above, “Data Layer 2” is the OpenStreetMap data that we want to edit. “Markers” are the waypoints from the GPS, and “30 Juni 2011.gpx” is the track from the GPS. Finally, “Walking Papers” is the layer created when I added my Walking Paper into JOSM. You can add the Bing imagery layer, which shows satellite imagery, by clicking “Imagery” on the top menu of JOSM and selecting “Bing Sat.”
- To hide one of these layers, select one of them with your mouse and click the Show/Hide button that looks like this:

.. image:: ../_static/josm_hide.png
   :align: center
   :width: 38px

- You should see the layer that you selected disappear in the map window. Click Show/Hide again, and it will reappear.
- You can close a layer by selecting it and using the delete button:

.. image:: ../_static/josm_delete.png
   :align: center
   :width: 38px

- Lastly, it’s important to know that you can only edit the layer that is considered active by JOSM. If you are unable to edit the map in your map window, it’s probably because you don’t have the correct layer set as active. Most layers, such as GPS points, Walking Papers, and satellite imagery, can’t be edited. The only layers that can be edited are data from OpenStreetMap, which are usually called “Data Layer 1”.
- To make a layer active, select it in the Layers panel, and click on the Activate button:

.. image:: ../_static/josm_layer_active.png
   :align: center
   :width: 40px


Saving OSM files
___________________

- Sometimes after you download some OSM data, you may wish to save it so that you can edit it offline, and then upload it later when you have internet access again.
- To save an OSM file, make sure that it is the active layer in the the Layers panel. Click “File” on the top menu, and click “Save”. Choose a location for the file and give it a name. You can also save by clicking this button:

.. image:: ../_static/josm_save.png
   :align: center
   :width: 36px

- You can now close JOSM and your data will be saved. When you want to open the file again, simply open JOSM, go to the “File” menu, and click “Open…”

Additional Drawing Tools
___________________________

- JOSM has some additional tools to make it easier to draw lines and shapes. These tools are found in the “Tools” menu at the top of JOSM.

.. image:: ../_static/josm_tools.png
   :align: center
   :width: 110px

- In order to apply the functions in this menu, you must first select a point, line or shape in the map window. Some of the most useful functions are described here:
Split Way
  This allows you to divide a line into two separate lines. This is useful if you want to add different attributes to different   parts of a road. To use this function, select a point in the middle of the line that you want to split, Select Split Way from the    Tools menu, and your line should be split in two.
Combine Way
  This does the opposite of Split Way. To combine two lines into a single line, they must share a single point. To use this function, select both lines that you want to combine. You can select more than one object by holding the SHIFT key on your keyboard and clicking on each line. When you have selected both lines, select Combine Way from the Tools menu.
Reverse Way
  This will change the direction of the line. If your line represents a road that is one way, you may want to change its direction. In other cases, direction doesn’t matter.
Simplify Way 
  If your line has too many points in it and you’d like to make it simpler, this will remove some of the points from a line.
Align Nodes in Circle
  If you are trying to make a circular shape, draw the circle as best you can and then select this function. It will help arrange your points in a circle.
Align Nodes in Line
  This function will align a series of points into a straight line.
Orthogonalize Shape
  This function is very useful for drawing buildings. After you draw a building, this function will reshape it to have square corners.

Tags
_______

- When you draw a point, line, or shape, it is create with a location, but no information about what it is. In other words, we know where it is, but not what it is. Before now, we have been using items from the Presets menu to define what it is.
- The way OpenStreetMap knows what an object is is by using tags. A tag is like a label that you can put on something. For example, if I draw a square, it’s only a square. But then I add multiple tags to it that describe what it is:
  - this square is a building
  - the name of the building is “Menara Thamrin”
  - the building is 16 levels high
- You can add as many tags as you want to an object. Tags are saved as pairs of text, called the keys and the values. In OpenStreetMap, the tags written above would in fact be:
  - building = yes
  - name = Menara Thamrin
  - building:levels = 16
- If you select an object in JOSM, you can see all the tags that are attached to it in the Properties panel on the right.

.. image:: ../_static/josm_tags.png
   :align: center
   :width: 315px

- You can add, edit, and delete these tags from this panel. The tags are traditionally in English however, so it is often better to use the Presets menu.

Keyboard Shortcuts
_____________________

- Sometimes it can be annoying to click over and over to select different options and menus in JOSM. Luckily there are shortcut keys on the keyboard that allow you to do many common tasks. Here is a list of some of the most commonly used shortcut keys, along with what they do:
- s:  Choose the Select tool
- a:  Choose the Draw tool
- z:  Choose the Zoom tool
- \+ (plus):  Zoom In
- \- (minus):  Zoom Out
- p:  Split Way
- c:  Combine Way
- o:  Align in Circle
- l:  Align in line
- q:  Orthogonalize (make a shape square)

Summary
_______
As you can see there are many additional features that make JOSM a powerful tool for making maps. Remember that the more you practice with these tools, the better you will become at adding information to OpenStreetMap.

In the final chapter we will step away from JOSM, and look at some interesting projects that use OpenStreetMap data, and learn how you can continue learning about OSM.