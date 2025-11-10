TTkTime
=======

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkTime
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkTime.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color':          TTkColor.fgbg("#888888","#222222")+TTkColor.UNDERLINE,
                                      'colorSeparator': TTkColor.fgbg("#CCCC00","#222222"),
                                      'hoverColor':     TTkColor.fgbg("#ffffff","#00AA66")+TTkColor.UNDERLINE,
                                      'selectedColor':  TTkColor.fgbg("#ffffff","#008844")+TTkColor.UNDERLINE},
                      'hover':       {'color':          TTkColor.fgbg("#AAAAAA","#000066")+TTkColor.UNDERLINE},
                      'disabled':    {'color':          TTkColor.fg(  "#444444")+TTkColor.UNDERLINE,
                                      'colorSeparator': TTkColor.fgbg("#666666","#222222")+TTkColor.UNDERLINE,
                                      'selectedColor':  TTkColor.fgbg("#888888","#444444")+TTkColor.UNDERLINE},
                      'focus':       {'color':          TTkColor.fgbg("#888888","#000066")+TTkColor.UNDERLINE}
                  }
   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------
   

   

   
   .. autosummary::
   
      closed
      currentStyleChanged
      focusChanged
      sizeChanged
      timeChanged
   

   
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
   .. autoattribute:: timeChanged
   

   
   Methods
   -------
   

   


   

   
   .. automethod:: setTime
   .. automethod:: time

   

   
   
   
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
   
   






TTkTime Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkTime

.. autosummary::


  classStyle

.. currentmodule::  TermTk.TTkWidgets


