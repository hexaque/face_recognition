# face_recognition
face recognition with python

Uygulamamızı Python 3.9 sürümünde Pycharm idesini kullanarak kodladık. Uygulamanın çalışabilmesi için
import face_recognition
import cv2
import numpy as np
import os
import glob
kütüphanelerini indirilip ideye entegre edilmesi ve import edilmesi gerekmektedir.
pip3 install face_recognition
pip install cmake face_recognition numpy opencv-python
Klasör içerisindeki data/faces kısmına programa tanıtılması istenilen kişinin yüzünün en az 2 adet fotoğrafını eklememiz bu fotoğrafları isimlendirirken ‘berke1.jpg’ ‘berke2.jpg’ şeklinde sınıflandırmamız gerekmektedir. Fotoğrafların uzantısı .jpg olması gerekmektedir. Uzantıyı .JPG şeklinde büyük harfle yazmamız durumunda program hata vermektedir.Bu sebeple küçük harf kullanmalıyız.
data/faces klasörüne yüzlerin tanıtımını yaptıktan sonra uygulamayı çalıştırıp Webcam erişim izni vermemiz gerekmektedir. Webcam penceresi açıldıktan sonra program gerçek zamanlı olarak kamera üzerinden yüz tanıma işlemi yapabilmektedir.
** Program çalıştırıldıktan sonra Webcam penceresinin açılması 15-20 saniye sürebilmektedir. Bunun sebebi fotoğrafları tarayıp öğrenmesinden kaynaklıdır.
