TTkCheckbox
===========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkCheckbox
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkCheckbox.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color': TTkColor.RST,
                                      'borderColor':TTkColor.RST,
                                      'cbContentColor': TTkColor.fg("#dddd88")+TTkColor.bg("#000044")},
                      'disabled':    {'color': TTkColor.fg('#888888'),
                                      'borderColor':TTkColor.fg('#888888'),
                                      'cbContentColor': TTkColor.fg('#888888')},
                      'focus':       {'color': TTkColor.fg("#dddd88")+TTkColor.bg("#000044")+TTkColor.BOLD,
                                      'borderColor': TTkColor.fg("#ffff00") + TTkColor.BOLD,
                                      'cbContentColor': TTkColor.fg("#dddd88")+TTkColor.bg("#000044")+TTkColor.BOLD},
                  }
   

   
   :ref:`Signals <Signal and Slots>`
   ---------------------------------

   .. autosummary::
   
      clicked
      closed
      currentStyleChanged
      focusChanged
      sizeChanged
      stateChanged
      toggled
   

   
   :ref:`Slots <Signal and Slots>`
   -------------------------------
   

   
   .. autosummary::
   
      setCheckState
      setChecked
   

   
   
   
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
   .. autoattribute:: stateChanged
   .. autoattribute:: toggled
   

   
   Methods
   -------
   

   

   
   .. automethod:: checkState
   .. automethod:: isChecked
   .. automethod:: isTristate
   .. automethod:: keyEvent
   .. automethod:: mousePressEvent
   .. automethod:: setCheckState
   .. automethod:: setChecked
   .. automethod:: setText
   .. automethod:: setTristate
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
   
   
   
   
   






TTkCheckbox Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkCheckbox

.. autosummary::


  classStyle

.. currentmodule::  TermTk.TTkWidgets


