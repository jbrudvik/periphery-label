[![Build status](https://img.shields.io/travis/jbrudvik/periphery-label.svg)](https://travis-ci.org/jbrudvik/periphery-label)
[![Bower version](http://img.shields.io/bower/v/periphery-label.svg)](https://github.com/jbrudvik/periphery-label)

  - [PeripheryLabel()](#peripherylabelidstring)
  - [PeripheryLabel.setToWindowTop()](#peripherylabelsettowindowtop)
  - [PeripheryLabel.insertSortedByAttr()](#peripherylabelinsertsortedbyattrelementelementcontainerelementattrstring)
  - [PeripheryLabel.show()](#peripherylabelshowmessagestring)
  - [PeripheryLabel.hide()](#peripherylabelhide)

## PeripheryLabel(id:String)

  A label that displays a message on the periphery.
  
  If multiple periphery labels exist, they will be grouped together.
  
  May be shown and hidden.
  
  Parameters:
  
  - id (string): Used for determining content order (required for consistent ordering)

## PeripheryLabel.setToWindowTop()

  Ensure the label is located at top of window.
  
  Fixed CSS positioning does not always hold, so force the correct absolute
  position if necessary.

## PeripheryLabel.insertSortedByAttr(element:Element, container:Element, attr:String)

  Inserts an element underneath a container element in position maintains
  sorted order of child elements by given attr.
  
  Assumptions:
  
  - Existing children of container are sorted by attr
  
  Parameters:
  
  - element: The element to be inserted (required)
  - container: The element under which element will be inserted (required)
  - attr (String): The attribute by which child elements are sorted (default: id)

## PeripheryLabel.show(message:String)

  Display message in label.
  
  If message is falsy, label will be hidden.
  
  Parameters:
  
  - message (String): The message to be displayed (required)

## PeripheryLabel.hide()

  Hide label

# Development

## Generating documentation

    $ npm install -g dox
    $ ./generate-docs > README.md

## Deployment

Where X.Y.Z is the new version number:

    $ git tag -a vX.Y.Z
    $ git push --tags
