# tello-drone-face-tracking
Bu Python kodu, DJI Tello dronunu yüz takibi yapmak için kullanmanızı sağlar. Dronun kamera görüntüsünde bir yüz tespit edilir ve dron, yüzü takip eder. Bu proje, OpenCV ve DJITelloPy kütüphanelerini kullanarak yüz tanıma ve drone kontrolü sağlar.

## Gereksinimler
- Python 3.x , OpenCV (cv2 kütüphanesi) , NumPy , DJITelloPy gerekli kütüphaneleri yükleyin.
- Tello dronunuzun Wi-Fi aracılığıyla bilgisayarınıza bağlı olduğundan emin olun.

## Kod Açıklaması
- findFace(img): Görüntüdeki yüzleri tespit eder ve yüzlerin koordinatlarını ve alanlarını döndürür. haarcascade_frontalface_default.xml dosyası yüz tespiti için kullanılır.
- trackFace(info, w, pid, pError): Tespit edilen yüzün konumuna göre dronu hareket ettirir. Yüzün ekranın ortasında kalmasını sağlar.
- cap = cv2.VideoCapture(0): Kameradan görüntü alır. Bu, dronun kamerasından gelen görüntüyü alır ve işleme alır.
- Döngü: Dronun kamerasından alınan görüntü sürekli olarak işlenir, yüz tespit edilir ve takip edilir.

## Kullanım
- haarcascades dosya yolunu doğru verdiğinize emin olun.
- facetracking.py dosyasını çalıştırın.
- Dronu kontrol etmeye başlamadan önce dronu kalkış yapacak şekilde konumlandırın.
- Program çalışırken, dronun yüzü takip ettiğini ve yüzün ekranın ortasında kalmasını sağladığını göreceksiniz.
- Programı durdurmak için " q " tuşuna basın. Bu, dronu inişe geçirecektir.

## Video
Dronun yüz takibi yaparken çalıştığı  ekran kaydını aşağıdaki bağlantıdan izleyebilirsiniz:

https://github.com/user-attachments/assets/84c536b5-35d3-4f00-9158-275bf4a1ed12


## Yararlanılan Kaynaklar
 [Tello Drone Python Programming Tutorial | OpenCV](https://www.youtube.com/watch?v=LmEcyQnfpDA&t=522s&pp=ygUSdGVsbG8gZHJvbmUgY29kaW5n)
