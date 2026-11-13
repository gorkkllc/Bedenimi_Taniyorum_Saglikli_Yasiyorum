# Bedenimi Tanıyorum ve Sağlıklı Yaşıyorum

İlkokul öğrencilerinin insan anatomisini ve temel iç organları etkileşimli, görsel ve keşfe dayalı bir deneyimle öğrenmelerine yardımcı olan 2D eğitsel dijital oyun prototipi.

* **Proje Durumu:** Prototip / Geliştirme Aşamasında (Ara Değerlendirme Sürümü)
* **Hedef Platform:** Masaüstü / PC (Windows)
* **Oyun Motoru:** Unreal Engine 5 (UMG Widget Blueprint Sistemi)
* **Geliştirici:** Görkem Kılıç (`240601031` — [@gorkkllc](https://github.com/gorkkllc)) | Bireysel Proje (%100 Katkı)
* **Ders:** Atlas Üniversitesi — Dijital Oyun Tasarımı Bölümü (`1514311011 — Dijital Oyun Projesi 1`)

---

## Genel Bakış

**Bedenimi Tanıyorum ve Sağlıklı Yaşıyorum**, etkileşimli ortamların ve oyun tabanlı öğrenmenin çocukların insan biyolojisini anlamasına nasıl destek olabileceğini araştıran eğitsel bir 2D oyun projesidir.

Proje, özellikle **7–10 yaş aralığındaki ilkokul öğrencileri** göz önünde bulundurularak tasarlanmıştır. Öğrenciler yalnızca ders kitaplarındaki düz metinlere bağlı kalmak yerine, seçtikleri karakter üzerinden vücuttaki temel organları keşfedebilir, organ görsellerini inceleyebilir ve rehber doktor karakterinin anlatımı eşliğinde organların görevlerini adım adım öğrenebilirler.

Geliştirme sürecinde bir **pedagog ile ön görüşme** gerçekleştirilmiş; görsellerin çocuklar için kaygı uyandırmayan yumuşak bir üslupla hazırlanması, metinlerin sadeleştirilmesi ve bilgilerin kısa zamanlı parçalara bölünmesi gerektiği belirlenmiştir. İlk kilometre taşı olarak giriş ekranı, karakter seçimi ve örnek organ modülünün (Akciğer) uçtan uca çalıştığı çekirdek prototip oluşturulmuştur.

---

## Öğrenme Hedefleri

* Soyut anatomik kavramları yaş grubuna uygun etkileşimli görseller ve somut benzetmeler sayesinde anlaşılır kılmak.
* Keşif, tıklama ve adım adım takip yoluyla aktif öğrenmeyi teşvik etmek.
* İlkokul öğrencilerinin insan vücudundaki 10 temel iç organı birbirinden ayırt etmesini ve temel görevlerini kavramasını sağlamak.
* Eğitici içerik hedeflerini sade, dikkat dağıtmayan ve erişilebilir bir arayüz tasarımıyla birleştirmek.
* Dijital oyunların ilkokul düzeyinde sağlık ve biyoloji eğitiminde destekleyici bir araç olarak kullanımını incelemek.

---

## Mevcut Kapsam ve Durum

Proje aşamalı (iteratif) olarak geliştirilmektedir. Aşağıdaki tablo, ara değerlendirme prototipinde tamamlanan bölümler ile final aşamasına planlanan özellikleri birbirinden ayırmaktadır.

| Alan | Açıklama | Durum |
| :--- | :--- | :--- |
| **Giriş ve Karakter Seçimi** | Başlangıç ekranı (`WBP_LoginScreen`) ve kız/erkek çocuk ekranlarına (`WBP_GirlScreen`, `WBP_BoyScreen`) yönlendirme | **Tamamlandı** |
| **Görsel Tasarım ve Varlıklar** | Pedagog görüşmesi doğrultusunda yenilenen 2D karakter, rehber doktor ve 10 iç organ illüstrasyonu | **Tamamlandı** |
| **Örnek Organ Etkileşimi (Akciğer)** | Akciğer butonuna tıklandığında organ görselinin açılması, 10'ar saniyelik 3 aşamalı bilgi akışı ve rehber doktor konuşma döngüsü (`Doctor_Animation`) | **Tamamlandı** |
| **Diğer Organ Modülleri** | Kalan 9 organ butonunun (Kalp, Mide, Beyin, Karaciğer, Böbrek, Bağırsak, Mesane, Pankreas, Üreme Organları) ortak etkileşim yapısına bağlanması | **Planlandı** |
| **Sesli Anlatım (`.mp3`)** | İlkokul öğrencilerinin okuma düzeyini desteklemek amacıyla her bilgi adımına özel `.mp3` seslendirme dosyalarının eklenmesi | **Planlandı** |
| **Ölçme ve Değerlendirme** | Keşif sonrasında *"Bu görevi yerine getiren organ hangisidir?"* formatında soru-cevap tabanlı mini değerlendirme ekranı | **Planlandı** |

> *Not: Bu tablo ara değerlendirme aşamasındaki mevcut ilerlemeyi ve final yol haritasını göstermektedir; uygulama ilerledikçe durumlar güncellenecektir.*

---

## Teknoloji Yığını

| Teknoloji | Amaç |
| :--- | :--- |
| **Unreal Engine 5 (UE5)** | Oyun motoru ve geliştirme ortamı |
| **Blueprint Visual Scripting** | Oynanış mantığı, zamanlayıcı akışları ve animasyon döngüleri |
| **Unreal Motion Graphics (UMG)** | 2D kullanıcı arayüzü, ekran geçişleri ve dinamik bilgi panelleri |
| **Masaüstü / PC (Windows)** | Hedef çalıştırma ve test platformu |
| **Git & GitHub** | Versiyon kontrolü ve haftalık geliştirme takibi |

---

## Başlarken

### Gereksinimler

* Unreal Engine 5 Editörü
* Git veya GitHub Desktop
* Standart fare (Mouse) girişine sahip Windows bilgisayar *(Projede harici sensör, API veya özel kontrolcü kullanılmamaktadır)*

### Depoyu Klonlayın

```bash
git clone [https://github.com/gorkkllc/Bedenimi_Taniyorum_Saglikli_Yasiyorum.git](https://github.com/gorkkllc/Bedenimi_Taniyorum_Saglikli_Yasiyorum.git)
cd Bedenimi_Taniyorum_Saglikli_Yasiyorum
```

### Projeyi Açın

1. Klonladığınız `Bedenimi_Taniyorum_Saglikli_Yasiyorum` klasörünü açın.
2. Proje ana dizinindeki `.uproject` dosyasına çift tıklayarak projeyi **Unreal Engine 5** ile başlatın.
3. Motorun proje varlıklarını ve paketlerini yüklemesini bekleyin.
4. Ana haritanın açık olduğundan emin olun ve üst menüden **Play (`Alt + P`)** butonuna basarak prototipi çalıştırın.

### Prototipi Test Edin

1. Giriş ekranında **Başla (Start)** butonuna tıklayın.
2. Açılan seçim ekranından **Kız Çocuk** karakterini seçin.
3. Bilgilendirme ekranının üst kısmındaki **Akciğer** butonuna tıklayın.
4. Ortada akciğer görselinin belirmesini, alt panelde 10'ar saniyelik aralıklarla 3 aşamalı bilgi akışının ilerlemesini ve sağ taraftaki rehber doktorun konuşma animasyon döngüsünü gözlemleyin.

---

## Depo Yapısı

Proje standart Unreal Engine 5 klasör düzenini takip etmektedir. Geliştirme süreci ilerledikçe içerik genişletilecektir.

```text
Bedenimi_Taniyorum_Saglikli_Yasiyorum/
├── Config/                      # Proje ve motor yapılandırma ayarları
├── Content/                     # Oyun haritaları, Widget Blueprint'ler (WBP) ve 2D görsel varlıklar
├── gorseller/                   # Ara değerlendirme ekran görüntüleri ve arayüz taslakları
├── BedenimiTaniyorum.uproject   # Unreal Engine 5 proje başlatıcı dosyası
└── README.md                    # Proje dokümantasyonu ve yol haritası
```

---

## Geliştirme Yol Haritası

Aşağıdaki yol haritası, ders takvimine göre tamamlanan adımları ve final teslimine kadar hedeflenen yönü özetlemektedir:

* [x] **1–2. Haftalar (Araştırma):** Hedef kitle (7–10 yaş) analizi, GitHub deposunun açılması, ilk README ve proje yapısının oluşturulması *(Sorumlu: Görkem Kılıç)*
* [x] **3–4. Haftalar (Tasarım):** Çekirdek döngü ve ekran akışı tasarımı, pedagog ön görüşmesi, kız/erkek karakter seçimi ve 2D arayüz taslakları *(Sorumlu: Görkem Kılıç)*
* [x] **5–7. Haftalar (İlk Prototip / Ara Değerlendirme):** Giriş, karakter seçimi ve bilgi ekranlarının UMG ile kurulması; 10 organ görselinin hazırlanması ve **Akciğer** etkileşiminin (10'ar sn 3 aşamalı metin + doktor animasyon döngüsü) kodlanması *(Sorumlu: Görkem Kılıç)*
* [ ] **9–12. Haftalar (Üretim):** Kalan 9 organ butonunun modüler yapıya bağlanması ve her bilgi kartı için `.mp3` sesli anlatım entegrasyonu *(Sorumlu: Görkem Kılıç)*
* [ ] **9–12. Haftalar (Ölçme Mekaniği):** Öğrenmeyi sınayan *"Bu görevi yerine getiren organ hangisidir?"* soru-cevap mini değerlendirme ekranının eklenmesi *(Sorumlu: Görkem Kılıç)*
* [ ] **11–13. Haftalar (Kullanıcı Testleri):** Veli onamı ile en az 3 hedef kullanıcı (`K1`, `K2`, `K3`) üzerinde oynanış ve okunabilirlik testlerinin yapılması *(Sorumlu: Görkem Kılıç)*
* [ ] **14–16. Haftalar (Final):** Test bulgularına göre arayüz iyileştirmeleri, hata düzeltmeleri ve final sürüm paketinin hazırlanması *(Sorumlu: Görkem Kılıç)*

---

## Görseller ve Test Bulguları

* **Ekran Görüntüleri:** Giriş ekranı, karakter seçimi ve akciğer bilgilendirme arayüzüne ait güncel ekran görüntüleri depo içerisindeki [`gorseller/`](./gorseller) klasöründe yer almaktadır.
* **Pedagog Ön Görüşmesi Bulguları (Tamamlandı):**
  * *Bulgu 1:* Gerçekçi anatomik organ çizimlerinin ilkokul öğrencilerinde korku ve çekince oluşturabileceği belirlenmiştir. → *Düzeltme:* Tüm organ ve karakter çizimleri sıcak, pastel tonlu ve çocuk dostu 2D illüstrasyonlarla yenilenmiştir.
  * *Bulgu 2:* Uzun metin bloklarının çocukların okuma hızını zorladığı tespit edilmiştir. → *Düzeltme:* Açıklamalar sadeleştirilerek 10'ar saniyelik 3 kısa adıma bölünmüş; final sürümü için sesli anlatım desteği planlanmıştır.
* **Hedef Kullanıcı Testi (Planlanan):** 9–12. haftalar arasında 7–10 yaş aralığında en az 3 ilkokul öğrencisi ile uygulamalı test yapılacak; katılımcılar anonim kodlarla (`K1`, `K2`, `K3`) raporlanarak gözlenen bulgulara göre iyileştirmeler uygulanacaktır.

---

## Kaynaklar, Katkı ve Yapay Zekâ Beyanı

* **Katkı Dağılımı:** Proje bireysel olarak yürütülmüş olup oyun tasarımı, UMG arayüz kurgusu, Blueprint kodlaması ve dokümantasyon süreçlerinin tamamı **Görkem Kılıç (%100)** tarafından gerçekleştirilmiştir.
* **Kullanılan Yapay Zekâ Araçları ve Öğrenci Kontrolü:**
  * **ChatGPT ve Google Gemini (Görsel Üretimi ve Metin Sadeleştirme):** Oyundaki kız/erkek çocuk karakterleri, rehber doktor ve 10 iç organ illüstrasyonlarının üretimi ile eğitici metinlerin ilkokul düzeyine sadeleştirilmesinde kullanılmıştır.
  * **Google Gemini (Blueprint ve Dokümantasyon Desteği):** Unreal Engine 5 UMG Blueprint etkileşim kurgusu (ekran geçişleri, zamanlayıcı akışı ve doktor konuşma döngüsü) ve proje dokümantasyonunun düzenlenmesinde destek alınmıştır.
  * **Kontrol Süreci:** Üretilen Blueprint düğümleri proje içinde öğrenci tarafından tek tek kurulup test edilmiştir.

---

## Katkıda Bulunma

Geri bildirimler, hata bildirimleri ve eğitsel iyileştirme önerileri memnuniyetle karşılanır:

1. Yeni bir bildirim açmadan önce mevcut **Issues** sekmesini kontrol edin.
2. Hata bildirimlerinde hatanın hangi ekranda ve hangi adımda oluştuğunu açıkça belirtin.
3. Özellik önerilerinde, önerinin 7–10 yaş grubunun öğrenme veya arayüz deneyimine nasıl katkı sağlayacağını açıklayın.

---

## Proje Durumu ve Kapsam

**Bedenimi Tanıyorum ve Sağlıklı Yaşıyorum**, aktif geliştirme sürecinde olan bağımsız bir akademik oyun prototipidir. Özellikler, etkileşim akışları ve arayüz detayları kullanıcı testleri doğrultusunda geliştirilmeye devam edecektir.

Bu depo, projenin haftalık geliştirme sürecini şeffaf biçimde belgelemek ve ilkokul düzeyinde oyun tabanlı sağlık eğitimi çalışmalarına temel oluşturmak amacıyla hazırlanmıştır.

---

## Lisans

Bu depo için henüz açık kaynaklı bir lisans seçilmemiştir. Bir lisans eklenene kadar tüm hakları proje geliştiricisine (`Görkem Kılıç`) aittir; izinsiz çoğaltma veya ticari kullanım varsayılmamalıdır.

*Unreal Engine ve keşfederek öğrenme merakıyla geliştirilmiştir.*
