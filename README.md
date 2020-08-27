# DeepLearning-Extract_40_features_from_human_faces
The CelebFaces Attributes (CelebA) Dataset, which is publicly provided by Kaggle, is used as a dataset for extracting the features of a person's face in a video. This dataset contains the following content:
1. 202,599 number of face images of various celebrities
2. 10,177 unique identities, but names of identities are not given
3. 40 binary attribute annotations per image
4. 5 landmark locations

The kaggle address that provides the dataset : <https://www.kaggle.com/jessicali9530/celeba-dataset>  <br>
For an arbitrary photo (090226.jpg) in the dataset, it is possible to extract which of the 40 categories has features. <br>
The feature that the image has is extracted as 1, and the feature that it does not have is extracted as 0. <br>
Because the dataset is large, we build an environment that can use GPUs through Google Colaboratory.<br>
Register the Colaboratory Google service and connect the GPU by linking the account.<br>
The linkage method is detailed in the address below.<br>
<https://blog.naver.com/skyshin0304/221328089139> <br>
You can use the dataset through the kaggle API in Google colaboratory. With this, you can easily use the giga unit data set in google colaboratory without having to download it directly to your computer. <br>
You can freely adjust filter, kernel_size, padding, input_shape, activation, pooling, and dropout to increase network performance. <br>
If the predicted value (preds) is greater than the percentage, you can adjust either 1 (confirmed as having a characteristic) or 0 (confirmed as having no characteristic). <br>
Finally, the bounding box processed image and features are put on one screen and saved locally as a jpg file. <br>
Extract 40 features from human faces using Deep Learning.
result : 

![agroup_feat-2](https://user-images.githubusercontent.com/29560815/72950976-3f236e80-3dd0-11ea-9601-d44e9aa293a9.jpg)

<br>
더 자세한 사항은 ppt를 참조하세요.<br>
See ppt for more details.<br>
