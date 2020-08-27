# DeepLearning-Extract_40_features_from_human_faces
영상 속 인물의 얼굴 속 특징 추출을 위한 데이터셋으로 Kaggle에서 public으로 제공하는 CelebFaces Attributes (CelebA) Dataset을 쓴다. 이 데이터셋은 다음과 같은 내용을 담고 있다.
 
1. 202,599 number of face images of various celebrities
2. 10,177 unique identities, but names of identities are not given
3. 40 binary attribute annotations per image
4. 5 landmark locations

해당 데이터셋을 제공하는 kaggle 주소 : <https://www.kaggle.com/jessicali9530/celeba-dataset>  <br>
데이터셋에 들어있는 임의의 사진(090226.jpg)에 대해서 40가지의 카테고리의 특징 중 어떤 것을 갖고 있는지 추출할 수 있다. <br>
해당 이미지가 갖고 있는 특성은 1, 갖고있지 않은 특징은 0으로 추출된다. <br>
데이터셋이 크기 때문에, Google Colaboratory를 통해 GPU를 쓸 수 있는 환경을 구축한다.<br>
Colaboratory 구글서비스를 등록하고 계정을 연동하여 GPU를 연결한다.<br>
GPU가 제대로 연결되면 다음의 코드를 입력했을 때 /device:GPU:0이라고 뜬다.<br>
연동 방법은 아래 주소에 자세히 나와있다.<br>
<https://blog.naver.com/skyshin0304/221328089139> <br>
Google colaboratory에서 kaggle API를 통해 데이터셋을 사용할 수 있다. 이를 이용하면 기가 단위의 데이터셋을 컴퓨터에 직접 다운받지 않아도 google colaboratory에서 간편하게 사용할 수 있다. <br>
filter, kernel_size, padding, input_shape, activation, Pooling, Dropout 등을 자유롭게 조정해서 네트웤의 성능을 높일 수 있다. <br>
예측값(preds)가 몇퍼센트 이상이면 1 (해당 특징을 갖고 있다고 판정) 아니면 0 (해당 특징을 갖고 있지 않다고 판정)할지 조정할 수 있다. <br>
최종적으로 bounding box처리된 이미지와 특징들을 한 화면에 담아 jpg파일로 로컬에 저장한다. <br>
Extract 40 features from human faces using Deep Learning.
result : 

![agroup_feat-2](https://user-images.githubusercontent.com/29560815/72950976-3f236e80-3dd0-11ea-9601-d44e9aa293a9.jpg)
