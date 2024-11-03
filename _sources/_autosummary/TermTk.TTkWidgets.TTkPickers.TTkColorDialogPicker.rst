TTkColorDialogPicker
====================

.. currentmodule:: TermTk.TTkWidgets.TTkPickers

.. autoclass:: TTkColorDialogPicker
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkPickers.TTkColorDialogPicker.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color': TTkColor.RST,
                                      'borderColor': TTkColor.RST,
                                      'titleColor': TTkColor.fg("#dddddd")+TTkColor.bg("#222222")},
                      'disabled':    {'color': TTkColor.fg('#888888'),
                                      'borderColor':TTkColor.fg('#888888'),
                                      'titleColor': TTkColor.fg('#888888')},
                      'focus':       {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#000044")+TTkColor.BOLD,
                                      'borderColor': TTkColor.fg("#ffff55"),
                                      'titleColor': TTkColor.fg("#ffffdd")+TTkColor.bg("#222222")},
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
   

   

   
   .. automethod:: color
   .. automethod:: setColor

   

   
   
   
   Methods Inherited from: :py:class:`TTkWindow`

   .. autosummary::

   
      focusOutEvent
      mouseDragEvent
      mousePressEvent
      paintEvent
      resizeEvent
      setWindowFlag
      windowFlag
   
   
   Methods Inherited from: :py:class:`TTkResizableFrame`

   .. autosummary::

   
      mouseDragEvent
      mousePressEvent
   
   
   Methods Inherited from: :py:class:`TTkFrame`

   .. autosummary::

   
      border
      menuBar
      newMenubarTop
      paintEvent
      resizeEvent
      setBorder
      setMenuBar
      setTitle
      setTitleAlign
      title
      titleAlign
   
   
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
   
   
   
   
   






TTkColorDialogPicker Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkPickers.TTkColorDialogPicker

.. autosummary::


  classStyle
  colorSelected
  customButtons

.. currentmodule::  TermTk.TTkWidgets.TTkPickers


