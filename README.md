jquery.plist
============

jQuery Property List Plugin.

This is a, somewhat, simple jQuery plugin that provides the ability to edit
XML-based Apple Property List files, i.e. .plist. This does not work with
binary property list files.

An interface to parse and load plist data is provided as well as save the
plist data back into XML form.

Requirements:

jQuery, font-awesome (for icons).
<script src="//code.jquery.com/jquery-1.11.0.min.js"></script>
<link href="//netdna.bootstrapcdn.com/font-awesome/3.2.1/css/font-awesome.css" rel="stylesheet" type="text/css" />

You will also need to include the js and css files for the plugin:
<script type='text/javascript' src='jquery.plist.js'></script>
<link href='jquery.plist.css' rel="stylesheet" type="text/css" />

Basically, just create an empty div where you want the property list editor
to appear and then create a new property list:

$('div').emptyPropertyList();

You can also load an existing property list from the XML data with:

$('div').loadPropertyList(xml);

When you are ready to save:

var text = $('div').savePropertyList();
