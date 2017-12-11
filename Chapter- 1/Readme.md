# Chapter - 1: Hello Flutter

Let's create the first __Hello Flutter__ Application. By the end of this chapter, we shall be able to display text on the screen.

## 1.0: Setup & Installation

First and foremost we need to install flutter SDK and the development environment. There are detailed instructions provided at flutter home page.  Please see the instructions at https://flutter.io/setup/ 

You may use any editor of your choice to write Dart code, however, if you want a proper IDE, the IDE of choice is IntelliJ IDEA CE with Flutter plugin.

Post setup and installation, the way to create the first app by calling the following'

```
flutter create myapp
```
Please open `lib/main.dart' file and remove all the generated code (if any) to start afresh

## 1.1: The Code Structure

The code structure starts with a `main()` function which loads a widget. For simplicity, we can consider a single widget as a container (visible/invisible), which loads other widgets. 


## 1.2: Hello Flutter 



Everything is a widget in flutter and displaying Text using a Text widget is no difference. However, before we go ahead and display texts on screen, we need to remember a couple of points about the widgets.

Technically, though not differentiated in flutter, we can consider widgets are of two types. 
- One which can act as a container and hold different widgets inside it
- Child widget, which needs a container widget to be present 
 
The text is a child widget and needs a container widget to run. we'll use the widget 'Directionality`  as a container for the same.

The first line of code is about importing the basic material so that we can can call the `runApp()` function which draws the widget.

The function `runApp()` takes a widget, which is created using `new`


