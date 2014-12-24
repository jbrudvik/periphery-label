[![Bower version](http://img.shields.io/bower/v/periphery-label.svg)](https://github.com/jbrudvik/periphery-label)

  - [PeripheryLabel()](#peripherylabel)
  - [PeripheryLabel.setToWindowTop()](#peripherylabelsettowindowtop)
  - [PeripheryLabel.insertSortedByAttr()](#peripherylabelinsertsortedbyattr)
  - [PeripheryLabel.show()](#peripherylabelshow)
  - [PeripheryLabel.hide()](#peripherylabelhide)

## PeripheryLabel()

  A label that displays a message on the periphery.
  
  If multiple periphery labels exist, they will be grouped together.
  
  May be shown and hidden.
  
  Parameters:
  
  - id (string): Used for determining content order (required for consistent ordering)

## PeripheryLabel.setToWindowTop()

  Ensure the label is located at top of window.
  
  Fixed CSS positioning does not always hold, so force the correct absolute
  position if necessary.

## PeripheryLabel.insertSortedByAttr()

  Inserts an element underneath a container element in position maintains
  sorted order of child elements by given attr.
  
  Assumptions:
  
  - Existing children of container are sorted by attr
  
  Parameters:
  
  - element: The element to be inserted (required)
  - container: The element under which element will be inserted (required)
  - attr (string): The attribute by which child elements are sorted (default: id)

## PeripheryLabel.show()

  Display message in label.
  
  If message is falsy, label will be hidden.
  
  Parameters:
  
  - message (string): The message to be displayed (required)

## PeripheryLabel.hide()

  Hide label

# Generating documentation

    $ npm install -g dox
    $ ./generate-docs
