TTkSlider
=========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkSlider
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkSlider.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {
                              'color': TTkColor.RST,
                              'sliderColor': TTkColor.fg('#6666bb')},
                      'disabled':    {
                              'color': TTkColor.fg('#666666'),
                              'sliderColor': TTkColor.fg('#888888')},
                      'focus':       {
                              'color': TTkColor.fg('#cccc00'),
                              'sliderColor': TTkColor.fg('#8888ff')},
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
   

   

   

   
   
   
   Slots Inherited from: :py:class:`TTkScrollBar`

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
   

   


   

   
   
   
   Methods Inherited from: :py:class:`TTkScrollBar`

   .. autosummary::

   
      color
      focusColor
      focusInEvent
      focusOutEvent
      maximum
      minimum
      mouseDragEvent
      mousePressEvent
      orientation
      pageStep
      paintEvent
      setColor
      setFocusColor
      setMaximum
      setMinimum
      setPageStep
      setRange
      setRangeTo
      setSingleStep
      setValue
      singleStep
      value
      wheelEvent
   
   
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
      setDropEventProxy
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
   
   






TTkSlider Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkSlider

.. autosummary::


  classStyle
  rangeChanged
  sliderMoved
  valueChanged

.. currentmodule::  TermTk.TTkWidgets


