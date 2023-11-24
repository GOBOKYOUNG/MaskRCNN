# 오픈소스 과제 1 - Mask R-CNN(202112867 고보경)

1. anaconda에서 가상환경 생성(python 3.7)

 ```
conda create -n MaskRCNN python==3.7
conda activate MaskRCNN
```

2. mask rcnn  다운
   
```
git clone https://github.com/matterport/Mask_RCNN
```

3. keras 2.1.2
```
pip install keras==2.1.2
```

4. pip install tensorflow-gpu==1.15.5
```
pip install tensorflow-gpu==1.15.5
```

5.다음과 같이 폴더를 만든다.
Mask_RCNN -> model -> balloon -> datasets

6. 1) https://github.com/matterport/Mask_RCNN/releases/download/v2.1/mask_rcnn_balloon.h5  
   2)  https://github.com/matterport/Mask_RCNN/releases/download/v1.0/mask_rcnn_coco.h5
       다운 받은 후 Mask_RCNN 폴더로 복사
   3)  https://github.com/matterport/Mask_RCNN/releases/download/v2.1/balloon_dataset.zip
      파일을 다운받아서 Mask_RCNN/model/balloon/datasets 폴더에 해제

7.다음의 명령어로 설치
```
pip install scikit-image
pip install -U scikit-image==0.16.2
pip install protobuf==3.20.*
```

8. samples/balloon  폴더로 이동한 뒤 다음의 명령어로 inference 실행
```
python balloon.py --dataset ../../model/balloon/datasets --weights ../../mask_rcnn_balloon.h5 --logs ../../model/balloon/logs --image ../../model/balloon/datasets/val/3800636873_ace2c2795f_b.jpg splash
```

8번에서 이미지 변경 후 실행




# 실행결과

-inference할 이미지

![16335852991_f55de7958d_k](https://github.com/GOBOKYOUNG/MaskRCNN/assets/113632026/baf06667-f177-4f62-891b-b958247ee8b2)

-inferernce 결과 이미지

![splash_20231124T200628](https://github.com/GOBOKYOUNG/MaskRCNN/assets/113632026/812e5c86-1567-4479-bd8e-fab467de35e6)


