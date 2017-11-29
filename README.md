# UIScrollView Paging Autolayout & Storyboard
This sample contains the Auto Layout implementation for UIScrollView with paging enabled. To simplify layout’s complexity for views inside content view this sample uses [Stack View](https://developer.apple.com/library/content/documentation/UserExperience/Conceptual/AutolayoutPG/LayoutUsingStackViews.html).

Introduction
------------

As it's stated in [Working with Scroll Views](https://developer.apple.com/library/content/documentation/UserExperience/Conceptual/AutolayoutPG/WorkingwithScrollViews.html#//apple_ref/doc/uid/TP40010853-CH24-SW1), you can setup ScrollView and its content in Interface Builder by using Auto Layout.

Steps to implement are:

1. Add the scroll view to the scene.
2. Draw constraints to define the scroll view’s size and position, as normal.
3. Add a view to the scroll view. Set the view’s Xcode specific label to Content View.
4. Pin the content view’s top, bottom, leading, and trailing edges to the scroll view’s corresponding edges. The content view now defines the scroll view’s content area.
5. (Optional) To disable horizontal scrolling, set the content view’s width equal to the scroll view’s width. The content view now fills the scroll view horizontally.
6. (Optional) To disable vertical scrolling, set the content view’s height equal to the scroll view’s height. The content view now fills the scroll view horizontally.
7. Lay out the scroll view’s content inside the content view. Use constraints to position the content inside the content view as normal.

Using constraints to position the content inside the content view might bring additional complexity to your layout. With stack view set as a content view each entry inside it will have just one single constraint instead of 5+. The stack view grows longer as the user adds more entries. Scrolling is automatically enabled as soon as there is too much content to fit on the screen.

Pre-requisites
--------------

- xCode 9.+
- iOS 11.+

Screenshots
-----------

<p align="center">
    <img src="https://user-images.githubusercontent.com/23726864/33372793-86268c4a-d4ff-11e7-9bc0-c7159cf6aa4a.gif" 
         alt="A gif illustratrating the way app works" width="324" />
</p>

Getting started
---------------

Check out branch master and then open StackPagingScroll/StackPagingScroll.xcodeproj in xCode.

Support
-------

If you've found an error in this sample, please file an issue: https://github.com/eugenebrusov/ios-stack-paging-scroll/issues

License
-------
```
Copyright (c) 2017 Eugene Brusov

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
