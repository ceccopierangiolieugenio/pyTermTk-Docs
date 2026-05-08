TTkListWidget
=============

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkListWidget
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkListWidget.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
              'default': {
                  'color':       TTkColor.RST,
                  'highlighted': TTkColor.bg("#004433"),
                  'hovered':     TTkColor.bg('#0088FF'),
                  'selected':    TTkColor.bg('#0055FF'),
                  'clicked':     TTkColor.fg('#FFFF00'),
                  'disabled':    TTkColor.fg('#888888'),
                  'searchColor': TTkColor.fg("#FFFF00")+TTkColor.UNDERLINE,
              }
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
   

   


   

   
   .. automethod:: addItem
   .. automethod:: addItemAt
   .. automethod:: addItems
   .. automethod:: addItemsAt
   .. automethod:: dragDropMode
   .. automethod:: filteredItems
   .. automethod:: indexOf
   .. automethod:: itemAt
   .. automethod:: items
   .. automethod:: moveItem
   .. automethod:: removeAt
   .. automethod:: removeItem
   .. automethod:: removeItems
   .. automethod:: search
   .. automethod:: searchVisibility
   .. automethod:: selectedItems
   .. automethod:: selectedLabels
   .. automethod:: selectionMode
   .. automethod:: setCurrentItem
   .. automethod:: setCurrentRow
   .. automethod:: setDragDropMode
   .. automethod:: setSearch
   .. automethod:: setSearchVisibility
   .. automethod:: setSelectionMode

   

   
   
   
   Methods Inherited from: :py:class:`TTkAbstractScrollView`

   .. autosummary::

   
      getViewOffsets
      resizeEvent
      setPadding
      update
      viewDisplayedSize
      viewFullAreaSize
      viewMoveTo
      wheelEvent
   
   
   Methods Inherited from: :py:class:`TTkContainer`

   .. autosummary::

   
      addWidget
      getPadding
      getWidgetByName
      hide
      keyEvent
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
   
   






TTkListWidget Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkListWidget

.. autosummary::


  classStyle
  itemClicked
  searchModified
  textClicked

.. currentmodule::  TermTk.TTkWidgets


