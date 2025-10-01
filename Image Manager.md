# SemTalk Online and Images

SemTalk Online is designed to use visual information to help people quickly understand what is being represented in the active worksheet. Associated worksheet Stencils show the standard objects specific to the worksheet in use. Core Stencil objects are specific to the methodology in use, but stencils can also contain additional Images that enhance a model's effectiveness. 

![Image Icons in the Stencil](./images/bildermanager/bildschablone.PNG)

Ways to Integrate Images:

* Via external hyperlinks: This is used for images that are stored and uploaded from a central file location. Changes, deletions and access restrictions made to the primary image are propagated to all instances of the image in all models that contain the image. A core benefit of this approach is that external hyperlinks do not affect the size of the model file.

* Via embedded base64-encoded image strings: Images can be permanently integrated into the model file as base64-encoded character strings. Please refer to section: [Convert images to base64](./image-manager#convert-images-to-base64)!
The primary advantage of this method is that the image does not have to be loaded from an external source so it is always immediately accessible to every model user. A disadvantage is that if any changes are made to the image, changes will not be propagated to the other models and model diagrams where the object is used. Additionally, model files can quickly become very large (even too large) if the model contains embedded images. Embedded objects should be used for images that do not change often, images that are specific to individual models and/or those images that cannot be obtained from a reliable external source.

* As unique symbols: Images can be added directly to model diagrams. This makes sense if an image only appears once in the model. 

* Via the Image Manager - an integraded image administration interface: If you are working with many images and, if these images are reused in several places, Image Manager is the best interface for images. All images can be clearly created here and transferred to the file. In this way, several modelers can contribute images and manage them together so that they are available for all modeling needs. 

# Integrating Images as Symbols

This option applies exclusively to images that are to be inserted as hyperlinks.
If an image icon is placed on the drawing sheet, a hyperlink can be easily inserted as text by double-clicking on the name “Image” that the icon was initially given.
Press Enter or click on another location to apply the URL and display the image.

![Bild als Hyperlink am Symbol einfügen](./images/bildermanager/bildurlamsymbol.png)


# Adding Images via the Formatting Dialog

If an image icon is placed on the drawing sheet, you can open the formatting dialog by right-clicking --> Formatting (or Menu Icon-->Formatting). This has an “Image” tab.

![Open Style Format Image Tab](./images/bildermanager/bildformatierung.PNG)

Here, you can either specify an external hyperlink or embed an image file converted to base64. To do this, please refer to the section: [Bilder nach base64 konvertieren](./Bilder-Manager#bilder-nach-base64-konvertieren)!

The image can then be embedded into the file.

If a name for the image is entered in the ID field, the image created can then also be reused in the formatting dialog of other image symbols via the selection box labeled ID.


# Image Manager

## Open Image Manager

The image manager is opened via the menu item Tools --> Customize --> Image Manager.
![BilderManager öffnen](./images/bildermanager/bildermanager.png)

![ImageManager interface](./images/bildermanager/bildermanagercontrol.PNG)

The window that opens will then list all existing images in the file with their names, contents, sizes, and whether they are already saved in the file.
The menu bar offers a wide range of options for working with images.

## Image Manager Menu List

![ImageManager interface](./images/bildermanager/bildermanagermenue.png)

Here, you can either use an external 
* New (+ symbol): Allows you to create a new image in the image manager
* Edit (pencil symbol): Existing images can be edited
* Delete (trash can symbol): Images can be deleted
* Apply to file: If images are to be embedded in the file, they must first be applied to the file and are then ready for use
* Remove from file: Images can be removed from the file. If they are already in use, the corresponding image shape loses its content. You can see whether an image is saved in the file by checking the “File” column in the overview menu of the image manager.
* Export/Import: The configuration from the image manager can be exported or imported so that a set of images can be easily transferred to other model files
A hyperlink can be specified or a base64-converted image file can be embedded. To do this, please reread the section:

## Working With the Image Manager

The Image Manager lists all existing images. However, it should be noted that images created using the Image Manager initially only exist in the Image Manager of the currently open model. To transfer one or more images to the file, select the “Transfer to file” menu item. Only then are the images embedded in the model. This procedure ensures that the images can first be created and checked correctly before they have any effect on the model file. In the same way, the images can then be removed centrally from the file by clicking on “Remove from file” in the menu.
Images that are embedded in the file have a check mark in the File column.
To add a new image or edit an existing one, use the “New” or ‘Edit’ buttons in the menu bar. An image entry always consists of an ID, i.e., a unique name, and the image content in the “Image” field. This can be either a URL or the base64-converted character string of an image.
If many base64-embedded images are used, it is important to keep an eye on the size of the images. The more images are stored in the model file, the larger it becomes, which can lead to longer loading times. Problems can also arise when exporting the model to a publication database if the file becomes too large. For this reason, the file size for export is limited to approximately 10 Mb. SemTalk Online will display a warning message in the Image Manager if the file size exceeds approximately 7 Mb. If you do not intend to export to a publication database, you can ignore the warning.



# Convert Images to base64

To embed an image in a SemTalk Online model, the file must be converted to a base64 string.
SemTalk Online does not offer its own conversion tool for this purpose, but links to a freely accessible one at https://base64.guru/converter/encode/I. Converters from other providers can also be used.

![base64 Conversion](./images/bildermanager/konverter.PNG)

To convert the image, it must first be uploaded to the conversion service, the output format must be set to “Data URI -- data:content/type;base64,” and then the Encode button must be pressed.
The result can then be copied into the “Image” field in SemTalk Online. If the process was successful, SemTalk Online will immediately display a preview of the image in the dialog box.





