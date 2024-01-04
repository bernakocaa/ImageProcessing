# ImageProcessing
# 1.Normalizasyon ile standardizasyon arasındaki farklar nelerdir?
Normalizasyon: Verileri belirli bir aralığa (genellikle 0 ile 1 arasına) ölçeklemek amacıyla kullanılır. Bu, verilerin orijinal dağılımını korumak istediğinizde tercih edilir. Standardizasyon: Verileri ortalama değeri 0, standart sapması 1 olacak şekilde dönüştürmeyi amaçlar. Bu, verilerin dağılımını merkezileştirir ve standart sapmayı birim yapar.

Normalizasyon: Genellikle veri noktasını minimum ve maksimum değerlere göre normalize etmek için kullanılan formül, (x - min) / (max - min) şeklindedir. Standardizasyon: Veri noktasını ortalama ve standart sapmaya göre standardize etmek için kullanılan formül, (x - mean) / std şeklindedir.

Normalizasyon: Verilerin dağılımını sıkıştırmaz ve orijinal veri aralığını korur. Standardizasyon: Verilerin dağılımını merkezileştirir ve standart sapma biriminde ifade eder.

Normalizasyon: Aykırı değerlere karşı daha duyarlıdır, çünkü minimum ve maksimum değerlere bağlıdır. Standardizasyon: Aykırı değerlere daha dayanıklıdır, çünkü ortalama ve standart sapma kullanılır.

# 2.Bit plane slicing
Bit-plane slicing, görüntü işleme alanında kullanılan bir tekniktir ve bir görüntünün her pikselinin biner tabanındaki değerini, yani her pikselin bitlerini ayrı ayrı incelemek ve işlemek anlamına gelir. Bu işlem, görüntünün farklı bit düzeylerindeki bilgileri analiz etmek, görselleştirmek veya işlemek için kullanılır. Her bir bit düzeyi, görüntünün belirli bir detay seviyesini temsil eder.

# 3.Histogram eşitleme
Histogram eşitleme, bir görüntü üzerindeki piksel yoğunluklarını düzenleyen bir görüntü işleme tekniğidir. Bu teknik, bir görüntünün kontrastını artırmak ve görüntü üzerindeki detayları daha belirgin hale getirmek amacıyla kullanılır. Histogram eşitleme, görüntü üzerindeki piksel değerlerini dağılımı daha dengeli bir hale getirerek gerçekleştirilir.

Bir görüntünün histogramı, piksel değerlerinin dağılımını gösteren bir grafiğidir. Histogram eşitleme işlemi, bir görüntünün histogramını genişleterek, bu dağılımı daha uniform hale getirir. Bu, görüntü üzerindeki piksel değerlerinin tam aralığını kullandığı ve daha geniş bir kontrast aralığına sahip olduğu anlamına gelir.

Histogram eşitleme işlemi aşağıdaki adımları içerir:

Görüntünün histogramını elde et. Kumulatif dağılım fonksiyonunu (CDF) hesapla. Yeniden ölçeklendirme işlemi yaparak yeni piksel değerlerini elde et. Bu işlem sonucunda, görüntü daha yüksek kontrastlı ve daha iyi görünürlüğe sahip olabilir. Histogram eşitleme, özellikle düşük kontrastlı veya düşük aydınlatmalı görüntülerde kullanılarak daha iyi görsel sonuçlar elde etmek için tercih edilen bir tekniktir.

# 4.Contrast stretching
Contrast stretching (kontrast genişletme), bir görüntü üzerindeki kontrastı artırmak amacıyla kullanılan bir görüntü işleme tekniğidir. Bu teknik, bir görüntüdeki piksel değerlerinin dağılımını genişleterek, piksel aralığını daha geniş bir şekilde kullanır. Sonuç olarak, görüntüdeki renk farklılıkları daha belirgin hale gelir, daha fazla detay ortaya çıkar ve genel görüntü kalitesi artar.

Contrast stretching işlemi, görüntüdeki piksel değerlerini bir giriş aralığından belirli bir çıkış aralığına eşleme prensibine dayanır. Bu işlem, özellikle görüntüdeki kontrastın sınırlı olduğu durumlarda veya bir görüntü daha geniş bir dinamik aralığa sahip olması istendiğinde kullanılır.

Contrast stretching işlemi, aşağıdaki adımları içerir:

1.Görüntünün minimum ve maksimum piksel değerlerini belirle. 2.Belirlenen giriş aralığındaki piksel değerlerini, istenen çıkış aralığına genişlet.

# 5.Gamma
Esas itibariyle sinyal işlemenin bir uygulaması olmasına karşılık, bilgisayar bilimlerinde resim işleme alanında kullanılan konulardan birisidir. Bir resmin amiyane tabirle aydınlığını belirlemeye yarayan çarpandır. Kelime bu çarpan için kullanılan grek alfabesindeki γ (gama) sembolünden gelmektedir. Literatürde gama kodlaması (gamma encoding) , gama eğrisi (gamma nonlinearity) gibi kavramlarla da ifade edilmektedir.

En basit anlamda bir değerin üstü olarak gösterilen γ çapanıdır. Bu durumda

x sonuç = (x giriş )γ olarak gösterilebilir. Yani giriş değerinin üssel fonksiyonudur.

Elektrikte bu durum potansiyel farkının üssü olarak gösterildiği için güç kuralı (power rule) olarak da ifade edilmektedir.

Vçıkış = (Vgiriş)γ şeklinde gösterilebilir.

# 6.Ortalama filtresi
Yaygın isimleri; Mean filtering (ortalama filtresi), Smoothing (yumuşatma), Averaging (ortalama), Box filtering (kutu filtreleme).

Ortalama filtresi, görüntüleri yumuşatmanın basit ve uygulanması kolay bir yöntemidir. Diğer bir deyişle, bir piksel ile diğerleri arasındaki değişim miktarını azaltmaktır. Genellikle görüntülerdeki gürültüyü azaltmak için kullanılır.

Ortalama filtresi, bir görüntünün her bir piksel değerini komşularının ve kendisinin dahil olduğu ortalama değer ile değiştirmektir. Bu durum, çevresindekileri temsil etmeyen piksel değerlerinin ortadan kalkmasına yol açar. Ortalama filtresi bir konvolüsyon filtresidir. Konvolüsyon filtreleri çekirdek şablon (kernel) temeline dayanır. Şekilde gösterildiği gibi çoğunlukla 3×3 kare çekirdek şablon kullanılır. Bazı yumuşatma işlemlerinde daha büyük şablonlar (5×5, 7x7 gibi) kullanılabilir. Büyük şablonun tek bir taramadaki etkisine benzer bir etki, küçük şablonun birden fazla geçişi ile de sağlanabilir.

# 7.Gaussian Filtresi
Gaussian filtresi, görüntü işleme alanında yaygın olarak kullanılan bir düzenleme filtresidir. Bu filtre, bir görüntü üzerinde yumuşatma (blurring) işlemi uygulamak için kullanılır. Gaussian filtresi, bir Gaussian fonksiyonunu (normal dağılım) kullanarak bir pikselin etrafındaki piksellerin ağırlıklı ortalamasını hesaplar.

Gaussian filtresi, özellikle gürültüyü azaltmak, kenarları yumuşatmak veya belirli detayları vurgulamak için kullanılır. Gaussian filtresi uygulandığında, piksel değerleri daha yumuşak bir geçişle değiştirilir.

# 8.Sobel Filtresi
Sobel Filtresi, görüntü işleme alanında kenar tespiti (edge detection) amacıyla kullanılan bir filtre türüdür. Sobel filtresi, bir görüntü üzerindeki kenarları vurgulamak ve tespit etmek için dikey ve yatay yönlere özgü iki farklı matris kullanır. Sobel filtresi genellikle gradyan (türev) hesaplamak için kullanılır. Dikey ve yatay kenarları vurgulamak için iki farklı filtre çekirdeği (kernel) kullanılır. Bu filtreler, görüntü üzerindeki piksel değerlerine uygulandığında, türevi alınmış bir görüntü elde edilir. Bu çekirdekler, bir pikselin etrafındaki dikey ve yatay yoğunluk farklarını ölçer. Filtrasyon işlemi sırasında, bu çekirdekler görüntü üzerinde kaydırılır ve her bir pikselin türeviden oluşan yeni bir görüntü elde edilir.

# 9.Blurring operation with Laplace
Laplace operatörü, bir görüntü üzerindeki kenarları belirlemek için kullanılan bir diferansiyasyon operatörüdür. Genellikle kenar tespiti ve görüntü iyileştirme işlemlerinde kullanılır. Ancak, Laplace operatörü doğrudan bir blurring (bulanıklık) işlemi değildir.

Eğer görüntüyü blurlamak (bulanıklaştırmak) istiyorsanız, genellikle bir blurring filtresi veya kerneli kullanılır. Örneğin, Gaussian filtresi, Mean (ortalama) filtresi gibi filtreler kullanılarak görüntüdeki detayları azaltmak ve kenarları yumuşatmak mümkündür.

# 10.Smoothing, sharpening
Smoothing (bulanıklaştırma) ve sharpening (keskinleştirme), görüntü işleme alanında kullanılan iki farklı tekniktir. Her bir teknik, belirli görüntü işleme hedeflerine yönelik olarak kullanılır.

Smoothing (Bulanıklaştırma): Amaç: Gürültüyü azaltmak, detayları yumuşatmak veya görüntüdeki keskin geçişleri düzeltmek için kullanılır. Kullanılan Filtreler: Gaussian filtresi, Mean (ortalama) filtresi, Median (medyan) filtresi gibi düzenleme filtreleri bulanıklaştırma işlemlerinde kullanılır. Uygulama: Bu işlem genellikle görüntüdeki gürültüyü azaltmak veya detayları azaltmak amacıyla kullanılır. Örneğin, bir görüntü üzerinde Gaussian blurring uygulamak, detayları azaltır ve kenarları yumuşatır. Sharpening (Keskinleştirme): Amaç: Görüntüdeki kenarları veya detayları vurgulamak, görüntüyü daha net ve keskin hale getirmek için kullanılır. Kullanılan Filtreler: Laplace filtresi, Gradient filtreleri (Sobel, Prewitt), Unsharp Masking gibi filtreler keskinleştirme işlemlerinde kullanılır. Uygulama: Keskinleştirme işlemi, genellikle bir görüntü üzerindeki kenarları vurgulamak veya görüntüdeki detayları daha belirgin hale getirmek için kullanılır. Bu, özellikle bir görüntünün daha net ve daha belirgin olmasını istediğiniz durumlarda kullanışlıdır.

# 11.Gaussian
Amaç: Gürültüyü azaltmak ve kenarları yumuşatmak için kullanılır. Kullanım: Bir görüntü üzerine uygulandığında, Gaussian filtresi her pikselin etrafındaki piksellerin ağırlıklı ortalamasını hesaplar. Avantajlar: Gürültüyü azaltma yeteneği ve görüntüyü yumuşatma özelliği nedeniyle, kenar tespiti veya detayların vurgulanması gerekmeyen durumlarda kullanışlıdır.

# 12.Salt and pepper
Salt and pepper, bir görüntüdeki gürültü türlerinden biridir. Bu tür gürültü, görüntü üzerinde siyah (salt) ve beyaz (pepper) rastgele piksellerin belirmesiyle karakterizedir. Salt and pepper gürültüsü, genellikle bir sensör hatası, iletim sırasındaki bozulmalar veya diğer çeşitli hatalar nedeniyle oluşabilir. Salt Gürültü: Görüntü üzerinde belirgin beyaz noktaların belirmesiyle karakterizedir. Bu beyaz noktalar, orijinal görüntüdeki piksel değerlerinden daha yüksek bir değere sahiptir. Pepper Gürültü: Görüntü üzerinde belirgin siyah noktaların belirmesiyle karakterizedir. Bu siyah noktalar, orijinal görüntüdeki piksel değerlerinden daha düşük bir değere sahiptir. Salt and pepper gürültüsü, görüntü üzerindeki detayları ve bilgiyi bozar, bu nedenle bu tür gürültülerle başa çıkmak, görüntü işleme uygulamalarında önemlidir. Gürültüyü azaltma teknikleri, median filtresi gibi filtrelerin kullanılması veya istatistiksel yaklaşımlar ile gerçekleştirilebilir.

# 13.Contraharmonic mean
CHM görüntü işleme alanında kullanılan bir filtreleme tekniğidir. Bu teknik, özellikle gürültülü görüntülerde etkili olabilir. Contraharmonic mean, bir piksel değerini çevresindeki piksellerin kuvvet ortalaması ile değiştirmek için kullanılır.

# 14.RGB kullanarak bölütlenme
RGB kullanarak bölütlenme (thresholding), bir renkli görüntüde belirli renk aralıklarını belirleyip bu renklere dayalı olarak bir maske oluşturma işlemidir. Bu işlem, genellikle bir görüntüdeki belirli renk veya renk aralıklarını vurgulamak, izole etmek veya belirli nesneleri ayırt etmek için kullanılır. RGB (Red, Green, Blue) renk modelinde her bir piksel, kırmızı, yeşil ve mavi bileşenlerin kombinasyonu ile temsil edilir. RGB bölütlenme işleminde, genellikle bir renk veya renk aralığına ait bileşen değerlerini belirleyerek, bu renklere ait olan bölgeleri vurgular veya izole edilir.

# 15.Açma - kapama işlemleri
Açma (opening) ve kapama (closing), morfolojik görüntü işleme operasyonlarıdır ve genellikle gürültü azaltma ve nesne tespiti gibi uygulamalarda kullanılırlar. Açma (Opening): Amaç: Açma işlemi, bir görüntü üzerindeki küçük nesne ve ince detayları azaltmak veya kaldırmak için kullanılır. Gürültüyü azaltmada etkilidir. Uygulama: Açma işlemi, genellikle bir görseldeki küçük beyaz nesneleri veya delikleri kapatmak için kullanılır. Operasyon: Önce erozyon (erosion) uygulanır, ardından bu işlemin sonucuna genişletme (dilation) uygulanır. Kapama (Closing): Amaç: Kapama işlemi, bir görüntü üzerindeki küçük delikleri doldurmak veya ince çizgileri birleştirmek için kullanılır. Nesnelerin kontürlerini düzeltmede etkilidir. Uygulama: Kapama işlemi, genellikle bir görseldeki küçük siyah nesneleri doldurmak veya ayırmak için kullanılır. Operasyon: Önce genişletme (dilation) uygulanır, ardından bu işlemin sonucuna erozyon (erosion) uygulanır.
