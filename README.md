# parking-lot-demo-custom-vision

Demo for determining occupied parking spots using Azure Custom Vision.

| Input Image | Detection Results |
| ------------- |:-------------:|
| ![Alt text](doc/input.jpg)| ![Alt text](doc/output.jpg) |


# Instructions

1. Sign up for [Custom Vision](https://www.customvision.ai) 
1. Run the notebook
1. Goto the [Custom Vision Settings](https://www.customvision.ai/projects#/settings) and copy/paste the `Training Key` and `Prediction Key` to the notebook in the first cell:

```python
training_key = "xxxx"
prediction_key = "xxxx"
```

# Known limitations

For best detection results, make sure that the cars are not too small in the images. Otherwise, Custom Vision might miss them or detect a lot of misclassifications, as shown in this image (cars on the left were not detected, or very inaccurately):

![Alt text](doc/too_small.jpg)