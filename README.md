![Logo](screen.png "Logo Title Text 1")

# Generator v2.1.1

Store, explore, share and create FileMaker code

## Getting Started

FileMaker 19 should work now.

- Download or clone or this repository.
- The prepped and **current version** is in the "dist" folder

The development version is in the "source" directory.

### Videos

JSON API and Field Maps
https://vimeo.com/190242455
https://vimeo.com/190256809

Custom Generators
http://youtu.be/EnycrdIHSBQ

Storing things on Disk
http://youtu.be/8-bjvfMV_Jk

## A Dev Tool Toolkit

Under the hood, you will find a collection of custom functions, and techniques that making building a Dev Toolkit like this one possible. Check them out and see what you can do. We hope to inspire people to build on top of Generator and the functions it includes.

## Storing Data In Text Files

A core Generator ideal is that storing this stuff as text files is ultimately better for maintaining, and sharing this type of code. To that end, the "Custom Generators" feature saves everything to disk as soon as you save edits.

The JSON API Explorer doesn't store things automatically on disk but instead makes it easy to export and import Requests.

The Field Maps feature currently doesn't have import and export, nor does store things in text. Its all in the DB. Field Maps seem less shareable, and more transient, but perhaps they should be exportable as well.

We are convinced that anything that might be shared or checked into a Version Control (like GitHub) should be in text. But it's not clear yet which approach is best, Save everything on edit, or just allow export and import. Your feedback is appreciated.

## Contributing

We welcome contributions from the community. That's what this is all about.

FileMaker files don't lend themselves well to Github since we can't do merges and pull requests. That's part of what this project is trying to change. But we can still use Github for issues, comments, and planning.

If you find a bug, please include a copy of the file with a Test that shows the bug in action if you can. Its the best way to get your issues addressed. Bugs that are clearly demonstrated are easily fixed.

If you have a bug fix, please include a copy of the file with the bug fixed. And instructions on where it is.

If you have ideas, please flesh them out in a copy of the file and include it on the issue. Nothing gets an idea across like semi-functional code.

## Roadmap

### Multi Clip Generators and Playback

We think that people will want to create a series of generators that should be "played back" in a certain order. That way you could send somebody a package which would include all the changes that need to be made to a system. Right now this is only supported by having an "order" property in the Generator that could be used to sort all the Generators in a folder in the correct order.

What we don't have yet is a great playback experience. But we think we could get there. Perhaps with a simpler Generator player file, that sucks up a folder full of generator packages and walks a user through those steps.

We hope to get there over time. Again your feedback or examples are appreciated.

### XML Editor with Find and Replace

This will have to be a web viewer app, doable but hard. And you can use text editors now since everything is on disk.

### Extending Field Maps

Right now field maps are sort of coupled to the JSON API explorer. They don't need to be. We should be able to Browse open files and tables and build JSON calcs and parsing script steps.

## Credits

Todd Geist created and designed Generator  
Chiyoko Yoshida of [chiyoFM](http://www.chiyoFM.com) created the Theme  
Nick Orr of [Goya LT](https://www.goya.com.au) provides the amazing and free Base Elements Plugin
