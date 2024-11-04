TTkComboBox
===========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkComboBox
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkComboBox.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#222222"),
                                      'borderColor':TTkColor.RST},
                      'disabled':    {'color': TTkColor.fg('#888888'),
                                      'borderColor':TTkColor.fg('#888888')},
                      'focus':       {'color': TTkColor.fg("#ffff88")+TTkColor.bg("#222222"),
                                      'borderColor': TTkColor.fg("#ffff00") + TTkColor.BOLD},
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
   
      setCurrentIndex
      setCurrentText
      setEditText
   

   
   
   
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
   

   

   
   .. automethod:: addItem
   .. automethod:: addItems
   .. automethod:: clear
   .. automethod:: currentIndex
   .. automethod:: currentText
   .. automethod:: insertPolicy
   .. automethod:: isEditable
   .. automethod:: lineEdit
   .. automethod:: setCurrentIndex
   .. automethod:: setCurrentText
   .. automethod:: setEditText
   .. automethod:: setEditable
   .. automethod:: setInsertPolicy
   .. automethod:: setTextAlign
   .. automethod:: textAlign

   

   
   
   
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
   
   






TTkComboBox Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkComboBox

.. autosummary::


  classStyle
  currentIndexChanged
  currentTextChanged
  editTextChanged

.. currentmodule::  TermTk.TTkWidgets


