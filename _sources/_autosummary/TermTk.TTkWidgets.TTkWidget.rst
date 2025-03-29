TTkWidget
=========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkWidget
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkWidget.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color': TTkColor.RST,           'borderColor': TTkColor.RST},
                      'disabled':    {'color': TTkColor.fg('#888888'), 'borderColor': TTkColor.fg('#888888')},
                      # 'hover':       {'color': TTkColor.fg('#00FF00')+TTkColor.bg('#0077FF')},
                      # 'checked':     {'color': TTkColor.fg('#00FF00')+TTkColor.bg('#00FFFF')},
                      # 'clicked':     {'color': TTkColor.fg('#FFFF00')},
                      # 'focus':       {'color': TTkColor.fg('#FFFF88')},
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
   

   


   

   
   .. automethod:: clearFocus
   .. automethod:: close
   .. automethod:: currentStyle
   .. automethod:: disableWidgetCursor
   .. automethod:: enableWidgetCursor
   .. automethod:: focusInEvent
   .. automethod:: focusOutEvent
   .. automethod:: focusPolicy
   .. automethod:: geometry
   .. automethod:: getCanvas
   .. automethod:: getPixmap
   .. automethod:: getWidgetByName
   .. automethod:: hasFocus
   .. automethod:: height
   .. automethod:: hide
   .. automethod:: isEnabled
   .. automethod:: isEntered
   .. automethod:: isVisible
   .. automethod:: isVisibleAndParent
   .. automethod:: lowerWidget
   .. automethod:: maxDimension
   .. automethod:: maximumHeight
   .. automethod:: maximumSize
   .. automethod:: maximumWidth
   .. automethod:: mergeStyle
   .. automethod:: minDimension
   .. automethod:: minimumHeight
   .. automethod:: minimumSize
   .. automethod:: minimumWidth
   .. automethod:: mouseEvent
   .. automethod:: move
   .. automethod:: moveEvent
   .. automethod:: name
   .. automethod:: paintChildCanvas
   .. automethod:: paintEvent
   .. automethod:: parentWidget
   .. automethod:: pasteEvent
   .. automethod:: pos
   .. automethod:: raiseWidget
   .. automethod:: resize
   .. automethod:: resizeEvent
   .. automethod:: setCurrentStyle
   .. automethod:: setDefaultSize
   .. automethod:: setDisabled
   .. automethod:: setEnabled
   .. automethod:: setFocus
   .. automethod:: setFocusPolicy
   .. automethod:: setGeometry
   .. automethod:: setMaximumHeight
   .. automethod:: setMaximumSize
   .. automethod:: setMaximumWidth
   .. automethod:: setMinimumHeight
   .. automethod:: setMinimumSize
   .. automethod:: setMinimumWidth
   .. automethod:: setName
   .. automethod:: setParent
   .. automethod:: setStyle
   .. automethod:: setToolTip
   .. automethod:: setVisible
   .. automethod:: setWidgetCursor
   .. automethod:: show
   .. automethod:: size
   .. automethod:: style
   .. automethod:: toolTip
   .. automethod:: update
   .. automethod:: widgetItem
   .. automethod:: width
   .. automethod:: x
   .. automethod:: y

   

   
   
   
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
   
   






TTkWidget Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkWidget

.. autosummary::


  classStyle

.. currentmodule::  TermTk.TTkWidgets


