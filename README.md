# Minimum-klid-Mesafesinin-Hesaplanmas-
Python Uygulama 2 / Minimum Öklid Mesafesinin Hesaplanması
Noktaların tanımlanması
Öklid mesafesi fonksiyonunun yazılması
Mesafelerin hesaplanması
Minimum mesafenin bulunması


Açıklamalar:
****Noktaların Tanımlanması:

Python
points = [(1, 2), (4, 6), (5, 9), (2, 1), (7, 8)]
Bu liste, 2D uzaydaki noktaları temsil eden demetler içerir.

***Öklid Mesafesi İçin Bir Fonksiyon Yazma:

Python
def euclideanDistance(point1, point2):
    return math.sqrt((point1[0] - point2[0]) ** 2 + (point1[1] - point2[1]) ** 2)
Bu fonksiyon, iki nokta arasındaki Öklid mesafesini hesaplar.

***Mesafelerin Hesaplanması:

Python
distances = []
for i in range(len(points)):
    for j in range(i + 1, len(points)):
        distance = euclideanDistance(points[i], points[j])
        distances.append(distance)
Bu döngü, listedeki her nokta çifti arasındaki mesafeyi hesaplar ve distances listesine ekler.

***Minimum Mesafenin Bulunması:

Python
min_distance = min(distances)
distances listesindeki minimum mesafeyi bulur.
