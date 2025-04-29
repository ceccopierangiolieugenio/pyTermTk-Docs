TTkLineEdit
===========

.. currentmodule:: TermTk.TTkWidgets

.. autoclass:: TTkLineEdit
   :show-inheritance:

   

   .. _TermTk.TTkWidgets.TTkLineEdit.classStyle:

   Style
   -----

   .. code-block:: python

      
          classStyle = {
                      'default':     {'color':         TTkColor.fgbg("#dddddd","#222222"),
                                      'bgcolor':       TTkColor.fgbg("#666666","#222222")+TTkColor.UNDERLINE,
                                      'selectedColor': TTkColor.fgbg("#ffffff","#008844")},
                      'disabled':    {'color':         TTkColor.fg(  "#888888"),
                                      'bgcolor':       TTkColor.fg(  "#444444")+TTkColor.UNDERLINE,
                                      'selectedColor': TTkColor.fgbg("#888888","#444444")},
                      'focus':       {'color':         TTkColor.fgbg("#dddddd","#000044"),
                                      'bgcolor':       TTkColor.fgbg("#666666","#000044")+TTkColor.UNDERLINE}
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
   
      copy
      cut
      paste
      setText
   

   
   
   
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
   

   


   

   
   .. automethod:: copy
   .. automethod:: cut
   .. automethod:: echoMode
   .. automethod:: inputType
   .. automethod:: paste
   .. automethod:: setEchoMode
   .. automethod:: setInputType
   .. automethod:: setText
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
   
   




TTkLineEdit Classes
---------------------


.. currentmodule::  TermTk.TTkWidgets.TTkLineEdit

.. autoclass::  EchoMode
   :show-inheritance:
   :members:
.. py:currentmodule::  TermTk.TTkWidgets




TTkLineEdit Attributes
------------------------

.. currentmodule::  TermTk.TTkWidgets.TTkLineEdit

.. autosummary::


  classStyle
  returnPressed
  textChanged
  textEdited

.. currentmodule::  TermTk.TTkWidgets


