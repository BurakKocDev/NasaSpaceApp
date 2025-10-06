# NasaSpaceApp
uygulama demo videosunu buradan izleyebilirsiniz:
https://youtu.be/sWxy0WPtT_A

NASA’nın açık kaynak Kepler, TESS ve K2 verilerini kullanarak, yapay zekâ destekli bir modelle yeni ötegezegenlerin otomatik tespitini sağlamak.

Yani projemiz, uzay gözlemlerinden gelen verileri analiz ederek bir nesnenin gerçekten “gezegen” olup olmadığını tahmin eden bir sistem geliştirmeyi hedefliyor.

🔬 Kullanılan Veri Seti

Projede NASA’nın Cumulative Exoplanet Data veri setini kullandık.
Bu veri seti:

Farklı uzay görevlerinden (Kepler, TESS, K2) toplanan binlerce gözlem içeriyor,

Her satır bir gökcismini temsil ediyor,

Işık eğrisi özellikleri, sinyal gücü, periyot, yarıçap, sıcaklık gibi birçok parametre barındırıyor,

“Confirmed”, “Candidate” ve “False Positive” etiketleriyle ötegezegenlerin sınıfını gösteriyor.

Bu sayede modelimiz, gökcisminin gerçek bir gezegen mi yoksa yanlış pozitif mi olduğunu öğrenebiliyor.

🤖 Yapay Zekâ Modeli

Veri ön işleme adımlarında:

Eksik ve bozuk veriler temizlendi,

Sayısal değişkenler ölçeklendirildi,

Etiketler “Confirmed / False Positive” olarak kodlandı.

Modelleme aşamasında:

Random Forest ve XGBoost gibi güçlü algoritmalarla testler yapıldı,

Modelin doğruluk oranı %90’ın üzerine çıkarıldı,

Eğitim sonrası model .pkl formatında kaydedilerek mobil/web uygulamasına entegre edilmeye hazır hâle getirildi.

📱 Uygulama Entegrasyonu

Projeyi sadece bir model olarak bırakmadık;
geliştirdiğimiz sistemi mobil uyumlu bir arayüze (Streamlit veya Flutter) entegre ettik.

Kullanıcı arayüzünde:

Kullanıcı, gökcisminin parametrelerini (örneğin yörünge süresi, yıldızın sıcaklığı vb.) giriyor,

Sistem bu girdileri modele gönderiyor,

Model, “Bu bir ötegezegen olabilir” veya “Yanlış pozitif” gibi bir tahmin veriyor.

Bu sayede proje, hem bilim insanlarına hem uzay meraklılarına keşif sürecinde yardımcı olacak bir araç hâline geliyor.

🌌 Beklenen Katkı

NASA’nın veri analiz yükünü azaltmak,

Ötegezegen keşif sürecini hızlandırmak,

Uzay araştırmalarında yapay zekâ kullanımına yeni bir örnek oluşturmak,

Eğitim, araştırma ve kamu ilgisini artırmak.
