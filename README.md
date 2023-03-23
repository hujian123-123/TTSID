# Satellite Image Dataset of Truck Activities (SIDTA)
## Abstract:
we divide the truck trajectory into loading/unloading points、resting points and traveling points , and use point of interest(POI) and area of interest(AOI) data to collect satellite images to create our image dataset.
## Example images:
![example images](https://github.com/hujian123-123/TTSID/raw/main/img/example%20img.png)
## Baseline model test results:
We selected ResNet50, Inception3(Ioffe and Szegedy, 2015), Shufflenetv2 (Ma et al., 2018) as the baseline models.
### Accuracy:
![Accuracy](https://raw.githubusercontent.com/hujian123-123/TTSID/main/img/baseline%20models%20result.png)
### Confusion matrix
![Confusion Matrix](https://raw.githubusercontent.com/hujian123-123/TTSID/main/img/confusion_matrix.png)
## Interpretability analysis:
We used the trained Resnet50 model with Shapley Additive Explanations (SHAP) (Lundberg and Lee, 2017) to analyze the model identification results.
![Interpretability analysis](https://github.com/hujian123-123/TTSID/raw/main/img/Interpretability_analysis.png)
## Instance analysis:
### Truck GPS Data:
Based on the recognition results of ResNet50, we filtered the results by using the thresholds of the front and back points to filter out the truck driving points identified as stopping points, to filter out the results of truck travel points identified as dwell points.
### LU Points:
![lu_points](https://raw.githubusercontent.com/hujian123-123/TTSID/main/img/lu_points.png)
### Rest Points:
![rest_points](https://raw.githubusercontent.com/hujian123-123/TTSID/main/img/rest_points.png)
### Traveling Points:
![traveling_points](https://raw.githubusercontent.com/hujian123-123/TTSID/main/img/traveling_points.png)
## SIDTA:
Download our dataset from [onedrive]()

## Download Google satellite images:
[Google-Map-Downloader](https://github.com/zhengjie9510/google-map-downloader)



