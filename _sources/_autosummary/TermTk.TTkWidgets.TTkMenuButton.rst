TTkMenuButton
=============

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkMenuButton
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkMenuButton.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = TTkWidget.classStyle | {
                      'default':     {'color': TTkColor.RST},
                      'highlighted': {'color': TTkColor.fg('#00FF00')+TTkColor.bg('#0055FF')},
                      'hover':       {'color': TTkColor.fg('#00FF00')+TTkColor.bg('#0077FF')},
                      'checked':     {'color': TTkColor.fg('#00FF00')+TTkColor.bg('#00FFFF')},
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
   

   
   .. autosummary::
   
      shortcutEvent
   

   
   
   
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
   

   

   
   .. automethod:: addMenu
   .. automethod:: addSpacer
   .. automethod:: data
   .. automethod:: isCheckable
   .. automethod:: isChecked
   .. automethod:: removeMenuItem
   .. automethod:: setCheckable
   .. automethod:: setChecked
   .. automethod:: setData
   .. automethod:: setHighlight
   .. automethod:: setText
   .. automethod:: shortcutEvent
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
   
   






TTkMenuButton Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkMenuButton

.. autosummary::


  classStyle
  dataChanged
  menuButtonClicked
  textChanged
  toggled
  triggered

.. currentmodule::  TermTk.TTkWidgets


