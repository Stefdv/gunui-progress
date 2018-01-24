## GunUi elements
GunUi is a set of webcomponents that enables you - the frontend developer - to build complex - Gun - applications without writing any ( well...almost) javascript

Every gunui- element has just 2 required attributes "soul" and "prop" that will link the element to a certain data-point.

## Purpose of `gunui-slider`
* Visual control a numeric value in your Gun data.
* Syncs the state of the slider with changes in Gun
* ...and then some...Look at the demo

#### Requires [`gunui-base`](https://github.com/Stefdv/gunui-base) in your main document

## But Why?
If you don't fully understand the purpose of gunui take a look at some of the GunUi elements.
* [gunui-button](https://stefdv.github.io/gunui-button/components/gunui-button/demo/index.html) Visual control of a Boolean value in your Gun data
* [gunui-progress](https://stefdv.github.io/gunui-progress/components/gunui-progress/demo/index.html) Visualize a Numeric value in your Gun data
* [gunui-slider](https://stefdv.github.io/gunui-slider/components/gunui-slider/demo/index.html) Visual control of a Numeric value in your Gun data.


## (Bower) Install gunui-slider
( When Polymer 3 arrives we can skip the bower part, but for now...)
```
bower install gunui-slider --save
```

## Your main document
```
<!doctype html>
<html lang="en">
  <head>
    <!-- load Gun from somewhere ( required ) -->
    <script src="my_path_to_gun.js"></script>

    <!-- import gunui-base ( required )-->
    <link rel="import" href="/bower_components/gunui-base/gunui-base.html">

    <!-- import gunui-slider -->
    <link rel="import" href="/bower_components/gunui-slider/gunui-slider.html">

  </head>
  <body>
    <gunui-base></gunui-base>

    <!-- somewhere in your app, or in a custom element -->
    <gunui-slider soul="lights" prop="lights.1.state" key="bri">Light 1</gunui-slider>

  </body>
</html>
```
That's it. No javascript!

You now control the property in Gun!

## Now what?
Now you are ready to start building great apps with Gun but without having to write javascript :). Take a look at all the GunUi elements available.

## Contact
I'm a terrible e-mail reader, so please post any questions in [gitter](https://gitter.im/amark/gun) @Stefdv
