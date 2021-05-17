# Classification-Hackaton-with-Insurace-Data

Araç Sigortası Satış Tahmin Problemi
Araç sahiplerinin araç sigortası satın almak konusundaki niyetlerinin tespiti sigorta şirketleri için büyük önem taşır. Doğru tahminler sigorta şirketleri için bir iletişim stratejisi planlayarak potansiyel müşterilere ulaşma, iş modellerini ve gelirlerini optmize etme fırsatı yaratır.

Müşterilerine sağlık sigortası sağlayan bir sigorta şirketi bir önceki yılın poliçe sahiplerine araç sigortası satmayı planlamaktadır. Müşterilerin araç sigortası ile ilgilenip ilgilenmediklerini tahmin amacıyla kullanılacak şirket verisi müşterinin demografik bilgilerini (yaş, cinsiyet, bulunduğu il vb), araç özelliklerini (yaş ve hasar durumu) ve poliçe bilgilerini (prim ve kanal bilgileri) içermektedir.

Aşağıdaki tablo veri setinde kullanılan öznitelikleri (features) ve açıklamalarını içermektedir.

Öznitelik	Açıklama
Musteri_no	Anonim müşteri no
Cinsiyet	Müşteri cinsiyeti (E/K)
Yas	Müşteri doğum yılı
Ehliyet	Müşteri ehliyet durumu (Var/Yok)
Sehir	Müşterinin bulunduğu il
Gecmis_police	Müşterinin halihazırda araç sigortası var mı? (Var/Yok)
Arac_yasi	Aracın yaşı (<1 Yıl, 1-2 Yıl, 2-5 Yıl, 5-10 Yıl, >10 Yıl)
Hasar_durumu	Müşteri aracında geçmişte hasar oluştu mu? (E/H)
Yillik_prm	Yıllık prim bedeli
Acenta_no	Satış sorumlusu kod numarası (anonim)
Sure	Sigortalı (sağlık sigortası) olma süresi (gün)
Sonuc	Müşteri isteği (hedef): ilgileniyor (1), ilgilenmiyor (0)
Veri dosyaları
1. Arac_train.xlsx (254687 gözlem, 11 öznitelik, 1 hedef) : En iyi modelinizi seçmek için kullanacağınız eğitim verisi.

2. Arac_test.xlsx (63672 gözlem, 11 öznitelik)

Başarı metriği
Bu hackathon için değerlendirme metriğiniz "ROC_AUC Score" olarak belirlenmiştir.

Hackathon rehberi
DA503 finali için almış olduğunuz Kaggle hesaplarını burada kullanabilirsiniz. Önemli olan Public Leaderboard üzerinde isimlerinizin görünüyor olmasıdır.
Kaggle'a giriş yaptıktan sonra https://www.kaggle.com/t/96ff603c76bb404589d4e4d5c0068be4 linki üzerinden yarışma sayfasını açın.
En iyi çalışan modeli elde ettiğinizde bir tahmin dosyası hazırlayın (örneğin pred.csv gibi) ve Kaggle'a yükleyin. Kullandığınız dosya isminin bir önemi bulunmamaktadır. Ancak bir hata ile karşılaşmamak için dosya formatı kritik öneme sahiptir (bir sonraki maddeyi lütfen dikkatle inceleyin).
Unutmayın, Hackathon süresince 7 kez çözüm dosyası yükleme hakkınız bulunmaktadır.

Kaggle tahmin dosyanızı nasıl değerlendiriyor?
Tahminlerinizi (pred.csv) Kaggle'a 7 kez yükleme hakkınız bulunmaktadır. Çözüm için kullandığınız modellerin hiç görmediği test verisi üzerindeki ROC_AUC performanslarını ancak bu şekilde ölçebilirsiniz. Modelde yapılan değişikliklerin sonuçlarını Kaggle üzerindeki performansınızı takip ederek yorumlayabilirsiniz. Aynı zamanda diğer grupların performansları ve sıralamaları da buradan görünür olacaktır.

Dikkat: Kaggle'da Public Leaderboard altında görünen (ROC_AUC) skorunuz test verisinin yalnızca %40'ı üzerindeki değerlendirme ile sıralamaya alınmaktadır. Hackathon'un nihai sıralaması ancak yarışma tamamlandığında test verisinin geriye kalan %60'ının da değerlendirmeye eklenmesiye (bu kısım sizlere görünür olmayan Private Leaderboard altında tutuluyor) ortaya çıkacaktır.
