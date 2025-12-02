# Headers and Footers
SemTalk Online allows users to customize Headers and Footers lables for **Model Files** and **Diagrams** background pages.

## Set Up the Background Pages

Since the elements of a background page are based on the Diagram size, it is necessary to set a fixes Diagram size and Orientation. For more information, go to Diagram.
Once a Diagram format has been defined, the Background page, with header and footer information can be activated. 

Go to **Settings - View** and set the Drawing Size settings to **US Letter** and click the **Landscape, Header & Footer and Auto-Complete** checkboxes to the **On** position.

![alt text](images/Header-Footer2.png)

## Background Pages Editor

Customize the **Background Page** in the  **Tools - Customize - Header Footer** pull-down menu. 

![alt text](images/Header-Footer3.png)

Edit the **Background Page Header/ Footer** settings as needed.

![alt text](images/Header-Footer5.png)

## Editing a Background Page

A Background Page consists of several fields that can be dynamically set or set with fixed defaults. Existing fields are listed the Table in the open dialog.

The most important fields are the **Header and Footer** (IDs, page Header and pageFooter). These are pre-defined and must never be deleted as they contain all other elements. They can be edited to adjust the size and/or orientation.

Each field on a Background Page has the following **Properties**:
- **ID**: A unique identifier for the field
- **Field Content**: (only one of the fields may be filled here)
- **Text Field**: Allows information from the model or a diagram to be displayed, e.g., file name, diagram name, comment, page number, or date values. Existing metadata created in the document properties of the file can also be used.
- **Text and TextL**: Language entries available in SemTalk Online can be used to fill fields with content, e.g., as labels for other fields. This has the advantage that when these entries are used, a translation into other languages is also integrated.
- **Image**: A Base64-converted image can be entered here, which is then displayed in the field. Using a converter such as https://base64.guru/converter/encode/image, an image can be converted into a Base64 string and then inserted into the field on the background page.
- **Formatting**
- **Area**: Determines whether the field is displayed in the Header or Footer.
- **Orientation**: Determines how the field is aligned within the area.
- **X and Y**: The detailed coordinates at which the fields are displayed.
- **Width and Height**: Height and width of the field
- **Formatting**: Additional formatting properties can be entered here, e.g., font size, font type, color, etc.