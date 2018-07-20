# ClipboardTextBox
Extended Windows Forms TextBox control that lets you handle and override clipboard events.

I got the idea from this [Visual C# Kicks article](http://www.vcskicks.com/clipboard-textbox.php).

## How to use
The ClipboardTextBox control behaves just like the standard Windows Forms TextBox control. 

Three events were added:
  * __TextCopied__ - Occurs when text was copied from the control.
  * __TextCut__ - Occurs when text was cut from the control.
  * __TextPasted__ - Occurs when text was pasted to the control.
  
The __ClipboardText__ property of the __ClipboardEventArgs__ holds the text that was affected by the clipboard action.
  
The events are invoked before the default Windows clipboard messages are sent. This gives you the option to prevent the messages with the __Handled__ property of the __ClipboardEventArgs__.

## Further information
  * [System.Windows.Forms.TextBox Class](https://msdn.microsoft.com/en-us/library/system.windows.forms.textbox(v=vs.110).aspx)
  * [System.Windows.Forms.Clipboard Class](https://msdn.microsoft.com/en-us/library/system.windows.forms.clipboard(v=vs.110).aspx)

