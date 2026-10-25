MovaForge
Turn Footage Into Motion.

MovaForge, tek kişinin bulunduğu bir videodaki hareketi 3B karakter animasyonuna dönüştürmek için geliştirdiğim Windows masaüstü uygulamasıdır.
Neler yapabilirsiniz?
- Bir videodaki hareketi 3B karaktere aktarabilirsiniz.
- Kaynak video ile karakter animasyonunu aynı zaman çizelgesinde karşılaştırabilirsiniz.
- Hareketi stabilize edip ayak ve el temasındaki kaymaları azaltabilirsiniz.
- Sorunlu zaman aralıklarını inceleyebileceğiniz, not ekleyebileceğiniz ve kalite kontrol sonuçlarını JSON olarak dışa aktarabileceğiniz inceleme ekranını kullanabilirsiniz.
- Animasyonu GLB, FBX veya düzenlenebilir Blender (.blend) projesi olarak dışa aktarabilirsiniz.
GLB ve FBX dosyaları Blender, Unity ve Unreal Engine gibi 3B araçlarda kullanılabilir. FBX ve .blend dışa aktarma işlemleri için uyumlu bir Blender kurulumu gerekebilir.
İlk prototip sonuçları
6,6 saniyelik, tek kişinin bulunduğu bir test klibinde şu sonuçları aldım:
Ölçüm	Önce	Sonra
Ayak kayması	24,4 cm	2,7 cm
El kayması	55,7 cm	7,8 cm
El temasında zemin penetrasyonu	13,0 cm	3,2 cm


Bu ölçümler yalnızca test edilen klibe aittir; her video, karakter veya kamera açısında aynı sonuç garanti edilmez.
İndirme ve çalıştırma
MovaForge, bu sürümde Windows için çalıştırılabilir EXE olarak sunulur. Kaynak kodu indirme paketine dahil değildir.
1. Bu GitHub deposunun Releases bölümünden en güncel Windows EXE dosyasını indirin.
2. Dosyayı bilgisayarınızda uygun bir klasöre kaydedin.
3. EXE dosyasını çalıştırın ve uygulama içindeki adımları izleyin.
İndirme dosyası neden büyük?
Tek paket hâlindeki uygulama, hareket çıkarımı için kullanılan yapay zekâ model dosyalarını ve gerekli çalışma zamanı bileşenlerini içerir. Bu bileşenlerin uygulamayla birlikte sunulması, kullanıcıların bunları ayrı ayrı kurma ihtiyacını azaltır; indirme boyutunu da artırır.
Bilinmesi gerekenler
- MovaForge hâlâ erken aşamadaki bir prototiptir; tüm üretim koşulları için doğrulanmış değildir.
- En iyi sonuçlar için videoda tek bir kişi, baştan ayağa ve mümkün olduğunca net görünmelidir. Kadraj dışında kalan vücut parçaları, yoğun hareket bulanıklığı, örtüşme veya sıra dışı kamera açıları sonucu etkileyebilir.
- İlk uçtan uca doğrulama tek bir kısa klip ve tek bir karakter üzerinde CPU ile yapıldı. Farklı videolar ve karakterlerle daha fazla test gerekiyor.
- NVIDIA/CUDA ile çalışma yolu mevcut olsa da uçtan uca GPU doğrulaması henüz tamamlanmadı; sonuçlar donanıma, sürücülere ve ortama bağlı olabilir.
- Test edilen klipte el temasında yaklaşık 3,2 cm kalıntı zemin penetrasyonu bulunuyordu.
- Prototip gerçek zamanlı işlem için doğrulanmış değildir; uzun videoların işlenmesi daha uzun sürebilir.
Geri bildirim
Hata bildirimleri, öneriler ve iş birliği için bu GitHub deposunun Issues bölümünü kullanabilirsiniz.
