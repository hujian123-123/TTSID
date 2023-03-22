# Satellite Image Dataset of Truck Activities (SIDTA)
## Abstract:
we divide the truck trajectory into loading/unloading points、resting points and traveling points , and use point of interest(POI) and area of interest(AOI) data to collect satellite images to create our image dataset.
## Example images:
![example images](https://github.com/hujian123-123/TTSID/raw/main/img/example%20img.png)
## Baseline model test results:
### Accuracy:
![Accuracy](https://raw.githubusercontent.com/hujian123-123/TTSID/main/img/baseline%20models%20result.png)
### Confusion matrix
![Confusion Matrix](https://github.com/hujian123-123/TTSID/tree/main/img/confusion%20matrix.png)
## Interpretability analysis:
![Interpretability analysis](https://github.com/hujian123-123/TTSID/raw/main/img/Interpretability%20analysis.png)
## Instance analysis:
### Truck GPS Data:
为过滤掉将卡车行驶点识别为停留点的错误，在识别结果的基础上，采用前后两点的阈值进行过滤。
### LU Points:
### Rest Points:
### Traveling Points:
## SIDTA:
Get our dataset from [onedrive]()

## Download Google satellite images:
[Google-Map-Downloader](https://github.com/zhengjie9510/google-map-downloader)



