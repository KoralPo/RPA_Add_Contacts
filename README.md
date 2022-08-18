# RPA_Add_Contacts
Automatic process in UiPhat which add contacts to Outlook, according to the Excel file.
The process is written in a generic way and provides an answer even in the case of data and a different number of contacts.
For the challenge only the following basic commands were used: 
Use Application/Browser, Click, Keyboard Shortcuts, Type Into, Get From Clipboard, If, Assign, Terminate Workflow, Excel Application Scope, Read Cell, Invoke VBA.

Workflow:

1. For each contact, the process will save their full name, email address and phone number in Outlook.
2. A search of each of the contacts on the Google.com website (this is only a search and the search results have no meaning).
3. In the contact card in Outlook, in the Job title field one of the following options was written: 
   "Does not exist in Google" || "The phone in Google is compatible" || "The phone in Google is not compatible".
4. The Flow selects the correct option by comparing the data in column D with the data in column E in the Excel file.
5. Finally enter the current date and time in the "Done On" cell, using the Invoke VBA command.


