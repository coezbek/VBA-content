
# Application.MailSend Method (Project)

Sends a mail message.


## Syntax

 _expression_. **MailSend**( **_To_**,  **_Cc_**,  **_Subject_**,  **_Body_**,  **_Enclosures_**,  **_IncludeDocument_**,  **_ReturnReceipt_**,  **_Bcc_**,  **_Urgent_**,  **_SaveCopy_**,  **_AddRecipient_**)

 _expression_A variable that represents an  **Application** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
|To|Optional| **String**|The user names of the primary recipients of the message, separated by commas.|
|Cc|Optional| **String**|The user names of the secondary recipients of the message, separated by commas.|
|Subject|Optional| **String**|The subject of the message.|
|Body|Optional| **String**|The main text of the message.|
|Enclosures|Optional| **String**|The file names of one or more files to include with the message. Use the list separator character to separate multiple file names. Do not add space between the list separator and the file name.|
|IncludeDocument|Optional| **Boolean**| **True** if the active project is included in the message. The default value is **True**.|
|ReturnReceipt|Optional| **Boolean**| **True** if a message is sent to the sender when the recipient opens the message. The default value is **False**.|
|Bcc|Optional| **String**|The user names of the message recipients which are not displayed, separated by semicolons. This argument is only supported in Microsoft Project for the Macintosh version 4.0|
|Urgent|Optional| **Boolean**| **True** if the message is given a high priority. This argument is only supported in Microsoft Project for the Macintosh version 4.0.|
|SaveCopy|Optional| **Boolean**| **True** if a copy of the message is saved in the SentItems folder. This argument is only supported in Microsoft Project for the Macintosh version 4.0.|
|AddRecipient|Optional| **Boolean**| **True** if recipients of the message are added to a personal address book. This argument is only supported in Microsoft Project for the Macintosh version 4.0.|

### Return Value

 **Boolean**


## Remarks

If the  **MailSend** method is used without specifying any arguments and there are no existing routing slips, a standard compose mail window appears with the active project as an embedded object. Otherwise, using the **MailSend** method without specifying any arguments prompts whether or not to use the routing slip.

