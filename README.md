XnaControl
==========

XnaControl is a wrapper that encapsulates the bits and pieces you need to
create an XNA control inside a WinForms project. It's a self-contained project
with no external dependencies except for MSBuild, XNA, and .NET 4. It is
based on the XNA WinFormsGraphicsSample[1].

Using it is pretty simple: subclass XnaControlBase in your own project and
implement Initialize() and Draw(). While the convention (as per the original
XNA sample this is derived from) is to do your content loading in the
Initialize method, I generally use this in conjunction with a tool that
rebuilds XNA content files (http://github.com/eropple/XnaContent) when the 
content files change so I tend to do most of my loading on the fly.


-Ed Ropple (ed+xnacontrol@edropple.com)

[1] - http://xbox.create.msdn.com/en-US/education/catalog/sample/winforms_series_1
