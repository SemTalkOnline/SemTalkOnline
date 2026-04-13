# Header and Footers

SemTalk Online allows you to customize headers and footers for model files and model pages. In SemTalk Online, this is collectively referred to as a **Background Page**.



## Setting up Background Pages

Since the elements of a background page are based on the drawing sheet size, it is necessary to set the drawing sheet size and orientation. For more information, see Wiki page: Drawing Sheet Format



Once a **Diagram** background format is defined, the Diagram background can be edited by checkingticking the **Header & Footer** checkbox to the on position in **Settings** (the gearbox Icon to the far right of the Pull-Down Menu).


SemTalk Online provides a sample background Diagram page that includes the **Diagram** name and **SemTalk logo** in the **Header**.


## Background Page Editor

The **Header and Footer Editor** is used to customize background pages to meet organizattional requirements. **Headers and Footers** each have there own editors located in **Tools -  Customize - Header/Footer Background Page**. This is where all existing background pages are listed. Users can either select an exisiting template or they can define a new template.

**Background Pages** are defined in three possible ways:

**Model Files**: Listing background pages that have been previously saved. These templates can be opened, modified, and saved back to the file.

**Cookies**: Local default **Background Page** settings that can be used as a basis for creating a background page. **NOTE**: When working on a Background page, the current version is always stored as a local Cookie on the user's computer.

**Database (when using MongoDB)**: Background pages can be stored in MongoDB if the user is logged in as an **Administrator**. These can then also be used by all other users for their model files. Double-click on one of the entries or click to select the desired **Background Page**.

If no **Background Pages** exist in the **File or Database**, the **Background Page** in the user’s **Cookies** is automatically opened. In this case, there is no separate **Start Page**.

**Creating and Editing a Background Page in an Open Dialog**: Background pages can be created, edited, deleted, exported, imported, and reset to their default state by selecting **Start** to opens the existing overview page.

**Editing Individual Components of a Background Page**:
Background Pages consists of several display fields that can be populated dynamically or defined with fixed values. Existing fields are listed as a table in the open Diagram.

**Core Header and Footer Settings** (IDs pageHeader and pageFooter). These are predefined components and must not be deleted, as they contain all other elements. They can be edited to adjust their size or orientation. 

For example.
Each field on a background page has a set of properties.

## Header and Footer Properties

**ID**: A unique identifier for the field
Field content: (only one of the fields may be filled here)

**Text**: Enables the display of information from the Model or a Diagram, e.g., File Name, Diagram Name, Comment, Page Number, or Date. 

Also existing document property metadata can also be used.

**Text and TextL**: Language entries available in SemTalk Online can be used to populate fields with content, e.g., as labels for other fields. This has the advantage that using these entries also integrates a translation into other languages.

**Image**: A Base64-encoded image can be entered here, which will then be displayed in the field. Using a converter such as https://base64.guru/converter/encode/image, an image can be converted into a Base64 string and then inserted into the background page field.

## Formatting:

**Area**: Determines whether the field is displayed in the Header or Footer.

**Orientation**: Determines how the field is aligned within the area.

**X and Y**: The detailed coordinates where the fields are displayed.

**Width and Height**: Height and width of the field

**Formatting**: Additional formatting properties can be entered here, e.g., for font size, font, color, etc.

The edit dialog can be opened either by selecting an existing entry and then clicking the pencil icon in the menu, or by using the + button to create a new entry.

**Applying a Background Page to a File**:
**Background Page** are displayed directly on the **Diagram's** drawing sheet. This setting is only found in the user's modeling environment. 

If the Background Page should be applied to all users who open the file, select **Apply to File** in the **Background Pag** menu entry. The newly configured **Background Page** is then applied to the **Model File** and is permanently viewed by all users.


**Background Page Settings** can also be used to import or export settings in JSON format or to reset the settings to its default state.

### Example of a Background Page

Creating and configuring a background page can be relatively complex so it may be necessary to experiment until the desired result is achieved.



The following example illustrates how different fields interact and to show how they can be positioned.

Right mouse click on the open Diagram and click on the Settings Icon ![alt text](images/SettingsIcon3.png). The **Diagram - Settings - View** menu contains the majority of the **Text Font Settings**. **File - Document Settings Pull-Down Menu** contains **Page Options** (e.g. A4, Landscape etc.) in the **Setting - View - Pull-Down Menu**. Click the **Header & Footer** checkbox.Default setting will appear below. If Logos are assigned, they will appear in the right corner. The **Footer** and **Page Number** will be inserted along with any assigned descriptive fields such as the **Last Modification Date** and **Comments**.

**IDs pageHeader and pageFooter** contain the settings for all other fields.
**Footers** are generally smaller than **Headers**. Select the row with the **ID pageFooter** and click on the **Pencil Icon** to edit. Change the **Height** field to 40 and select **OK**.

A field labeled **Page** will be inserted. Create a new entry by selecting the **+** icon. An unique **ID** will be assigned and the position of the new entry will be set. The field should be located in the top-left corner of the **Footer** with the orientation set to **Left**. 

**X and Y** fields are used to perform precise pixel-level positioning within the **Footer**. T default values are set to **0** and **0**. The **Width** is set to accomodate the length of the text. 

In the shown example, the **Width** is set to 100 and the **Height** is set to 40 so that it matches the settings for the **Footer**. The the field text should be set in the **Page** option. Either type the text directly into the field or select the text value **Page** from the pull-down list. 

SemTalk Online contains these option and allows them to be set for multiple languages. Options can also be reused for **Background** pages. Click **OK** to save the new **Settings**.

Actual **Page Numbers** should be inserted usong the **+** icon. Select the position to match the position shown above. Click on the **X** icon and set the coordinate to 100 to match the settings of the **Field Width**. The new **Page Number** field will be placed directly behind the first field. Set the width of the new **Page Number** field to 50 since the **Page Number** field requires less space. 

Select **Diagram: Outline** in the **Text Pull-Down** menu to see the page number of the current **Diagram**. If a **Page Number** does not appear, **Diagram Page Numbers** have not yet been numbered. Add **Diagram Page Numbers** in the **Diagram - Reindex** pull-down menu. 

This menu will also show the internal identifier will also appear in the text field. In the selection box, it looks as follows:
The 3 highlighted entries are the ones that must be selected for steps 4, 5, and 6.
Click OK to complete the process.
The last modification date is created in the same way. The X coordinate must be set to 150 this time, since the two previous fields together total a width of 150, and the width can again be set to 100. In the text field, select “Document: Modified.”

Click OK to complete the process again.
The last field should contain a comment from the diagram’s properties. Therefore, “Diagram: Comment” is selected. The X coordinate must be set to 250, and the length is set to 800 this time so that a sentence fits in the field.

The background page is now complete. The example can be retrieved as a JSON file and imported in the header and footer dialog.
As a tip for positioning, it is recommended to work with borders during creation. In the Formatting field, the strokeColor attribute can be set to black (strokeColor=black;) to create a black border around the field. This can be helpful when arranging individual fields to see the exact size and position on the drawing sheet. At the end of the work, the border can then be removed again.
  