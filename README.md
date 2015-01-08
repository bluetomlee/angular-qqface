# AngularJS QQFace filter

> An AngularJS filter for replacing [qqface codes](http://www..com) with actual emoticons

## Installation

The filter is available in a default form on [Bower](http://bower.io) (you will need Bower 0.9 or greater). By default, each emoji is 21x21 pixels. You can install it the usual way:

    bower install angular-qqface

To customise the emoji dimensions, you will need to fork the repository and change the Gruntfile appropriately (if you haven't used Grunt before, I suggest reading the [quick start guide](http://gruntjs.com/getting-started) on their website):


## Usage

Use it just like any Angular filter. Here's some very simple example markup:

```html
<html>
    <head>
        <meta charset="utf-8">
        <link rel="stylesheet" href="emoji.min.css">
        <script src="angular.min.js"></script>
        <script src="qqface.js"></script>
    </head>
    <body ng-app="app" ng-controller="AppCtrl">
        <ul>
            <li ng-repeat="item in items" ng-bind-html-unsafe="message | qqface"></li>
        </ul>
    </body>
</html>
```

## Licensing and Attribution
The AngularJS qqface filter is released under the MIT license as detailed in the LICENSE file that should be distributed with this library; the source code is [freely available](http://github.com/globaldev/angular-qqface-filter).

The filter was developed by [Bluetom](http://liyi.it) during work on [dxy](http://www.dxy.cn/).  Global Personals Ltd have kindly agreed to the extraction and release of this software under the license terms above.