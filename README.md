## GunUi elements
GunUi is a set of webcomponents that enables you - the frontend developer - to build complex - Gun - applications without writing any ( well...almost) javascript

Every gunui- element has just 2 required attributes "soul" and "prop" that will link the element to a certain data-point.

## Purpose of `gunui-progress`
* Visualizes a changing value in your Gun data as a progress bar.
* Second ( intermediate ) bar can be linked to a second value in Gun
* Syncs the state of the progressbar with changes in Gun
* ...and then some...Look at the [demo](https://stefdv.github.io/gunui-progress/components/gunui-progress/demo/index.html)

#### Requires [`gunui-base`](https://github.com/Stefdv/gunui-base) in your main document

## But Why?
If you don't fully understand the purpose of gunui take a look at some of the GunUi elements.
* [gunui-button](https://stefdv.github.io/gunui-button/components/gunui-button/demo/index.html) Visual control of a Boolean value in your Gun data
* [gunui-progress](https://stefdv.github.io/gunui-progress/components/gunui-progress/demo/index.html) Visualize a Numeric value in your Gun data
* [gunui-slider](https://github.com/Stefdv/gunui-slider) Visual control of a Numeric value in your Gun data.

NOTE: Somehow i can't register gunui-slider to bower ( working on it )

## (Bower) Install gunui-button
( When Polymer 3 arrives we can skip the bower part, but for now...)
```
bower install gunui-progress --save
```
### import
```
  <link rel="import" href="/bower_components/gunui-progress/gunui-progress.html">
```
### Use
```
    <gunui-progress soul="engine" prop="temp">Temp</gunui-progress>
```
That's it. No javascript!

You now have a visual representation of some value in Gun!
## Demo
Take a look at the [demo](https://stefdv.github.io/gunui-progress/components/gunui-progress/demo/index.html)
## Now what?
Now you are ready to start building great apps with Gun but without having to write javascript :). Take a look at all the GunUi elements available.

## Contact
I'm a terrible e-mail reader, so please post any questions in [gitter](https://gitter.im/amark/gun) @Stefdv
