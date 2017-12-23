# Chapter - 2: Creating Application Layouts

A full-fledged app requires many things like an application bar, menu items, and a display area to name a few. We can use widgets to create those or can use the existing layout widgets provided by flutter. 

One such way to create a layout is `MaterialApp Widget`.  

## 2.0: Using MaterialApp

MaterialApp` helps in creating Material Design Application. It not only helps in creating Material Specific design but manage and set up `routes` which enables multi-page applications

The material design is mainly build using 'Scaffold` which provide basic app elements like `AppBar` and a `body`.As the name suggests, the `AppBar` creates an application bar and the `body` contains the large display area. 

Here is our first example of `MaterialApp`  where the widgets are arranged like this

![](https://github.com/DakshHub/Flutter_MobileApp_Development/blob/master/Chapter-%202/Chapter%202-0.png)

and here is how our code for `widget class MyApp`  looks like

```
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return new MaterialApp
    (
      title: "MyApplication",
      home: new Scaffold
      (
        appBar: new AppBar
        (
          title: new Text("My ToDo Application"),
        ),
        body: new Text("Display Area"),
      ),
    );
  }
} 

```

## 2.1: Displaying Multiple Widgets

Till now we have seen that all widgets take only one child, but this is not sufficient in full-fledged applications especially in `Scaffold body`. Even a minimalistic application will have to use multiple widgets

In Flutter, there are widget containers which take the array of widgets and those are used for displaying more than one items in widgets. The prominent containers are 'Row` and `Column`

Let's display multiple items in display area using `Column`, the arrangement of widgets shall look like

~[](https://github.com/DakshHub/Flutter_MobileApp_Development/blob/master/Chapter-%202/Chapter%202-1.png)

And the code changes as 

```
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return new MaterialApp
    (
      title: "MyApplication",
      home: new Scaffold
      (
        appBar: new AppBar
        (
          title: new Text("My ToDo Application"),
        ),
        body: new Column
        (
          children: <Widget>
          [
            new Text("Display Text - 1"),
            new Text("Display Text - 2"),
            new Text("Display Text - 3"),
          ],
        )
      ),
    );
  }
} 

```

