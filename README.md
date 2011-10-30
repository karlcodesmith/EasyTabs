.NET Title Bar Tabs
===================

.NET Title Bar Tabs is a library that you can add to your .NET WinForms applications (WPF support coming eventually) in order to render a list of tabs in the title bar of the application, similar to Chrome, Firefox, Trillian, etc.  Instead of inheriting from System.Windows.Forms.Form, you inherit from TitleBarTabs.  The base class takes care of the grunt work of rendering the tabs, responding to clicks to activate/close/add/etc. while you simply add TitleBarTab objects to the Tabs collection.  TitleBarTab objects expect their content property to be set to a Form object that represents the contents for the tab.  You can design these forms in Visual Studio the same as you would any other application; the Title and Icon properties are used to display the tab itself.

The library comes with a renderer for Chrome-like tabs (ChromeTabRenderer), but you can implement your own by creating a class inheriting from BaseTabRenderer.

Bear in mind that this is very early code.  Things like tab reordering, tearing, and more advanced graphical effects have not been implemented yet.  You are welcome to poke around the code and submit patches, but just remember that this is alpha-quality code.