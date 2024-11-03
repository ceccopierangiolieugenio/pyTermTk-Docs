TTkAbstractListItem
===================

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkAbstractListItem
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkAbstractListItem.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = TTkWidget.classStyle | {
                      'default':     {'color': TTkColor.RST},
                      'highlighted': {'color': TTkColor.bg('#008855')+TTkColor.UNDERLINE},
                      'hover':       {'color': TTkColor.bg('#0088FF')},
                      'selected':    {'color': TTkColor.bg('#0055FF')},
                      'clicked':     {'color': TTkColor.fg('#FFFF00')},
                      'disabled':    {'color': TTkColor.fg('#888888')},
                  }
   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------

   .. autosummary::
   
      closed
      currentStyleChanged
      focusChanged
      sizeChanged
   

   
   :ref:`Slots <Signal and Slots>`
   -------------------------------
   

   

   
   
   
   Slots Inherited from: :py:class:`TTkWidget`

   .. autosummary::

   
      close
      hide
      lowerWidget
      raiseWidget
      setDisabled
      setEnabled
      setFocus
      setVisible
      show
      update
   
   
   
   
   

   
   Members
   -------

   
   .. autoattribute:: closed
   .. autoattribute:: currentStyleChanged
   .. autoattribute:: focusChanged
   .. autoattribute:: sizeChanged
   

   
   Methods
   -------
   

   

   
   .. automethod:: data
   .. automethod:: mousePressEvent
   .. automethod:: setData
   .. automethod:: setText
   .. automethod:: text

   

   
   
   
   Methods Inherited from: :py:class:`TTkWidget`

   .. autosummary::

   
      clearFocus
      close
      currentStyle
      disableWidgetCursor
      enableWidgetCursor
      focusInEvent
      focusOutEvent
      focusPolicy
      geometry
      getCanvas
      getPixmap
      getWidgetByName
      hasFocus
      height
      hide
      isEnabled
      isEntered
      isVisible
      isVisibleAndParent
      lowerWidget
      maxDimension
      maximumHeight
      maximumSize
      maximumWidth
      mergeStyle
      minDimension
      minimumHeight
      minimumSize
      minimumWidth
      mouseEvent
      move
      moveEvent
      name
      paintChildCanvas
      paintEvent
      parentWidget
      pasteEvent
      pos
      raiseWidget
      resize
      resizeEvent
      setCurrentStyle
      setDefaultSize
      setDisabled
      setEnabled
      setFocus
      setFocusPolicy
      setGeometry
      setMaximumHeight
      setMaximumSize
      setMaximumWidth
      setMinimumHeight
      setMinimumSize
      setMinimumWidth
      setName
      setParent
      setStyle
      setToolTip
      setVisible
      setWidgetCursor
      show
      size
      style
      toolTip
      update
      widgetItem
      width
      x
      y
   
   
   
   
   






TTkAbstractListItem Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkAbstractListItem

.. autosummary::


  classStyle
  listItemClicked

.. currentmodule::  TermTk.TTkWidgets


