TTkMenuBarButton
================

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkMenuBarButton
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkMenuBarButton.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = TTkMenuButton.classStyle | {
                      'default': TTkMenuButton.classStyle['default'] |
                                 {'borderColor':TTkColor.RST, 'shortcutColor': TTkColor.fg("#dddddd") + TTkColor.UNDERLINE,
                                  'glyphs':('├','─','┤','┄','┄','▶')},
                      'clicked': TTkMenuButton.classStyle['clicked'] |
                                 {'color': TTkColor.fg("#ffff88")},
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
   

   

   
   
   
   Slots Inherited from: :py:class:`TTkMenuButton`

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
   

   

   
   
   
   Methods Inherited from: :py:class:`TTkMenuButton`

   .. autosummary::

   
      addMenu
      addSpacer
      data
      isCheckable
      isChecked
      mouseReleaseEvent
      paintEvent
      removeMenuItem
      setCheckable
      setChecked
      setData
      setFocus
      setHighlight
      setText
      shortcutEvent
      text
   
   
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
   
   
   
   
   






TTkMenuBarButton Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkMenuBarButton

.. autosummary::


  classStyle
  dataChanged
  menuButtonClicked
  textChanged
  toggled
  triggered

.. currentmodule::  TermTk.TTkWidgets


