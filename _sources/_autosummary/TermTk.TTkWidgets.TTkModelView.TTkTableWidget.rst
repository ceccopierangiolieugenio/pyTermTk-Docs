TTkTableWidget
==============

.. currentmodule:: TermTk.TTkWidgets.TTkModelView

.. autoclass:: TTkTableWidget
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkModelView.TTkTableWidget.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {
                          'color':          TTkColor.RST,
                          'lineColor':      TTkColor.fg("#444444"),
                          'headerColor':    TTkColor.fg("#FFFFFF")+TTkColor.bg("#444444")+TTkColor.BOLD,
                          'hoverColor':     TTkColor.fg("#FFFF00")+TTkColor.bg("#0088AA")+TTkColor.BOLD,
                          'currentColor':   TTkColor.fg("#FFFF00")+TTkColor.bg("#0088FF")+TTkColor.BOLD,
                          'selectedColor':  TTkColor.bg("#0066AA"),
                          'separatorColor': TTkColor.fg("#555555")+TTkColor.bg("#444444")},
                      'disabled':    {
                          'color':          TTkColor.fg("#888888"),
                          'lineColor':      TTkColor.fg("#888888"),
                          'headerColor':    TTkColor.fg("#888888"),
                          'hoverColor':     TTkColor.bg("#888888"),
                          'currentColor':   TTkColor.bg("#888888"),
                          'selectedColor':  TTkColor.fg("#888888"),
                          'separatorColor': TTkColor.fg("#888888")},
                  }
   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------

   .. autosummary::
   
      cellChanged
      cellClicked
      cellDoubleClicked
      cellEntered
      closed
      currentCellChanged
      currentStyleChanged
      focusChanged
      sizeChanged
      viewChanged
      viewMovedTo
      viewSizeChanged
   

   
   :ref:`Slots <Signal and Slots>`
   -------------------------------
   

   
   .. autosummary::
   
      copy
      cut
      paste
      redo
      resizeColumnToContents
      resizeColumnsToContents
      resizeRowToContents
      resizeRowsToContents
      setColumnWidth
      setRowHeight
      setSortingEnabled
      sortByColumn
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

   
   .. autoattribute:: cellChanged
   .. autoattribute:: cellClicked
   .. autoattribute:: cellDoubleClicked
   .. autoattribute:: cellEntered
   .. autoattribute:: closed
   .. autoattribute:: currentCellChanged
   .. autoattribute:: currentStyleChanged
   .. autoattribute:: focusChanged
   .. autoattribute:: sizeChanged
   .. autoattribute:: viewChanged
   .. autoattribute:: viewMovedTo
   .. autoattribute:: viewSizeChanged
   

   
   Methods
   -------
   

   

   
   .. automethod:: clearSelection
   .. automethod:: columnCount
   .. automethod:: copy
   .. automethod:: currentColumn
   .. automethod:: currentRow
   .. automethod:: cut
   .. automethod:: hSeparatorVisibility
   .. automethod:: horizontalHeader
   .. automethod:: isRedoAvailable
   .. automethod:: isSortingEnabled
   .. automethod:: isUndoAvailable
   .. automethod:: keyEvent
   .. automethod:: leaveEvent
   .. automethod:: model
   .. automethod:: mouseDoubleClickEvent
   .. automethod:: mouseDragEvent
   .. automethod:: mouseMoveEvent
   .. automethod:: mousePressEvent
   .. automethod:: mouseReleaseEvent
   .. automethod:: paste
   .. automethod:: redo
   .. automethod:: resizeColumnToContents
   .. automethod:: resizeColumnsToContents
   .. automethod:: resizeRowToContents
   .. automethod:: resizeRowsToContents
   .. automethod:: rowCount
   .. automethod:: selectAll
   .. automethod:: selectColumn
   .. automethod:: selectRow
   .. automethod:: setColumnWidth
   .. automethod:: setHSeparatorVisibility
   .. automethod:: setModel
   .. automethod:: setRowHeight
   .. automethod:: setSelection
   .. automethod:: setSortingEnabled
   .. automethod:: setVSeparatorVisibility
   .. automethod:: sortByColumn
   .. automethod:: undo
   .. automethod:: unselectColumn
   .. automethod:: unselectRow
   .. automethod:: vSeparatorVisibility
   .. automethod:: verticalHeader
   .. automethod:: viewDisplayedSize
   .. automethod:: viewFullAreaSize

   

   
   
   
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
   
   
   
   
   






TTkTableWidget Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkModelView.TTkTableWidget

.. autosummary::


  classStyle

.. currentmodule::  TermTk.TTkWidgets.TTkModelView


