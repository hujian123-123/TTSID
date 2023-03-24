# Satellite Image Dataset of Truck Activities (SIDTA)
## Abstract:
To identify truck activity, we divided the truck trajectory into three types of points: loading/unloading, resting, and traveling points. We collected satellite images for each point using point of interest (POI) and area of interest (AOI) data, creating a dataset of 1000 satellite images for each point type. The images have a resolution of 600x600.
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
A journey of a truck from Chengdu to Shanghai (containing 2000 GIS points) is selected as an example for analysis.
![example_data](https://raw.githubusercontent.com/hujian123-123/TTSID/main/img/example_img.png)
### Method:
Based on the recognition results of ResNet50, we filtered the results by using the thresholds of the front and back points to filter out the truck driving points identified as stopping points, to filter out the results of truck travel points identified as dwell points
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



