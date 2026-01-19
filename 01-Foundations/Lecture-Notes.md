# Computer Vision Lecture Notes: 
FoundationsModule: 01 - Foundational Image ProcessingTopic: Digital Image Representation & OpenCV BasicsSource: Master School Curriculum💡 Core ConceptsBu bölümde bilgisayarlı görünün temel yapı taşlarını ve görüntülerin dijital ortamda nasıl temsil edildiğini not alıyoruz.1. Digital Image RepresentationPixels & Resolution: Bir görüntünün en küçük birimi ve yoğunluğu.Color Channels: * RGB: Red, Green, Blue (Standart).BGR: OpenCV'nin varsayılan okuma formatı.Grayscale: Işık yoğunluğu (0-255).2. Mathematical FoundationsGörüntü işleme aslında matris operasyonlarıdır. Bir görüntüyü $f(x, y)$ fonksiyonu olarak tanımlayabiliriz:$x, y$: Piksel koordinatları.$f$: O koordinattaki yoğunluk (intensity) değeri.🛠️ Key Operations & Code SnippetsDers sırasında öğrendiğimiz en kritik OpenCV fonksiyonları:Pythonimport cv2
import numpy as np

# Image Reading & Display
img = cv2.imread('path/to/image.jpg')
cv2.imshow('Display Window', img)

# Color Space Conversion
gray_img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

# Image Resizing
resized = cv2.resize(img, (width, height))
🚀 Key Takeaways (Önemli Çıkarımlar)[ ] OpenCV'nin resimleri BGR olarak okuduğunu asla unutma (Matplotlib ile görselleştirirken RGB'ye çevir).[ ] Görüntü filtreleme (Blurring) aslında bir Convolution (evrişim) işlemidir.[ ] Kenar algılama (Edge Detection) için pikseller arasındaki gradient (türev) değişimlerine bakılır.🔗 Resources & ReferencesMaster School Course MaterialsOpenCV 