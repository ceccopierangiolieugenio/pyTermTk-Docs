TTkFrame
========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkFrame
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkFrame.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color': TTkColor.fg("#dddddd")+TTkColor.bg("#222222"),
                                      'fillColor': TTkColor.RST,
                                      'borderColor': TTkColor.RST},
                      'disabled':    {'color': TTkColor.fg('#888888'),
                                      'fillColor': TTkColor.RST,
                                      'borderColor':TTkColor.fg('#888888')}
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
   

   


   

   
   .. automethod:: border
   .. automethod:: menuBar
   .. automethod:: newMenubarTop
   .. automethod:: setBorder
   .. automethod:: setMenuBar
   .. automethod:: setTitle
   .. automethod:: setTitleAlign
   .. automethod:: title
   .. automethod:: titleAlign

   

   
   
   
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
   
   






TTkFrame Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkFrame

.. autosummary::


  classStyle

.. currentmodule::  TermTk.TTkWidgets


