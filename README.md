# ras2las
### Well log digitalization
a.k.a. the young and the ras2las. Started at the [geophysics hackathon before SEG 2017 annual meeting](https://agilescientific.com/events/2017/9/22/geophysics-hackathon)
put on by Agile Scientific. [Slides here](https://docs.google.com/presentation/d/1wCs5e6a0eNdaXZ--Iemo0zXMd5kPOTUDpSpMWiUIE_c/edit?usp=sharing)

The intention was to adapt [scatteract](https://github.com/bloomberg/scatteract) to well logs but this effort is stopped.


#### Goal:
Web app to digitize well logs.
Input PDF --> output LAS

#### Contributors:
+ [Diego Castaneda](https://github.com/dfcastap)
+ Lanre Aboaba
+ [Chance Sanger](https://github.com/chancesang)
+ [Suman Gautam](https://github.com/sgotham)
+ [Will Sanger](https://github.com/willsa14)

#### Dependencies (partial list)
+ Tensorflow
+ Google Vision service (for OCR)
+ Wand (for reading PDFs)
+ [welly](https://github.com/agile-geoscience/welly) and lasio (for handling .las format well logs)

#### Needs:
+ More open training datasets with both raster and .las.
+ Work on the key components, firstly:
  + Picking curve with CNN
  + Scaling curve picks based on axes labels
    + Method to reject bad axes label picks
