## File Format and File Properties
The storage format for SemTalk Online's model files is **SDX** which contains the **Object Model** and the graphics in a **MxGraph in JSON** format. 

Template files saved ib the **STX** format .
Files are stored in a **MongoDB** or in a **SharePoint Library**.

- **Error - File Size**: If a file becomes too large, SemTalk Online functionality may be impaired. Embedded images contribute significantly to the size of the file. The **Image Manager** therefore displays a warning as soon as this size range is reached.

- **Loading Time**: Large models load more slowly.

- **Auto-Save to Local Storage**: Saves the file to the local storage on the user's device after every relevant change. This ensures that the current status is not lost if the application needs to be restarted or updated. 

  Most browser's **Auto Save** only allow a maximum size of 5 MB. If the file exceeds this size, **Auto Save** states can no longer be stored. In this case, users must actively save the file regularly in the DB or Library to avoid data loss.

**Publishing to a Portal**: When a file size of 7 MB is reached, publishing to a portal database becomes critical. If a file size is 10 MB or larger, Portal publishing will fail.
If users receives a warning message regarding the file size, it is recommended to reduce the size of the model or immediately **Publish to a Portal**.