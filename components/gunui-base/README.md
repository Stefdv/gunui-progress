#### GunUi elements
GunUi is a set of webcomponents that enables you - the frontend developer - to build complex - [Gun](https://github.com/amark/gun) - applications without writing any javascript.<br>Just link an element to a 'data-point' in your Gun data by setting attributes.<br>
`<gunui-button soul="lights" prop="hall.ceiling">Light</gunui-button>` and you're all set.

## GunUi-Base
`gunui-base` is required by all gunui elements but has no visual appearance by itself.

#### Purpose of `gunui-base`
* main element for all 'gunui-' elements.
* Setup Gun by providing attributes ( `<gunui-base peers="">`)
* makes sure that every gunui- element has the required properties and methods.
* Creates global nameSpace 'GunUi' where 'GunUi.gun' will be the global Gun instance
* ...and then some...we'll get to that when using the elements

<b> Without `gunui-base` none of the gunui elements will work!

<b> You should use `gunui-base` only once and place it in your main document!

#### (NPM) Install Gun
'Gun' is not provided as bower module so we'll have to use NPM.

```
npm install gun
```

#### (Bower) Install gunui
( When Polymer 3 arrives we can skip the bower part, but for now...)
```
bower install gunui-base --save
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
  </head>
  <body>
    <!-- place gunui-base -->
    <gunui-base peers=` "http://gunServer1/gun","http://gunServer2/gun" '></gunui-base>
  </body>
</html>
```
That's it.

<b>NOTE:<br>
Gun is available as 'GunUi.gun'</b>

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
