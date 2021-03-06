INCLUDES = -I$(top_srcdir)/include -I$(top_srcdir) $(freetype2_CFLAGS) $(pcre_CFLAGS)

libCEGUIBase_la_LDFLAGS =
libCEGUIBase_la_LIBADD =

if MINGW32_BUILD
libCEGUIBase_la_CPPFLAGS = -DCEGUIBASE_EXPORTS
libCEGUIBase_la_LDFLAGS += -shared -no-undefined
libCEGUIBase_la_LIBADD += -lwinmm
endif

libCEGUIBase_la_LDFLAGS += -version-info @CEGUI_VERSION_INFO@
libCEGUIBase_la_LIBADD += $(freetype2_LIBS) $(pcre_LIBS)

lib_LTLIBRARIES=libCEGUIBase.la

libCEGUIBase_la_SOURCES = CEGUIBase.cpp \
                      CEGUIBoundSlot.cpp \
                      CEGUIColourRect.cpp \
                      CEGUIConfig_xmlHandler.cpp \
                      CEGUICoordConverter.cpp \
                      CEGUIDataContainer.cpp \
                      CEGUIDefaultLogger.cpp \
                      CEGUIDefaultResourceProvider.cpp \
                      CEGUIDynamicModule.cpp \
                      CEGUIEvent.cpp \
                      CEGUIEventArgs.cpp \
                      CEGUIEventSet.cpp \
                      CEGUIEventSignal.cpp \
                      CEGUIEventSignalSet.cpp \
                      CEGUIExceptions.cpp \
                      CEGUIFactoryModule.cpp \
                      CEGUIFont.cpp \
                      CEGUIFontManager.cpp \
                      CEGUIFontProperties.cpp \
                      CEGUIFont_xmlHandler.cpp \
                      CEGUIFreeTypeFont.cpp \
                      CEGUIGlobalEventSet.cpp \
                      CEGUIGUILayout_xmlHandler.cpp \
                      CEGUIImage.cpp \
					  CEGUIImageCodec.cpp \
                      CEGUIImageset.cpp \
                      CEGUIImagesetManager.cpp \
                      CEGUIImageset_xmlHandler.cpp \
                      CEGUILogger.cpp \
                      CEGUIMouseCursor.cpp \
                      CEGUIPixmapFont.cpp \
                      CEGUIProperty.cpp \
                      CEGUIPropertyHelper.cpp \
                      CEGUIPropertySet.cpp \
                      CEGUIRect.cpp \
                      CEGUIRenderCache.cpp \
                      CEGUIRenderer.cpp \
                      CEGUIScheme.cpp \
                      CEGUISchemeManager.cpp \
                      CEGUIScheme_xmlHandler.cpp \
                      CEGUIScriptModule.cpp \
                      CEGUIScriptWindowHelper.cpp \
                      CEGUISize.cpp \
                      CEGUIString.cpp \
                      CEGUISubscriberSlot.cpp \
                      CEGUISystem.cpp \
                      CEGUITextUtils.cpp \
                      CEGUITexture.cpp \
                      CEGUIWindow.cpp \
                      CEGUIWindowFactory.cpp \
                      CEGUIWindowFactoryManager.cpp \
                      CEGUIWindowManager.cpp \
                      CEGUIWindowProperties.cpp \
                      CEGUIWindowRenderer.cpp \
                      CEGUIWindowRendererManager.cpp \
                      CEGUIXMLAttributes.cpp \
                      CEGUIXMLHandler.cpp \
                      CEGUIXMLParser.cpp \
                      CEGUIXMLSerializer.cpp \
                      CEGUIcolour.cpp \
                      elements/CEGUIBaseFactories.cpp \
                      elements/CEGUIButtonBase.cpp \
                      elements/CEGUICheckbox.cpp \
                      elements/CEGUIClippedContainer.cpp \
                      elements/CEGUICheckboxProperties.cpp \
                      elements/CEGUICombobox.cpp \
                      elements/CEGUIComboboxProperties.cpp \
                      elements/CEGUIComboDropList.cpp \
                      elements/CEGUIDragContainer.cpp \
                      elements/CEGUIDragContainerProperties.cpp \
                      elements/CEGUIEditbox.cpp \
                      elements/CEGUIEditboxProperties.cpp \
                      elements/CEGUIFrameWindow.cpp \
                      elements/CEGUIFrameWindowProperties.cpp \
                      elements/CEGUIGroupBox.cpp \
                      elements/CEGUIGUISheet.cpp \
                      elements/CEGUIItemEntry.cpp \
                      elements/CEGUIItemEntryProperties.cpp \
                      elements/CEGUIItemListBase.cpp \
                      elements/CEGUIItemListBaseProperties.cpp \
                      elements/CEGUIItemListbox.cpp \
                      elements/CEGUIItemListboxProperties.cpp\
                      elements/CEGUIListbox.cpp \
                      elements/CEGUIListboxItem.cpp \
                      elements/CEGUIListboxProperties.cpp \
                      elements/CEGUIListboxTextItem.cpp \
                      elements/CEGUIListHeader.cpp \
                      elements/CEGUIListHeaderProperties.cpp \
                      elements/CEGUIListHeaderSegment.cpp \
                      elements/CEGUIListHeaderSegmentProperties.cpp \
                      elements/CEGUIMenubar.cpp \
                      elements/CEGUIMenuBase.cpp \
                      elements/CEGUIMenuBaseProperties.cpp \
                      elements/CEGUIMenuItem.cpp \
                      elements/CEGUIMultiColumnList.cpp \
                      elements/CEGUIMultiColumnListProperties.cpp \
                      elements/CEGUIMultiLineEditbox.cpp \
                      elements/CEGUIMultiLineEditboxProperties.cpp \
                      elements/CEGUIPopupMenu.cpp \
                      elements/CEGUIPopupMenuProperties.cpp \
                      elements/CEGUIProgressBar.cpp \
                      elements/CEGUIProgressBarProperties.cpp \
                      elements/CEGUIPushButton.cpp \
                      elements/CEGUIRadioButton.cpp \
                      elements/CEGUIRadioButtonProperties.cpp \
                      elements/CEGUIScrollablePane.cpp \
                      elements/CEGUIScrollablePaneProperties.cpp \
                      elements/CEGUIScrollbar.cpp \
                      elements/CEGUIScrollbarProperties.cpp \
                      elements/CEGUIScrolledContainer.cpp \
                      elements/CEGUIScrolledContainerProperties.cpp \
                      elements/CEGUIScrolledItemListBase.cpp \
                      elements/CEGUIScrolledItemListBaseProperties.cpp \
                      elements/CEGUISlider.cpp \
                      elements/CEGUISliderProperties.cpp \
                      elements/CEGUISpinner.cpp \
                      elements/CEGUISpinnerProperties.cpp \
                      elements/CEGUITabButton.cpp \
                      elements/CEGUITabControl.cpp \
                      elements/CEGUITabControlProperties.cpp \
                      elements/CEGUIThumb.cpp \
                      elements/CEGUIThumbProperties.cpp \
                      elements/CEGUITitlebar.cpp \
                      elements/CEGUITitlebarProperties.cpp \
                      elements/CEGUITooltip.cpp \
                      elements/CEGUITooltipProperties.cpp \
                      elements/CEGUITree.cpp \
                      elements/CEGUITreeProperties.cpp \
                      elements/CEGUITreeItem.cpp \
                      falagard/CEGUIFalComponentBase.cpp \
                      falagard/CEGUIFalDimensions.cpp \
                      falagard/CEGUIFalFrameComponent.cpp \
                      falagard/CEGUIFalImageryComponent.cpp \
                      falagard/CEGUIFalImagerySection.cpp \
                      falagard/CEGUIFalLayerSpecification.cpp \
                      falagard/CEGUIFalNamedArea.cpp \
                      falagard/CEGUIFalPropertyDefinition.cpp \
                      falagard/CEGUIFalPropertyDefinitionBase.cpp \
                      falagard/CEGUIFalPropertyLinkDefinition.cpp \
                      falagard/CEGUIFalPropertyInitialiser.cpp \
                      falagard/CEGUIFalSectionSpecification.cpp \
                      falagard/CEGUIFalStateImagery.cpp \
                      falagard/CEGUIFalTextComponent.cpp \
                      falagard/CEGUIFalWidgetComponent.cpp \
                      falagard/CEGUIFalWidgetLookFeel.cpp \
                      falagard/CEGUIFalWidgetLookManager.cpp \
                      falagard/CEGUIFalXMLEnumHelper.cpp \
                      falagard/CEGUIFalagard_xmlHandler.cpp

if MACOSX_BUILD
INCLUDES += -I$(top_srcdir)/src/implementations/mac
libCEGUIBase_la_SOURCES += implementations/mac/macPlugins.cpp
endif

EXTRA_DIST = implementations/mac/macPlugins.h
