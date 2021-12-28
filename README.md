# TubesTKC

## Overview Jurnal Referensi
Jurnal yang digunakan sebagai rujukan berjudul <a href="https://www.sciencedirect.com/science/article/abs/pii/S0010482521006193">Skin lesion image retrieval using transfer learning-based approach for query-driven distance recommendation</a> bertema Content-based Image Retrieval. Dalam jurnal tersebut, dataset yang digunakan yaitu International Skin Imaging Collaboration (ISIC) 2018 dan 2019. Dataset terdiri dari 7 kelas penyakit kanker kulit diantaranya Melanoma (MEL), Melanocytic nevus (NV), Basal cell carcinoma (BCC), Keratinocytic tumors (AKIEC), Benign keratosis (BKL), Dermatofibroma (DF), dan Vascular lesions (VASC). Feature Extraction yang diterapkan pada jurnal yaitu convoolutional neural network (CNN) dengan model ResNet50. Hasil evaluasi model yang didapatkan antara lain rata-rata presisi, recall dan f1-score dengan nilai 97% Pada dataset ISIC 2018. Sedangkan pada ISIC 2019 menghasilkan nilai rata-rata presisi 76%, recall 70% dan f1-score 72%.

Gambar dibawah menunjukkan hasil image retrieval dari model ResNett50 :

<img width="422" alt="a" src="https://user-images.githubusercontent.com/64589800/147535576-ecd7b521-28d7-4a0d-b133-8716290b7cc4.png">

## Overview Dataset
Dataset yang digunakan merupakan dataset image klasifikasi kanker kulit dari Challenge <a href="https://challenge2018.isic-archive.com/">International Skin Imaging Collaboration (ISIC) 2018</a>. Dataset tersebut terdiri dari 10.015 data gambar dengan 7 kelas penyakit antara lain Melanoma (MEL), Melanocytic nevus (NV), Basal cell carcinoma (BCC), Keratinocytic tumors (AKIEC), Benign keratosis (BKL), Dermatofibroma (DF), dan Vascular lesions (VASC) yang diperoleh dari open source Kaggle. Data gambar tersebut selanjutnya diresize ke ukuran 32 x 32 piksel dengan color RGB.

Berikut merupakan tampilan dataset ISIC 2018 :

![d](https://user-images.githubusercontent.com/64589800/147536091-c66bb788-fe3d-44b0-98d0-ba24a04317e2.png)

## Preprocessing
Tahap pertama preprocessing yakni melakukan resampling dengan metode Random Over Sampler karena dataset yang digunakan merupakan imbalance dataset sehingga jumlah gambar per-kelasnya tidak sama atau tidak seimbang.

Berikut merupakan plot sebelum dan setelah dilakukan resampling :

<img width="300" alt="imbalance" src="https://user-images.githubusercontent.com/64589800/147536301-06fc3a55-e410-4bfc-b994-cb10b6cfb692.png">
<img width="300" alt="balance" src="https://user-images.githubusercontent.com/64589800/147536311-d92cba1b-94c7-41ce-bf72-8b9572d55f3c.png">

