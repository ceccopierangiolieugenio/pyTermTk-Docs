TTkTextEdit
===========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkTextEdit
   :show-inheritance:

   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------
   

   
   Signals linked to: :py:class:`TTkTextEditView`

   .. autosummary::
   
      TTkTextEditView.currentColorChanged
      TTkTextEditView.cursorPositionChanged
      TTkTextEditView.redoAvailable
      TTkTextEditView.textChanged
      TTkTextEditView.undoAvailable

   
   :py:class:`TTkTextEdit` signals:
   
   

   
   .. autosummary::
   
      closed
      currentStyleChanged
      focusChanged
      sizeChanged
   

   
   :ref:`Slots <Signal and Slots>`
   -------------------------------
   

   
   Slots linked to: :py:class:`TTkTextEditView`

   .. autosummary::
   
      TTkTextEditView.append
      TTkTextEditView.clear
      TTkTextEditView.copy
      TTkTextEditView.cut
      TTkTextEditView.ensureCursorVisible
      TTkTextEditView.find
      TTkTextEditView.paste
      TTkTextEditView.redo
      TTkTextEditView.setColor
      TTkTextEditView.setText
      TTkTextEditView.undo

   
   :py:class:`TTkTextEdit` slots:
   
   

   
   .. autosummary::
   
      append
      clear
      copy
      cut
      ensureCursorVisible
      find
      paste
      redo
      setColor
      setLineNumber
      setLineNumberStarting
      setText
      undo
   

   
   
   
   
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
   

   
   Methods
   -------
   

   
   Methods linked to: :py:class:`TTkTextEditView`

   .. autosummary::
   
      TTkTextEditView.append
      TTkTextEditView.clear
      TTkTextEditView.copy
      TTkTextEditView.cut
      TTkTextEditView.document
      TTkTextEditView.ensureCursorVisible
      TTkTextEditView.extraSelections
      TTkTextEditView.find
      TTkTextEditView.isReadOnly
      TTkTextEditView.isRedoAvailable
      TTkTextEditView.isUndoAvailable
      TTkTextEditView.lineWrapMode
      TTkTextEditView.multiLine
      TTkTextEditView.paste
      TTkTextEditView.redo
      TTkTextEditView.setColor
      TTkTextEditView.setExtraSelections
      TTkTextEditView.setLineWrapMode
      TTkTextEditView.setReadOnly
      TTkTextEditView.setText
      TTkTextEditView.setWordWrapMode
      TTkTextEditView.setWrapWidth
      TTkTextEditView.textCursor
      TTkTextEditView.toAnsi
      TTkTextEditView.toPlainText
      TTkTextEditView.toRawText
      TTkTextEditView.undo
      TTkTextEditView.wordWrapMode
      TTkTextEditView.wrapWidth

   
   :py:class:`TTkTextEdit` methods:
   
   


   

   
   .. automethod:: append
   .. automethod:: clear
   .. automethod:: copy
   .. automethod:: cut
   .. automethod:: document
   .. automethod:: ensureCursorVisible
   .. automethod:: extraSelections
   .. automethod:: find
   .. automethod:: getLineNumber
   .. automethod:: isReadOnly
   .. automethod:: isRedoAvailable
   .. automethod:: isUndoAvailable
   .. automethod:: lineNumberStarting
   .. automethod:: lineWrapMode
   .. automethod:: multiLine
   .. automethod:: paste
   .. automethod:: redo
   .. automethod:: ruler
   .. automethod:: setColor
   .. automethod:: setDocument
   .. automethod:: setExtraSelections
   .. automethod:: setLineNumber
   .. automethod:: setLineNumberStarting
   .. automethod:: setLineWrapMode
   .. automethod:: setReadOnly
   .. automethod:: setText
   .. automethod:: setWordWrapMode
   .. automethod:: setWrapWidth
   .. automethod:: textCursor
   .. automethod:: textEditView
   .. automethod:: toAnsi
   .. automethod:: toPlainText
   .. automethod:: toRawText
   .. automethod:: undo
   .. automethod:: wordWrapMode
   .. automethod:: wrapWidth

   

   
   
   
   Methods Inherited from: :py:class:`TTkAbstractScrollArea`

   .. autosummary::

   
      resizeEvent
      setHorizontalScrollBarPolicy
      setVerticalScrollBarPolicy
      setViewport
      update
      viewport
   
   
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
   
   




TTkTextEdit Classes
---------------------


.. currentmodule::  TermTk.TTkWidgets.TTkTextEdit

.. autoclass::  ExtraSelection
   :show-inheritance:
   :members:
.. py:currentmodule::  TermTk.TTkWidgets




TTkTextEdit Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkTextEdit

.. autosummary::


  classStyle
  currentColorChanged
  cursorPositionChanged
  redoAvailable
  textChanged
  undoAvailable

.. currentmodule::  TermTk.TTkWidgets


