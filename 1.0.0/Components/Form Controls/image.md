## Overview
Image component is used to insert an image into a page.

## Usage
The image in used to display an image in a page. The image has two required attributes: src and alt. 

**Note:** Images are not technically inserted into the page, images are linked to HTML pages. The image  component creates a holding space for the referenced image.

### How to use   
- Drag and drop the component. 
- Double click the component to display the list of attributes that can be used with it.
- Place the images inside the assets editor and save the image inside one of the folders available inside assets editor, and give the path in imgsrc attribute
- Fill the attributes which are needed and save the page.

### Example 
Input the component field with the attribute value:
``` 
imgsrc = /home/prashanth/Documents/neutrinos.png
Alt  = Neutrinos
```
Save it and run.
When the page is loaded "imgsrc = /home/prashanth/Documents/neutrinos.png" will display the image that is specified in the path. And the "alt = Neutrinos" will display the text Neutrinos if the image cannot be loaded or not found.

## Associated Attributes
- **style:** Used to specify the inline style.
- **class:** it specifies one or more class names for an element. The class attribute is mostly used to point to a class in a style sheet.
- **Imgsrc:** The src attribute specifies the URL(web address) of the image. Images should be saved inside assets editor and placed within the folders Android or Materiallcons or Web or iOS folders and the appropriate path should be given.
- **Alt:** THe alt attribute provides an alternate text for an image, if the user cannot view it.

## Support
- **Devices:** Android, iOS
- **Browsers:**  Latest version of all modern browsers
- **Dependencies version:** 
    - Angular CLI version: 5.0.0 + 
    - Cordova version: 7.1.0 +

