##Good news
Fixed in 10.7.2 -- See [@radian's comment](https://twitter.com/#!/radian/status/123072764142829568)

    GNU gdb 6.3.50-20050815 (Apple version gdb-1705) (Fri Jul  1 10:50:06 UTC 2011)
    Copyright 2004 Free Software Foundation, Inc.
    GDB is free software, covered by the GNU General Public License, and you are
    welcome to change it and/or distribute copies of it under certain conditions.
    Type "show copying" to see the conditions.
    There is absolutely no warranty for GDB.  Type "show warranty" for details.
    This GDB was configured as "x86_64-apple-darwin".tty /dev/ttys007
    [Switching to process 54969 thread 0x0]
    2011-10-09 17:36:43.066 SandPath[54969:407] -[NSRemoteOpenPanel _configureForFilename:]: unrecognized selector sent to instance 0x101886f30
    2011-10-09 17:36:43.074 SandPath[54969:407] An uncaught exception was raised
    2011-10-09 17:36:43.074 SandPath[54969:407] -[NSRemoteOpenPanel _configureForFilename:]: unrecognized selector sent to instance 0x101886f30
    2011-10-09 17:36:43.081 SandPath[54969:407] (
         0   CoreFoundation                      0x00007fff8efb2986 __exceptionPreprocess + 198
         1   libobjc.A.dylib                     0x00007fff927b0d5e objc_exception_throw + 43
         2   CoreFoundation                      0x00007fff8f03e5ae -[NSObject doesNotRecognizeSelector:] + 190
         3   CoreFoundation                      0x00007fff8ef9f803 ___forwarding___ + 371
         4   CoreFoundation                      0x00007fff8ef9f618 _CF_forwarding_prep_0 + 232
         5   AppKit                              0x00007fff88415e99 -[NSPathCell _otherItemClick:] + 321
         6   CoreFoundation                      0x00007fff8efa211d -[NSObject performSelector:withObject:] + 61
         7   AppKit                              0x00007fff87e0a852 -[NSApplication sendAction:to:from:] + 139
         8   AppKit                              0x00007fff87ef734f -[NSMenuItem _corePerformAction] + 399
         9   AppKit                              0x00007fff87ef7086 -[NSCarbonMenuImpl performActionWithHighlightingForItemAtIndex:] + 125
         10  AppKit                              0x00007fff88192e9c -[NSMenu _internalPerformActionForItemAtIndex:] + 38
         11  AppKit                              0x00007fff880253f1 -[NSCarbonMenuImpl _carbonCommandProcessEvent:handlerCallRef:] + 138
         12  AppKit                              0x00007fff87e710bf NSSLMMenuEventHandler + 339
         13  HIToolbox                           0x00007fff8e26a8ec _ZL23DispatchEventToHandlersP14EventTargetRecP14OpaqueEventRefP14HandlerCallRec + 1263
         14  HIToolbox                           0x00007fff8e269ef8 _ZL30SendEventToEventTargetInternalP14OpaqueEventRefP20OpaqueEventTargetRefP14HandlerCallRec + 446
         15  HIToolbox                           0x00007fff8e280d03 SendEventToEventTarget + 76
         16  HIToolbox                           0x00007fff8e2c7249 _ZL18SendHICommandEventjPK9HICommandjjhPKvP20OpaqueEventTargetRefS5_PP14OpaqueEventRef + 398
         17  HIToolbox                           0x00007fff8e3ae0f1 SendMenuCommandWithContextAndModifiers + 56
         18  HIToolbox                           0x00007fff8e3f45e1 SendMenuItemSelectedEvent + 253
         19  HIToolbox                           0x00007fff8e2c032d _ZL19FinishMenuSelectionP13SelectionDataP10MenuResultS2_ + 101
         20  HIToolbox                           0x00007fff8e3ecfed _ZL19PopUpMenuSelectCoreP8MenuData5PointdS1_tjPK4RecttjS4_S4_PK10__CFStringPP13OpaqueMenuRefPt + 1660
         21  HIToolbox                           0x00007fff8e3ed2ac _HandlePopUpMenuSelection7 + 621
         22  AppKit                              0x00007fff880280bd _NSSLMPopUpCarbonMenu3 + 3860
         23  AppKit                              0x00007fff883cf02e _NSPopUpCarbonMenu3 + 39
         24  AppKit                              0x00007fff88026222 -[NSCarbonMenuImpl popUpMenu:atLocation:width:forView:withSelectedItem:withFont:withFlags:withOptions:] + 322
         25  AppKit                              0x00007fff88203b41 -[NSPopUpButtonCell trackMouse:inRect:ofView:untilMouseUp:] + 564
         26  AppKit                              0x00007fff8841581e -[NSPathCell trackMouse:inRect:ofView:untilMouseUp:] + 1040
         27  AppKit                              0x00007fff87e08786 -[NSControl mouseDown:] + 786
         28  AppKit                              0x00007fff8841ca9e -[NSPathControl mouseDown:] + 376
         29  AppKit                              0x00007fff87dd366e -[NSWindow sendEvent:] + 6280
         30  AppKit                              0x00007fff87d6bf19 -[NSApplication sendEvent:] + 5665
         31  AppKit                              0x00007fff87d0242b -[NSApplication run] + 548
         32  AppKit                              0x00007fff87f8052a NSApplicationMain + 867
         33  SandPath                            0x00000001000017a2 main + 34
         34  SandPath                            0x0000000100001774 start + 52
         35  ???                                 0x0000000000000001 0x0 + 1
    )