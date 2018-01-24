#### GunUi elements
GunUi is a set of webcomponents that enables you - the frontend developer - to build complex - [Gun](https://github.com/amark/gun) - applications without writing any javascript.<br>Just link an element to a 'data-point' in your Gun data by setting attributes.<br>
`<gunui-button soul="lights" prop="hall.ceiling">Light</gunui-button>` and you're all set.



## GunUi-Progress
`gunui-progress` is a Gun wrapper around [`paper-progress`](https://www.webcomponents.org/element/PolymerElements/paper-progress/elements/paper-progress)

#### Purpose of `gunui-progress`
* Visual view a Numeric value in your Gun data.
* Syncs the state of the progress with changes in Gun
* ...and then some...Take a look at the demos

#### Requirements
* [Gun](https://github.com/amark/gun) loaded in your main document
* [gunui-base](https://github.com/Stefdv/gunui-base) in your main document

#### (Bower) Install gunui-progress
( When Polymer 3 arrives we can skip the bower part, but for now...)
```
bower install gunui-progress --save
```

#### Your main document
```
<!doctype html>
<html lang="en">
  <head>
    <!-- load Gun from somewhere ( required ) -->
    <script src="my_path_to_gun.js"></script>

    <!-- import gunui-base ( required )-->
    <link rel="import" href="/bower_components/gunui-base/gunui-base.html">

    <!-- import gunui-checkbox -->
    <link rel="import" href="/bower_components/gunui-progress/gunui-progress.html">

  </head>
  <body>
    <gunui-base></gunui-base>

    <!-- somewhere in your app, or in a custom element -->
    <gunui-progress soul="lights" prop="lights.1.state.bri" subscribe></gunui-progress>

  </body>
</html>
```
That's it. No javascript!

You now control the property in Gun!

#### Now what?
Now you are ready to start building great apps with Gun but without having to write javascript :).<br>Take a look at all the GunUi elements available.

### Demos
If you don't fully understand the purpose of gunui take a look at some of the GunUi elements.
#### Property Elements
Element | Demo | Type | Change | Observe | Available
----------- | ------------ | ------- | ---- | ---- | ----
[gunui-button](https://github.com/Stefdv/gunui-button) | [demo](https://stefdv.github.io/gunui-button/components/gunui-button/demo/index.html)| Boolean | :white_check_mark: | :white_check_mark: | :white_check_mark:
[gunui-checkbox](https://github.com/Stefdv/gunui-checkbox) | [demo](https://stefdv.github.io/gunui-checkbox/components/gunui-checkbox/demo/index.html)  | Boolean | :white_check_mark: | :white_check_mark: | :white_check_mark:
gunui-toggle | | Boolean | :white_check_mark: | :white_check_mark: | :soon:
[gunui-progress](https://github.com/Stefdv/gunui-progress) | [demo](https://stefdv.github.io/gunui-progress/components/gunui-progress/demo/index.html) | Numeric | :black_square_button: | :white_check_mark: | :white_check_mark:
[gunui-slider](https://github.com/Stefdv/gunui-slider)|[demo](https://stefdv.github.io/gunui-slider/components/gunui-slider/demo/index.html) | Numeric | :white_check_mark: | :white_check_mark: | :white_check_mark:
gunui-input | | Numeric / String | :white_check_mark: | :white_check_mark: | :soon:
gunui-textfield | | String | :white_check_mark: | :white_check_mark: | :soon:


#### Contact
I am not much of an e-mail reader, but please post issues and questions.<br>
It would speed things up if you notify me in the Gun [gitter](https://gitter.im/amark/gun) @Stefdv
