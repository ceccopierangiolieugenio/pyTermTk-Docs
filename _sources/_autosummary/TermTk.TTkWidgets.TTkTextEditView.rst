TTkTextEditView
===============

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkTextEditView
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkTextEditView.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color':         TTkColor.fg("#dddddd")+TTkColor.bg("#222222"),
                                      'selectedColor': TTkColor.fg("#ffffff")+TTkColor.bg("#008844"),
                                      'lineColor':     TTkColor.fg("#444444"),
                                      'wrapLineColor': TTkColor.fg("#888888")+TTkColor.bg("#333333")},
                      'disabled':    {'color': TTkColor.fg('#888888'),
                                      'selectedColor': TTkColor.bg("#888888"),
                                      'lineColor':     TTkColor.fg("#888888"),
                                      'wrapLineColor': TTkColor.fg('#888888')},
                      'focus':       {'selectedColor': TTkColor.fg("#ffffff")+TTkColor.bg("#008888")},
                  }
   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------

   .. autosummary::
   
      closed
      currentStyleChanged
      focusChanged
      sizeChanged
      viewChanged
      viewMovedTo
      viewSizeChanged
   

   
   :ref:`Slots <Signal and Slots>`
   -------------------------------
   

   
   .. autosummary::
   
      append
      clear
      copy
      cut
      paste
      redo
      setColor
      setText
      undo
   

   
   
   
   Slots Inherited from: :py:class:`TTkAbstractScrollView`

   .. autosummary::

   
      viewMoveTo
   
   
   Slots Inherited from: :py:class:`TTkContainer`

   .. autosummary::

   
      hide
      show
   
   
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
   .. autoattribute:: viewChanged
   .. autoattribute:: viewMovedTo
   .. autoattribute:: viewSizeChanged
   

   
   Methods
   -------
   

   

   
   .. automethod:: append
   .. automethod:: clear
   .. automethod:: copy
   .. automethod:: cut
   .. automethod:: document
   .. automethod:: isReadOnly
   .. automethod:: isRedoAvailable
   .. automethod:: isUndoAvailable
   .. automethod:: lineWrapMode
   .. automethod:: multiLine
   .. automethod:: paste
   .. automethod:: redo
   .. automethod:: setColor
   .. automethod:: setDocument
   .. automethod:: setLineWrapMode
   .. automethod:: setReadOnly
   .. automethod:: setText
   .. automethod:: setWordWrapMode
   .. automethod:: setWrapWidth
   .. automethod:: textCursor
   .. automethod:: toAnsi
   .. automethod:: toPlainText
   .. automethod:: toRawText
   .. automethod:: undo
   .. automethod:: viewDisplayedSize
   .. automethod:: viewFullAreaSize
   .. automethod:: wordWrapMode
   .. automethod:: wrapWidth

   

   
   
   
   Methods Inherited from: :py:class:`TTkAbstractScrollView`

   .. autosummary::

   
      resizeEvent
      update
      viewMoveTo
      wheelEvent
   
   
   Methods Inherited from: :py:class:`TTkContainer`

   .. autosummary::

   
      addWidget
      getPadding
      getWidgetByName
      hide
      layout
      maximumHeight
      maximumWidth
      minimumHeight
      minimumWidth
      mouseEvent
      paintChildCanvas
      removeWidget
      rootLayout
      setCurrentStyle
      setLayout
      setPadding
      show
      update
   
   
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
   
   






TTkTextEditView Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkTextEditView

.. autosummary::


  classStyle
  currentColorChanged
  redoAvailable
  textChanged
  undoAvailable

.. currentmodule::  TermTk.TTkWidgets


