TTkButton
=========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkButton
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkButton.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#000044"),
                                      'borderColor': TTkColor.RST,
                                      'grid':1},
                      'disabled':    {'color': TTkColor.fg('#888888'),
                                      'borderColor':TTkColor.fg('#888888'),
                                      'grid':0},
                      'hover':       {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#000050")+TTkColor.BOLD,
                                      'borderColor': TTkColor.fg("#FFFFCC")+TTkColor.BOLD,
                                      'grid':1},
                      'checked':     {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#004488"),
                                      'borderColor': TTkColor.fg("#FFFFFF"),
                                      'grid':0},
                      'unchecked':   {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#000044"),
                                      'borderColor': TTkColor.RST,
                                      'grid':3},
                      'clicked':     {'color': TTkColor.fg("#FFFFDD")+TTkColor.BOLD,
                                      'borderColor': TTkColor.fg("#DDDDDD")+TTkColor.BOLD,
                                      'grid':0},
                      'focus':       {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#000044")+TTkColor.BOLD,
                                      'borderColor': TTkColor.fg("#ffff00") + TTkColor.BOLD,
                                      'grid':1},
                  }
   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------

   .. autosummary::
   
      clicked
      closed
      currentStyleChanged
      focusChanged
      sizeChanged
      toggled
   

   
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

   
   .. autoattribute:: clicked
   .. autoattribute:: closed
   .. autoattribute:: currentStyleChanged
   .. autoattribute:: focusChanged
   .. autoattribute:: sizeChanged
   .. autoattribute:: toggled
   

   
   Methods
   -------
   

   

   
   .. automethod:: border
   .. automethod:: isCheckable
   .. automethod:: isChecked
   .. automethod:: setCheckable
   .. automethod:: setChecked
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
   
   






TTkButton Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkButton

.. autosummary::


  classStyle

.. currentmodule::  TermTk.TTkWidgets


