TTkScrollBar
============

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkScrollBar
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkScrollBar.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color': TTkColor.RST},
                      'disabled':    {'color': TTkColor.fg('#888888')},
                      'focus':       {'color': TTkColor.fg('#cccc00')},
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
   

   

   
   .. autosummary::
   
      setPageStep
      setRange
      setRangeTo
      setSingleStep
      setValue
   

   
   
   
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
   

   


   

   
   .. automethod:: color
   .. automethod:: focusColor
   .. automethod:: maximum
   .. automethod:: minimum
   .. automethod:: orientation
   .. automethod:: pageStep
   .. automethod:: setColor
   .. automethod:: setFocusColor
   .. automethod:: setMaximum
   .. automethod:: setMinimum
   .. automethod:: setPageStep
   .. automethod:: setRange
   .. automethod:: setRangeTo
   .. automethod:: setSingleStep
   .. automethod:: setValue
   .. automethod:: singleStep
   .. automethod:: value

   

   
   
   
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
   
   
   Methods Inherited from: :py:class:`TMouseEvents`

   .. autosummary::

   
      enterEvent
      leaveEvent
      mouseDoubleClickEvent
      mouseDragEvent
      mouseMoveEvent
      mousePressEvent
      mouseReleaseEvent
      mouseTapEvent
      wheelEvent
   
   
   Methods Inherited from: :py:class:`TKeyEvents`

   .. autosummary::

   
      keyEvent
   
   
   Methods Inherited from: :py:class:`TDragEvents`

   .. autosummary::

   
      dragEnterEvent
      dragLeaveEvent
      dragMoveEvent
      dropEvent
   
   






TTkScrollBar Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkScrollBar

.. autosummary::


  classStyle
  rangeChanged
  sliderMoved
  valueChanged

.. currentmodule::  TermTk.TTkWidgets


