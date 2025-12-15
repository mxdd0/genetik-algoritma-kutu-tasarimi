# Genetik Algoritma ile Kargo Kutusu Optimizasyonu (Senaryo 6)

Bu proje, BLG-307 Yapay Zeka Sistemleri dersi kapsamında hazırlanmıştır.

**Öğrenci:** [Bahadır Beldek]  
**Numara:** [2112721066]

Proje Tanımı
Bir e-ticaret firması için, hacmi maksimize ederken malzeme maliyetini minimize edecek **optimum kargo kutusu boyutlarını (genişlik ve yükseklik)** Genetik Algoritma kullanarak bulmayı amaçlar.

Seçilen Senaryo: Senaryo 6
* **Amaç Fonksiyonu:** `y = x1*x2 - 0.1*x1^2 - 0.1*x2^2`
* **Değişkenler:**
    * x1 (Genişlik): [10, 40] cm
    * x2 (Yükseklik): [5, 20] cm

### Kısıtlar (Constraints)
1.  **Raf Sınırı:** `x1 * x2 <= 600`
2.  **Minimum Genişlik:** `x1 >= 15`

Kullanılan Yöntemler
Projede Python dili ve aşağıdaki Genetik Algoritma mekanizmaları kullanılmıştır:
* **Popülasyon:** 50 Birey
* **Seçilim (Selection):** Turnuva Seçimi (Tournament Selection)
* **Çaprazlama (Crossover):** Tek Noktalı / Karışık Çaprazlama
* **Mutasyon (Mutation):** Rastgele değer atama (%10 oranında)
* **Ceza Yöntemi (Penalty):** Kısıtları sağlamayan bireylere çok düşük puan (-9999) verilerek elenmeleri sağlanmıştır.

Kurulum ve Çalıştırma
1.  Bu repodaki `.ipynb` uzantılı dosyayı indirin.
2.  Google Colab üzerinden veya Jupyter Notebook ile dosyayı açın.
3.  Tüm hücreleri sırasıyla çalıştırın.

Sonuçlar
Algoritma sonucunda kısıtları sağlayan en iyi x1 ve x2 değerleri bulunmuş ve gelişim grafiği çizdirilmiştir.
