## File Format and File Properties
The storage format for process files in SemTalk Online is SDX. The file contains the SemTalk object model and graphics from MxGraph in JSON format. Template files have the format STX.
The files are stored either in a MongoDB or in a SharePoint library.

*Error message: File size
If a file becomes too large, SemTalk Online functionality may be impaired. Embedded images contribute significantly to the size of the file. 
The image manager therefore displays a warning as soon as this size range is reached.

*Loading times: Large models load more slowly.

*Auto-save to local storage: 
SemTalk Online saves the file to the local storage on the user's device after every relevant change. This ensures that the current status is not lost if the application needs to be restarted or updated. However, most browsers only allow a maximum size of 5 MB for this auto-save. 
If the file exceeds this size, the save states can no longer be stored. In this case, the user must actively save the file regularly in the DB or library to avoid data loss.

*Publishing to the portal: When a file size of 7 MB is reached, publishing to a portal database becomes critical. If a file size is 10 MB or larger, publishing will fail.
If the user receives a warning message regarding the file size, it is recommended to reduce the size or to publish to a portal.