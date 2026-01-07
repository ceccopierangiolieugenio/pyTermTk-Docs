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
              'default':{'searchColor': TTkColor.fg("#FFFF00") + TTkColor.UNDERLINE}}
      
          @dataclass(frozen=True)
          class _DropListData:
              widget: TTkAbstractScrollView
              items: list
      
          __slots__ = ('_selectedItems', '_selectionMode',
                       '_highlighted', '_items', '_filteredItems',
                       '_dragPos', '_dndMode',
                       '_searchText', '_showSearch',
                       # Signals
                       '_itemClicked', '_textClicked', '_searchModified')
      
          _items:List[TTkAbstractListItem]
          _showSearch:bool
          _highlighted:Optional[TTkAbstractListItem]
          _selectedItems:List[TTkAbstractListItem]
          _filteredItems:List[TTkAbstractListItem]
      
          def __init__(self, *,
                       items:List[TTkAbstractListItemType]=[],
                       selectionMode:TTkK.SelectionMode=TTkK.SelectionMode.SingleSelection,
                       dragDropMode:TTkK.DragDropMode=TTkK.DragDropMode.NoDragDrop,
                       showSearch:bool=True,
                       **kwargs) -> None:
              '''
              :param items: Initial list of items (Any or :py:class:`TTkAbstractListItem` objects), defaults to []
              :type items: list, optional
              :param selectionMode: Selection behavior (:py:class:`TTkK.SelectionMode.SingleSelection` or :py:class:`TTkK.SelectionMode.MultiSelection`), defaults to :py:class:`TTkK.SelectionMode.SingleSelection`
              :type selectionMode: :py:class:`TTkK.SelectionMode`, optional
              :param dragDropMode: Drag and drop behavior (NoDragDrop, InternalMove, DragOnly, DropOnly, DragDrop), defaults to NoDragDrop
              :type dragDropMode: :py:class:`TTkK.DragDropMode`, optional
              :param showSearch: Whether to show the search hint at the top, defaults to True
              :type showSearch: bool, optional
              '''
              # Signals
              self._itemClicked = pyTTkSignal(TTkAbstractListItem)
              self._textClicked = pyTTkSignal(str)
              self._searchModified = pyTTkSignal(str)
      
              # Default Class Specific Values
              self._selectionMode = selectionMode
              self._selectedItems = []
              self._items = []
              self._filteredItems = self._items
              self._highlighted = None
              self._dragPos = None
              self._dndMode = dragDropMode
              self._searchText:str = ''
              self._showSearch:bool = showSearch
              # Init Super
              super().__init__(**kwargs)
              self.addItemsAt(items=items, pos=0)
              self.viewChanged.connect(self._viewChangedHandler)
              self.setFocusPolicy(TTkK.ClickFocus | TTkK.TabFocus)
              self.searchModified.connect(self._searchModifiedHandler)
      
          @pyTTkSlot()
          def _viewChangedHandler(self):
              x,y = self.getViewOffsets()
              self.layout().setOffset(-x,-y)
      
          @pyTTkSlot(TTkAbstractListItem)
          def _labelSelectedHandler(self, label:TTkAbstractListItem):
              if self._selectionMode == TTkK.SingleSelection:
                  for item in self._selectedItems:
                      item._setSelected(False)
                      item._setHighlighted(False)
                  self._selectedItems = [label]
                  label._setSelected(True)
              elif self._selectionMode == TTkK.MultiSelection:
                  for item in self._selectedItems:
                      item._setHighlighted(False)
                  label._setSelected(not label._selected)
                  if label._selected:
                      self._selectedItems.append(label)
                  else:
                      self._selectedItems.remove(label)
              if self._highlighted:
                  self._highlighted._setHighlighted(False)
              label._setHighlighted(True)
              self._highlighted = label
              self.itemClicked.emit(label)
              self.textClicked.emit(label.text())
      
          @pyTTkSlot(str)
          def _searchModifiedHandler(self) -> None:
              if self._showSearch and self._searchText:
                  self.setPadding(1,0,0,0)
              else:
                  self.setPadding(0,0,0,0)
      
              if self._searchText:
                  text = self._searchText.lower()
                  self._filteredItems = [i for i in self._items if text in i._lowerText]
                  for item in self._items:
                      item._quickVisible = text in item._lowerText
              else:
                  self._filteredItems = self._items
                  for item in self._items:
                      item._quickVisible = True
                      item.setVisible(True)
      
              self._placeItems()
      
          def search(self) -> str:
              '''
              Returns the current search text.
      
              :return: The active search filter string
              :rtype: str
              '''
              return self._searchText
      
          def setSearch(self, search:str) -> None:
              '''
              Sets the search text to filter items.
      
              :param search: The search string to filter by
              :type search: str
              '''
              self._searchText = search
              self.searchModified.emit(search)
      
          def searchVisibility(self) -> bool:
              '''
              Returns whether the search hint is visible.
      
              :return: True if search hint is shown
              :rtype: bool
              '''
              return self._showSearch
      
          def setSearchVisibility(self, visibility:bool) -> None:
              '''
              Sets the visibility of the search hint at the top of the list.
      
              :param visibility: True to show search hint, False to hide
              :type visibility: bool
              '''
              self._showSearch = visibility
      
          def dragDropMode(self) -> TTkK.DragDropMode:
              '''
              Returns the current drag-drop mode.
      
              :return: The drag-drop behavior setting
              :rtype: :py:class:`TTkK.DragDropMode`
              '''
              return self._dndMode
      
          def setDragDropMode(self, dndMode:TTkK.DragDropMode) -> None:
              '''
              Sets the drag-drop mode for this list.
      
              :param dndMode: The new drag-drop behavior
              :type dndMode: :py:class:`TTkK.DragDropMode`
              '''
              self._dndMode = dndMode
      
          def selectionMode(self) -> TTkK.SelectionMode:
              '''
              Returns the current selection mode.
      
              :return: The selection behavior setting
              :rtype: :py:class:`TTkK.SelectionMode`
              '''
              return self._selectionMode
      
          def setSelectionMode(self, mode:TTkK.SelectionMode) -> None:
              '''
              Sets the selection mode for this list.
      
              :param mode: The new selection behavior (SingleSelection or MultiSelection)
              :type mode: :py:class:`TTkK.SelectionMode`
              '''
              self._selectionMode = mode
      
          def selectedItems(self) -> List[TTkAbstractListItem]:
              '''
              Returns the list of currently selected items.
      
              :return: List of selected item widgets
              :rtype: list[:py:class:`TTkAbstractListItem`]
              '''
              return self._selectedItems
      
          def selectedLabels(self) -> List[str]:
              '''
              Returns the text of all selected items.
      
              :return: List of selected item texts
              :rtype: list[str]
              '''
              return [i.text() for i in self._selectedItems]
      
          def items(self) -> List[TTkAbstractListItem]:
              '''
              Returns all items in the list.
      
              :return: Complete list of items
              :rtype: list[:py:class:`TTkAbstractListItem`]
              '''
              return self._items
      
          def filteredItems(self) -> List[TTkAbstractListItem]:
              '''
              Returns items matching the current search filter.
      
              :return: Filtered list of visible items
              :rtype: list[:py:class:`TTkAbstractListItem`]
              '''
              return self._filteredItems
      
          def resizeEvent(self, w:int, h:int) -> None:
              maxw = 0
              for item in self.layout().children():
                  maxw = max(maxw,item.minimumWidth())
              maxw = max(self.width(),maxw)
              for item in self.layout().children():
                  x,y,_,h = item.geometry()
                  item.setGeometry(x,y,maxw,h)
              TTkAbstractScrollView.resizeEvent(self, w, h)
      
          def addItem(self, item:TTkAbstractListItemType, data:Any=None) -> None:
              '''
              Appends a single item to the end of the list.
      
              :param item: The item to add (string or :py:class:`TTkAbstractListItem`)
              :type item: str or :py:class:`TTkAbstractListItem`
              :param data: Optional user data to associate with the item
              :type data: Any, optional
              '''
              self.addItemAt(item, len(self._items), data)
      
          def addItems(self, items:List[TTkAbstractListItemType]) -> None:
              '''
              Appends multiple items to the end of the list.
      
              :param items: List of items to add (strings or :py:class:`TTkAbstractListItem` objects)
              :type items: list
              '''
              self.addItemsAt(items=items, pos=len(self._items))
      
          def _placeItems(self) -> None:
              '''
              Internal method to position items in the layout.
              '''
              minw = self.width()
              for item in self._items:
                  if item in self._filteredItems:
                      minw = max(minw,item.minimumWidth())
              for y,item in enumerate(self._filteredItems):
                  item.setGeometry(0,y,minw,1)
              self.viewChanged.emit()
              self.update()
      
          def addItemAt(self, item:TTkAbstractListItemType, pos:int, data:Any=None) -> None:
              '''
              Inserts a single item at the specified position.
      
              :param item: The item to insert (string or :py:class:`TTkAbstractListItem`)
              :type item: str or :py:class:`TTkAbstractListItem`
              :param pos: The index position to insert at
              :type pos: int
              :param data: Optional user data to associate with the item
              :type data: Any, optional
              '''
              if isinstance(item, str) or isinstance(item, TTkString):
                  item = TTkAbstractListItem(text=item, data=data)
              self.addItemsAt([item],pos)
      
          def addItemsAt(self, items:List[TTkAbstractListItemType], pos:int) -> None:
              '''
              Inserts multiple items at the specified position.
      
              :param items: List of items to insert (strings or :py:class:`TTkAbstractListItem` objects)
              :type items: list
              :param pos: The index position to insert at
              :type pos: int
              '''
              items = [
                  _i if isinstance(_i, TTkAbstractListItem)
                  else TTkAbstractListItem(
                          text=TTkString(_i if isinstance(_i,TTkString) else str(_i)),
                          data=_i)
                  for _i in items
              ]
              for item in items:
                  if not issubclass(type(item),TTkAbstractListItem):
                      TTkLog.error(f"{item=} is not an TTkAbstractListItem")
                      return
              for item in items:
                  item.listItemClicked.connect(self._labelSelectedHandler)
              self._items[pos:pos] = items
              self.layout().addWidgets(items)
              self._placeItems()
      
          def indexOf(self, item:TTkAbstractListItemType) -> int:
              '''
              Returns the index of the given item.
      
              :param item: The item to find
              :type item: :py:class:`TTkAbstractListItem` or the data or the text to be searched
              :return: The index of the item, or -1 if not found
              :rtype: int
              '''
              if isinstance(item, TTkAbstractListItem):
                  return self._items.index(item)
              for i, it in enumerate(self._items):
                  if it.data() == item or it.text() == item:
                      return i
              return -1
      
          def itemAt(self, pos:int) -> TTkAbstractListItem:
              '''
              Returns the item at the specified index.
      
              :param pos: The index position
              :type pos: int
              :return: The item at that position
              :rtype: :py:class:`TTkAbstractListItem`
              '''
              return self._items[pos]
      
          def moveItem(self, fr:int, to:int) -> None:
              '''
              Moves an item from one position to another.
      
              :param fr: The source index
              :type fr: int
              :param to: The destination index
              :type to: int
              '''
              fr = max(min(fr,len(self._items)-1),0)
              to = max(min(to,len(self._items)-1),0)
              # Swap
              self._items[to] , self._items[fr] = self._items[fr] , self._items[to]
              self._placeItems()
      
          def removeItem(self, item:TTkAbstractListItem) -> None:
              '''
              Removes a single item from the list.
      
              :param item: The item to remove
              :type item: :py:class:`TTkAbstractListItem`
              '''
              self.removeItems([item])
      
          def removeItems(self, items:List[TTkAbstractListItem]) -> None:
              '''
              Removes multiple items from the list.
      
              :param items: List of items to remove
              :type items: list[:py:class:`TTkAbstractListItem`]
              '''
              self.layout().removeWidgets(items)
              for item in items.copy():
                  item.listItemClicked.disconnect(self._labelSelectedHandler)
                  item._setSelected(False)
                  item._setHighlighted(False)
                  self._items.remove(item)
                  if item in self._selectedItems:
                      self._selectedItems.remove(item)
                  if item == self._highlighted:
                      self._highlighted = None
              self._placeItems()
      
          def removeAt(self, pos:int) -> None:
              '''
              Removes the item at the specified index.
      
              :param pos: The index of the item to remove
              :type pos: int
              '''
              self.removeItem(self._items[pos])
      
          def setCurrentRow(self, row:int) -> None:
              '''
              Selects the item at the specified row.
      
              :param row: The row index to select
              :type row: int
              '''
              if row<len(self._items):
                  item = self._items[row]
                  self.setCurrentItem(item)
      
          def setCurrentItem(self, item:TTkAbstractListItem) -> None:
              '''
              Selects the specified item and emits the itemClicked signal.
      
              :param item: The item to select
              :type item: :py:class:`TTkAbstractListItem`
              '''
              item.listItemClicked.emit(item)
      
          def _moveToHighlighted(self) -> None:
              '''
              Internal method to scroll the view to show the highlighted item.
              '''
              index = self._items.index(self._highlighted)
              h = self.height()
              offx,offy = self.getViewOffsets()
              if index >= h+offy-1:
                  self.viewMoveTo(offx, index-h+1)
              elif index <= offy:
                  self.viewMoveTo(offx, index)
      
          def mousePressEvent(self, evt:TTkMouseEvent) -> bool:
              return True
      
          def mouseDragEvent(self, evt:TTkMouseEvent) -> bool:
              if not(self._dndMode & TTkK.DragDropMode.AllowDrag):
                  return False
              if not (items:=self._selectedItems.copy()):
                  return True
              drag = TTkDrag()
              data =TTkListWidget._DropListData(widget=self,items=items)
              h = min(3,ih:=len(items)) + 2 + (1 if ih>3 else 0)
              w = min(20,iw:=max([it.text().termWidth() for it in items[:3]])) + 2
              pm = TTkCanvas(width=w,height=h)
              for y,it in enumerate(items[:3],1):
                  txt = it.text()
                  if txt.termWidth() < 20:
                      pm.drawText(pos=(1,y), text=it.text())
                  else:
                      pm.drawText(pos=(1,y), text=it.text(), width=17)
                      pm.drawText(pos=(18,y), text='...')
              if ih>3:
                  pm.drawText(pos=(1,4), text='...')
              pm.drawBox(pos=(0,0),size=(w,h))
              drag.setPixmap(pm)
              drag.setData(data)
              drag.exec()
              return True
      
          def dragEnterEvent(self, evt:TTkDnDEvent) -> bool:
              if not(self._dndMode & TTkK.DragDropMode.AllowDrop):
                  return False
              if issubclass(type(evt.data()),TTkListWidget._DropListData):
                  return self.dragMoveEvent(evt)
              return False
      
          def dragMoveEvent(self, evt:TTkDnDEvent) -> bool:
              offx,offy = self.getViewOffsets()
              y=min(evt.y+offy,len(self._items))
              self._dragPos = (offx+evt.x, y)
              self.update()
              return True
      
          def dragLeaveEvent(self, evt:TTkDnDEvent) -> bool:
              self._dragPos = None
              self.update()
              return True
      
          def dropEvent(self, evt:TTkDnDEvent) -> bool:
              if not(self._dndMode & TTkK.DragDropMode.AllowDrop):
                  return False
              self._dragPos = None
              if not issubclass(type(evt.data())  ,TTkListWidget._DropListData):
                  return False
              t,b,l,r = self.getPadding()
              offx,offy = self.getViewOffsets()
              wid   = evt.data().widget
              items = evt.data().items
              if wid and items:
                  wid.removeItems(items)
                  wid._searchModifiedHandler()
                  for it in items:
                      it.setCurrentStyle(it.style()['default'])
                  yPos = offy+evt.y-t
                  if self._filteredItems:
                      if yPos < 0:
                          yPos = 0
                      elif yPos > len(self._filteredItems):
                          yPos = len(self._items)
                      elif yPos == len(self._filteredItems):
                          filteredItemAt = self._filteredItems[-1]
                          yPos = self._items.index(filteredItemAt)+1
                      else:
                          filteredItemAt = self._filteredItems[yPos]
                          yPos = self._items.index(filteredItemAt)
                  else:
                      yPos = 0
                  self.addItemsAt(items,yPos)
                  self._searchModifiedHandler()
                  return True
              return False
      
          def keyEvent(self, evt:TTkKeyEvent) -> bool:
              # if not self._highlighted: return False
              if ( not self._searchText and evt.type == TTkK.Character and evt.key==" " ) or \
                 ( evt.type == TTkK.SpecialKey and evt.key == TTkK.Key_Enter ):
                  if self._highlighted:
                      self._highlighted.listItemClicked.emit(self._highlighted)
      
              elif evt.type == TTkK.Character:
                  # Add this char to the search text
                  self._searchText += evt.key
                  self.update()
                  self.searchModified.emit(self._searchText)
      
              elif ( evt.type == TTkK.SpecialKey and
                     evt.key == TTkK.Key_Tab ):
                  return False
      
              elif ( evt.type == TTkK.SpecialKey and
                     evt.key in (TTkK.Key_Delete,TTkK.Key_Backspace) and
                     self._searchText ):
                  # Handle the backspace to remove the last char from the search text
                  self._searchText = self._searchText[:-1]
                  self.update()
                  self.searchModified.emit(self._searchText)
      
              elif ( evt.type == TTkK.SpecialKey and
                     self._filteredItems):
                  # Handle the arrow/movement keys
                  index = 0
                  if self._highlighted:
                      self._highlighted._setHighlighted(False)
                      if self._highlighted not in self._filteredItems:
                          self._highlighted = self._filteredItems[0]
                      index = self._filteredItems.index(self._highlighted)
                  offx,offy = self.getViewOffsets()
                  h = self.height()
                  if evt.key == TTkK.Key_Up:
                      index = max(0, index-1)
                  elif evt.key == TTkK.Key_Down:
                      index = min(len(self._filteredItems)-1, index+1)
                  elif evt.key == TTkK.Key_PageUp:
                      index = max(0, index-h)
                  elif evt.key == TTkK.Key_PageDown:
                      index = min(len(self._filteredItems)-1, index+h)
                  elif evt.key == TTkK.Key_Right:
                      self.viewMoveTo(offx+1, offy)
                  elif evt.key == TTkK.Key_Left:
                      self.viewMoveTo(offx-1, offy)
                  elif evt.key == TTkK.Key_Home:
                      self.viewMoveTo(0, offy)
                  elif evt.key == TTkK.Key_End:
                      self.viewMoveTo(0x10000, offy)
                  elif evt.key in (TTkK.Key_Delete,TTkK.Key_Backspace):
                      if self._searchText:
                          self._searchText = self._searchText[:-1]
                          self.update()
                          self.searchModified.emit(self._searchText)
                  self._highlighted = self._filteredItems[index]
                  self._highlighted._setHighlighted(True)
                  self._moveToHighlighted()
      
              else:
                  return False
              return True
      
          def focusInEvent(self):
              if not self._items: return
              if not self._highlighted:
                  self._highlighted = self._items[0]
              self._highlighted._setHighlighted(True)
      
          def focusOutEvent(self):
              if self._highlighted:
                  self._highlighted._setHighlighted(False)
              self._dragPos = None
      
          # Stupid hack to paint on top of the child widgets
          def paintChildCanvas(self):
              super().paintChildCanvas()
              if self._dragPos:
                  canvas = self.getCanvas()
                  x,y = self._dragPos
                  offx,offy = self.getViewOffsets()
                  p1 = (0,y-offy-1)
                  p2 = (0,y-offy)
                  canvas.drawText(pos=p1,text="╙─╼", color=TTkColor.fg("#FFFF00")+TTkColor.bg("#008855"))
                  canvas.drawText(pos=p2,text="╓─╼", color=TTkColor.fg("#FFFF00")+TTkColor.bg("#008855"))
      
          def paintEvent(self, canvas: TTkCanvas) -> None:
              if self._showSearch and self._searchText:
                  w,h = self.size()
                  color = self.currentStyle()['searchColor']
                  if len(self._searchText) > w:
                      text = TTkString("≼",TTkColor.BG_BLUE+TTkColor.FG_CYAN)+TTkString(self._searchText[-w+1:],color)
                  else:
                      text = TTkString(self._searchText,color)
                  canvas.drawTTkString(pos=(0,0),text=text, color=color, width=w)
      
   

   
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


