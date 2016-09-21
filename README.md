# Camera Widget For PhoneGap

The camera widget enables PhoneGap native camera functionality within your Mendix mobile
application.

## Contributing

For more information on contributing to this repository visit
[Contributing to a GitHub repository](https://world.mendix.com/display/howto50/Contributing+to+a+GitHub+repository)!

## Compatibility
The camera widget functions on the latest versions of both iOS and Android. Windows Phone is
currently not supported. Additionally, v3.0 drops support for Mendix 5 projects. If you wish to include the widget in an older project, please download v2.5 from the versions tab. 

## Offline
In version 3.0, support for offline profiles was introduced. Functionality remains the same in the new offline profile, with the exception that on save microflows and the Autosave setting will trigger an error in the client when enabled.  

## Configuration

Place the widget in a dataview where you want the button to be placed. Make sure this form is
reachable from a mobile application.

### Appearance
#### Image container class
The class that will be set on the image preview container.

#### Width
The width of the image preview.

#### Height
The height of the image preview.

#### Image Location
Where the image preview will be shown relative to the button.

### Button
#### Label
The label text that is shown on the button.

#### Class
An optional class to be placed directly on the button dom node.

### Behaviour
#### On save microflow
An optional microflow that will be triggered when the object is saved.

#### Autosave
Optional setting to auto-save an image to the contextobject. use the on save mf to commit the object
and run further actions.

#### Picture Source
Setting that determines where the image will come from: gallery or the camera.

#### Auto start delay
Delay (ms) before opening the camera/gallery, zero means no auto start.

### Image quality
Be aware that setting this higher will be more taxing and will take longer to upload.  If quality
width and height are both set to `0`, the image will be saved full size.

#### Quality width
The width of the image that is eventually stored and send to the application, between 0 and 100. 
#### Quality height
The height of the image that is eventually stored and send to the application, between 0 and 100.

