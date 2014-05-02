Barcode-Generator
=================

I'm putting this code up mostly as a historical curiosity, but also because it might be useful to somebody. Just be aware that this is old, old, old code.

This was one of my earlier pieces of publicly released Cocoa Code. I started the switch from Mac Toolbox programming to Cocoa with Rhapsody DP3, but it was a slow transition. This project was started almost exactly 12 years to the day before the initial post here on GitHub. The oldest creation dates in the source code are May 1, 2002 and I am posting this on May 2, 2014. 

I have converted this to ARC and corrected all of the errors, warnings, and analyzers issues except for a few deprecations around open/save dialogs that I didn't feel like tackling.

The app was intended to be a test scaffold for a barcode framework. I never got around to creating an actual framework out of the code.

You are welcome to use the code for any uses without attribution or payment. It also comes with no warranty whatsoever. This code was written in the very early days of OS X and a lot has changed. Even if they hadn't, I was still pretty new to Objective-C and there are almost certainly some cases of "you really shouldn't do it like this" in here.

Here's the original README contents:

Cocoa Barcodes is a set of classes (and a test application) for generating two-dimensional barcodes. It supports many of the more common one-dimensional linear barcodes in use today, allows you to export a barcode as a TIFF, EPS, or PDF image, to copy the barcode image to the pasteboard, or to drag it to any other application that accepts standard OS X PDF data from the pasteboard, including TextEdit?. You can also print barcodes directly to any supported printer. Please note that you may not be able to create readable barcodes at all bar widths allowed by a specification. For example, Code 3 of 9 allows a bar width of as small as 7.5 mils, but I haven't had much luck going smaller than 13 mils on ink jet printers.

You have a fair amount of control over the final appearance of the barcode, including the bar width (in 1/10 mil increments), bar height, font size, and captioning. The following barcode types are supported:

Code 3 of 9
Extended Code 3 of 9
Code 128
Interleaved 2 of 5
Industrial 2 of 5
Codabar
PostNet?
Modified Plessey
Modified Plessey (hexadecimal)
UPC-A
UPC-E
EAN-13
EAN-8
Royal Mail Barcode (also known as RM4SCC or CBC)
Planet Barcode
Japan Post Barcode

Cocoa Barcodes is based on Barcode Generator, an open source Mac program which began its life as a test scaffold for a set of Cocoa classes I was writing. I did not initially intend to release it as a standalone program, but by the time I was done testing the code, it had the lion's share of the features available on other OS X barcode programs at the time so I decided to release it.