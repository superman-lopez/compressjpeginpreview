# compressjpeginpreview
This quartz filter compresses the JPEG in a PDF, while maintaining usable resolution.  The purpose of this quartz filter is to use it with Apple's Preview.app to quickly reduce the file size of images in PDF's while maintaining legibility.  Apple does have a built-in filter called "Reduce File Size" that has the same purpose, however this filter is too aggressive and converts images to a resolution that is too low.

To install this filter for the currently logged in user, run the below command in Terminal:
```
mkdir -p ~/Library/Filters/ && curl -o ~/Library/Filters/Compress\ Images\ in\ PDF.qfilter https://raw.githubusercontent.com/superman-lopez/compressjpeginpreview/master/Compress%20Images%20in%20PDF.qfilter
```
After this the filter can be used in Preview.app (and other apps that support quartz filters).
1. Open the PDF in Preview.app
2. Select _File_ and _Export..._
3. Choose _Format_ to be _PDF_
4. Choose _Quartz Filter_ to _Compress Images in PDF_
5. Choose your prefered destination and click _Save_


To uninstall simply run:
```
rm ~/Library/Filters/Compress\ Images\ in\ PDF.qfilter
```
