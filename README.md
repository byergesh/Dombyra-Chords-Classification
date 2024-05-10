# Dombyra-Chords-Classification
Classificaiton the 22 classses of Dombyra (Kazakh national musical instrument) chord's sounds into 22 classes with high accuracy. The dataset was collected manually using 3 different dombyra's and different devices for the classification. 


Link to the dataset: 
https://drive.google.com/drive/folders/17pnC6VWnnQk8wr58NKsIX6GmeVf6fGbl?usp=sharing


PCA visualization of classes:
![newplot](https://github.com/byergesh/Dombyra-Chords-Classification/assets/91945196/48c4f61c-782e-4e0b-bd46-384d2d4ae043)


Analysis through MFCC(feature extraction from sound) + Traditional ML models:

  - MFCC+kNN methods with RandomOversamper() with python built in function showed the best results
  - best accuracy ~97%

Analysis through ResNet architecture form pytorch library:
  - Mel Spectrogram Images were extracted from sound files all classes
  - Pretrained resnet18 and resnet50 were used for image processing task
  - The best accuracy were taken using resnet18 architecture (~98%)
![Без названия](https://github.com/byergesh/Dombyra-Chords-Classification/assets/91945196/af7c0e3f-9246-4317-913c-c936fc7ed3d8)
