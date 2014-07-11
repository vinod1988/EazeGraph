EazeGraph
=========

EazeGraph is an Android library for creating beautiful and fancy charts. Its main goal was to create a lighweight library which is easy to use and highly customizeable with an "up-to-date"-look.

Currently 4 different chart types are available, which can be viewed below.

__________
<b>IMPORTANT:</b>

This library is not intented for "mathematical" purposes like "achartengine" or "androidplot". It is intented to have a beautiful visual presentation of "user related"-data where only one value is provided and the rest is calculated dynamically.

So for example it's not possible to push 2D-values in the LineChart and let them plot just like in our beloved math lessons.

If you want such functionality either you use one of the libraries I named before or you wait some time until I finished a "mathematical plotting"-chart ;)

Currently BarCharts only support positive values. I will provide this functionality later.

<b>Your Android application should at least use Android API Level 14 in order to use this library!!!</b>

Chart types
===========

- Bar Chart

<img src="https://raw.github.com/blackfizz/EazeGraph/master/imagery/bar_chart.png" width="400px" height="300px" />


- Stacked Bar Chart

<img src="https://raw.github.com/blackfizz/EazeGraph/master/imagery/stacked_bar_chart.png" width="450px" height="300px" />

- Pie Chart

<img src="https://raw.github.com/blackfizz/EazeGraph/master/imagery/pie_chart.png" width="400px" height="420px" >


- Line Chart

<img src="https://raw.github.com/blackfizz/EazeGraph/master/imagery/line_chart.png" width="600px" height="320px" />
<img src="https://raw.github.com/blackfizz/EazeGraph/master/imagery/cubic_line_chart.png" width="600px" height="320px" />


Features
========

- 4 different chart types
- dynamic legend label generation
- possibility to use your own legend labels 
- animations for every chart
- touch interaction for PieChart and LineChart
- various xml attributes for customizing the charts
- and much more


Examples
========

Examples on how to correctly use these charts are either below or you can view the source of the sample app I provided.

If you want to see the library in action, just download the sample APK from the PlayStore:


Including in your project
=========================

Insert in your root project's 'build.gradle' under repositories:

    repositories {
        maven {
            url 'https://oss.sonatype.org/content/groups/public'
        }
    }

and in your android app project folder in the 'build.gradle' under dependencies:

    dependencies {
        compile 'com.github.blackfizz:eazegraph:1.0.9-SNAPSHOT@aar'
    }

That's it. now you are ready to use the library!

Usage
=====

Wiki
====

[Project Wiki][10]

Changelog
=========
**1.0.9**
* fixed bug in BarCharts, when layout size changed and the chart tried to calculate positions for empty elements.

**1.0.8**
* LineChart's value will now set its position the the left of the indicator, if it doesn't fit on the screen
* fixed bug where the LineChart GraphOverlay wasn't updated when new values are imported 

**1.0.7**
* the opening animation can now be opened clockwise or counterclockwise (use attribute "egOpenClockwise"

**1.0.6**
* added possibility to use a custom set inner value in PieChart

**1.0.5**
* added x-axis for Line Charts
* Line Charts now support negative values

**1.0.4**
* added standard value for line chart and the corresponding XML-attributes
* fixed some calculation bugs which caused some displaying errors when a lot of data is inserted
* added clearing methods for Charts
* fixed the legend calculation function

**1.0.1**
* added 'eg' namespace for attributes

**1.0.0**
* initial commit of this library

Contributing
=============

I would love to see people contributing to this project. So just go ahead. If you think you did something amazing and your feature should be implemented in this library, make a pull request! Do not hesitate.

Credit
======

This library was developed for the official YAZIO Android app:

https://play.google.com/store/apps/details?id=com.yazio.android

https://play.google.com/store/apps/details?id=com.yazio.android.pro

License
=======

    Copyright (C) 2014 Paul Cech

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

[5]: https://raw.github.com/blackfizz/EazeGraph/master/imagery/bar_chart.png
[6]: https://raw.github.com/blackfizz/EazeGraph/master/imagery/stacked_bar_chart.png
[7]: https://raw.github.com/blackfizz/EazeGraph/master/imagery/pie_chart.png
[8]: https://raw.github.com/blackfizz/EazeGraph/master/imagery/line_chart.png
[9]: https://raw.github.com/blackfizz/EazeGraph/master/imagery/cubic_line_chart.png
[10]: https://github.com/blackfizz/EazeGraph/wiki
