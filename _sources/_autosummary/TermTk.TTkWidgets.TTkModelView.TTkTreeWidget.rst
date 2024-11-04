TTkTreeWidget
=============

.. currentmodule:: TermTk.TTkWidgets.TTkModelView

.. autoclass:: TTkTreeWidget
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkModelView.TTkTreeWidget.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {
                          'color': TTkColor.RST,
                          'lineColor': TTkColor.fg("#444444"),
                          'headerColor': TTkColor.fg("#ffffff")+TTkColor.bg("#444444")+TTkColor.BOLD,
                          'selectedColor': TTkColor.fg("#ffff88")+TTkColor.bg("#000066")+TTkColor.BOLD,
                          'separatorColor': TTkColor.fg("#444444")},
                      'disabled':    {
                          'color': TTkColor.fg("#888888"),
                          'lineColor': TTkColor.fg("#888888"),
                          'headerColor': TTkColor.fg("#888888"),
                          'selectedColor': TTkColor.fg("#888888"),
                          'separatorColor': TTkColor.fg("#888888")},
                  }
   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------

   .. autosummary::
   
      closed
      currentStyleChanged
      focusChanged
      itemActivated
      itemChanged
      itemClicked
      itemCollapsed
      itemDoubleClicked
      itemExpanded
      sizeChanged
      viewChanged
      viewMovedTo
      viewSizeChanged
   

   
   :ref:`Slots <Signal and Slots>`
   -------------------------------
   

   

   
   
   
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
   .. autoattribute:: itemActivated
   .. autoattribute:: itemChanged
   .. autoattribute:: itemClicked
   .. autoattribute:: itemCollapsed
   .. autoattribute:: itemDoubleClicked
   .. autoattribute:: itemExpanded
   .. autoattribute:: sizeChanged
   .. autoattribute:: viewChanged
   .. autoattribute:: viewMovedTo
   .. autoattribute:: viewSizeChanged
   

   
   Methods
   -------
   

   

   
   .. automethod:: addTopLevelItem
   .. automethod:: addTopLevelItems
   .. automethod:: clear
   .. automethod:: columnWidth
   .. automethod:: indexOfTopLevelItem
   .. automethod:: isSortingEnabled
   .. automethod:: resizeColumnToContents
   .. automethod:: selectedItems
   .. automethod:: setColumnWidth
   .. automethod:: setHeaderLabels
   .. automethod:: setSortingEnabled
   .. automethod:: sortColumn
   .. automethod:: sortItems
   .. automethod:: takeTopLevelItem
   .. automethod:: topLevelItem
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
   
   






TTkTreeWidget Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkModelView.TTkTreeWidget

.. autosummary::


  classStyle

.. currentmodule::  TermTk.TTkWidgets.TTkModelView


