# Mosaicer
Using OpenCV & Tensorflow Digitize One's face on Video <strong>Automatically</strong>

* Slideshare : http://www.slideshare.net/SuekyeongNam/mosaicer
* Description in Korean: http://www.slideshare.net/seongside/mosaicer-description-korean
* Youtube : https://youtu.be/qifwKGzVR4c


## Requirement
+ Python3 ↑
+ OpenCV 3.1.0
+ Tensorflow 1.2.1
+ PIL 4.1.1
+ dlib 19.6.1
+ Flask (web.py) 0.11.1

## Modules
* Convert
  * Image files to Labeled Binary file
  * Append image files in existing file
* Train
  * Make model by labeled binary files
* Evaluate
  * Classify image by model which is a result of Train
* Mosaic
  * Digitize your video by model
* Web
  * Support above functions on REST API request
* [Mosaic WEB]
  * Use Mosaicer simply by web


## How To Train
<strong>Before RUN you should configure your directory on 'config.py'</strong>

```
1. Put your 32x32 Images on 'Image' folder

2. RUN python binary_convert.py (with label, foldername)

  EX) [python binary_convert.py (1) (foldername)] or [python binary_convert.py (0) (foldername)]

  images with label 1 is digitized by default

  You should do this step twice by different label

3. RUN python train.py
```


## How To
```
1. If you want to digitize one's face on the video

2. Put the video on 'VIDEO' folder

3. RUN python mosaicer.py with your video name

  EX) [python mosacier.py test.avi]

4. WATCH YOUR VIDEO 'result.avi' in video/result folder
```

<strong>Or just Use [Mosaic WEB]</strong>

## [API]


## [REST API]
For Web Module


## License
Mosaicer is released under [MIT License]

[MIT License]: https://github.com/seongahjo/Mosaicer/blob/dev/LICENSE
[API]: https://github.com/seongahjo/Mosaicer/blob/master/API.md
[REST API]: https://github.com/seongahjo/Mosaicer/blob/master/REST_API.md
[Mosaic WEB]: https://github.com/seongahjo/Mosaicer/tree/master/node
