# Eulerian Video Magnification
EVM in TouchDesigner. Works with the free Non-Commercial license. Runs in real time.

![Watch the video](https://raw.githubusercontent.com/tschnz/TouchDesigner-Projects/master/EulerianVideoMagnification/EVM_Banana.gif)
_Motion magnified banana. Left is the original, rotated around the center of the image 3 times a second by 0.2px, right is the motion magnified version._ 

You can find this validation in the .toe - the .tox holds only the EVM Base Comp.

---
Options
---
 - __Amplification__: How strong movements are magnified
 - __Spatial Cutoff Delta__: High value prevents small details (like noise) from being magnified 
 - __Low/High Frequency in %__: Low value should always be < High value. The higher the values the more fast movements are magnified. The lower the more slow movements are magnified
 - __Color Attenuation__: Color correction. Multiplication factor for color channels (a*&b* from [CIE-L*a*b*](https://de.wikipedia.org/wiki/Lab-Farbraum))

---
Source
---
Math equations and logic derived from my old QT/C++ project [Live Video Magnification](https://github.com/tschnz/Live-Video-Magnification).


Originally proposed by [Wu et al. (MIT)](https://people.csail.mit.edu/mrub/evm/). Algorithm to magnify/enhance motion in _"videos that are difficult or impossible to see with the naked eye and display them in an indicative manner"_.

Watch their supplemental video:
[![Watch the video](https://i3.ytimg.com/vi/ONZcjs1Pjmk/maxresdefault.jpg)](https://www.youtube.com/watch?v=ONZcjs1Pjmk)