---
layout: post
title: Ödeme Kartları Endüstrisi Veri Güvenliği Standartları (PCI DSS) ile Güvenli Kart Ödemeleri
date: 2024-04-15 09:00:20 +0300
description: # Add post description (optional)
img: pci_dss_gereklilik.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Technology, Banking,  Payment, Credit Card, PCI DSS, Digital Transformation, Ödeme yöntemleri, Kredi kartı, Bankacılık, Finans] # Add post tags (optional)
---
Günümüzde ödeme alışkanlıklarında önemli bir değişim gözlemlenmektedir. Yüksek miktarda nakit para taşımanın zorluğu, nakit para bulundurmak için Bankamatik’e gitme gerekliliği, giderek yaygınlaşan çevrimiçi alışveriş ve kart ile ödemede taksitlendirme gibi sebeplerden dolayı nakit para yerine ödeme aracı olarak kart kullanımında ciddi bir artış söz konusudur.

Bankalararası Kart Merkezi (BKM) verilerine göre, 2023 yılı itibarıyla Türkiye’de kredi kartı sayısı 117,7 milyon, banka kartı sayısı 189,5 milyon ve ön ödemeli kart sayısı 90 milyon adettir. Toplam kart sayısı ise 397 milyon adettir[1]. Dünya genelinde ise kullanımdaki kredi kartı, banka kartı ve ön ödemeli kart sayılarının toplamı 2023 yılı itibariyle 26.71 Milyar adet olarak kayıtlara geçmiştir. [2]

Türkiye Cumhuriyeti Merkez Bankası (TCMB) verilerine göre, Şekil 1'de gösterildiği gibi, Türkiye’de 2023 yılı boyunca yaklaşık 8 Trilyon Türk Lirası kartlı harcama yapılmıştır. Bu oran bir önceki yıla göre %100'ün üzerinde bir artış demektir.

<p style="text-align: center"><img src="{{site.baseurl}}/assets/img/kart_harcama.jpg"></p>
<p style="text-align: center">Şekil 1: Türkiye’de 2023 yılı boyunca yaklaşık 8 Trilyon Türk Lirası kartlı harcama yapıldı.</p>

Hem Türkiye’de hem de Dünya genelinde milyarlarca kartın kullanıldığı ve çok yüksek miktarlarda işlem hacmine sahip olan kartla ödeme sektöründe güvenlik konusu tahmin edileceği üzere çok önemlidir.

Açılımı Payment Card Industry Data Security Standard olan, Türkçeye ise Ödeme Kartı Sektörü Veri Güvenliği Standardı olarak geçen PCI DSS, 2004 yılında dört büyük kredi kartı şirketi Visa, MasterCard, Discover ve American Express tarafından ortaklaşa oluşturulmuştur. Ödeme Kartı Sektörü Güvenlik Standartları Konseyi (Payment Card Industry Security Standards Council — PCI SSC) ise, Ödeme Kartı Sektörü Veri Güvenliği Standardı’nın devam eden gelişimini yönetmek amacıyla American Express, Discover Financial Services, JCB International, MasterCard ve Visa Inc. tarafından 2006 yılında kurulmuştur.

PCI DSS, kredi kartı, banka kartı ve nakit kartı işlemlerinin güvenliğini sağlamayı ve kart sahiplerini kişisel bilgilerinin kötüye kullanılmasına karşı korumayı amaçlamaktadır. Kart bilgilerini işleyen, saklayan veya ileten tüm şirketlerin güvenli bir ortam oluşturmasını sağlamaya yönelik bir dizi gereksinimdir ve yaygın olarak kabul görmektedir.

<p style="text-align: center"><img src="{{site.baseurl}}/assets/img/pci_dss.jpg"></p>
<p style="text-align: center">Şekil 2 - PCI DSS [3]</p>


## PCI DSS Uyumluluğu ##

PCI DSS uyumluluğu, ödeme kartı işlemlerine dahil olan işletmelerin ve kuruluşların, kart sahiplerinin hassas bilgilerini korumak ve veri ihlallerini önlemek için belirlenen güvenlik standartlarını uygulamasını gerektirir. Bu uyumluluk, ödeme kartı markaları tarafından desteklenir ve sıkı denetimler ve cezai yaptırımlarla uygulanabilir. Ayrıca, işletmelerin itibarını korumak ve müşteri güvenini sağlamak için de önemlidir. PCI DSS uyumluluğu bir işletmenin bu standartlara uygunluğunu ifade eder.

PCI SSC’ye göre, bir satıcının PCI uyumluluk kontrol listesinin bir parçası olarak tamamlaması gereken gereklilikler vardır. PCI DSS gereklilikleri Şekil 3'teki gibi gruplanmaktadır; Güvenli Ağ, Kart Sahibi Verilerinin Güvenliği, Güvenlik Açığı, Giriş (Erişim) Kontrolü, Ağ İzleme ve Test Etme, Bilgi Güvenliği ana başlıklarında gruplanmaktadır. [4]

<p style="text-align: center"><img src="{{site.baseurl}}/assets/img/pci_dss_gereklilik.jpg"></p>
<p style="text-align: center">Şekil 3: PCI DSS Gereklilikleri</p>

PCI DSS uyumluluğu için kontrol edilmesi gereken 12 ana gereksinim aşağıda listelenmiştir:

**Güvenli Ağ**

1.Güvenlik duvarlarını kullanın ve Bakımını yapın

2.Uygun parola korumaları

**Kart Sahibi Verilerinin Güvenliği**

3.Kart sahini verilerini koruyun

4.İletilen verileri şifreleyin

**Güvenlik Açığı Yönetimi**

5.Antivirüs kullanın ve bakımını yapın

6.Düzgün güncellenmiş yazılım

**Giriş (Erişim) Kontrolü**

7.Veri erişimini kısıtlayın

8.Erişim için benzersiz kimlikler oluşturun

9.Fiziksel erişimi kısıtlayın

**Ağ İzleme ve Test Etme**

10.Erişim günlükleri oluşturun ve takibini yapın

11.Güvenlik açıklarını tarayın ve test edin

**Bilgi Güvenliği**

12.Bilgi güvenliğiyle ilgili bir politika sürdürülmelidir

## PCI DSS Sertifikası ve Uyumluluk Seviyesi ##

Sisteme dahil olmak için PCI DSS sertifikası adı verilen uygunluk onay formu doldurulmalıdır. Bu form uyarınca sisteme dahil olmak isteyen işyeri ya da e-ticaret şirketi sahipleri üç aylık periyotlarla gerçekleştirilen bir ağ taramasına tabi tutulmaktadır.

PCI DSS sertifikası almak için başvurulan uygunluk onay formu değerlendirmesi şirketin özelliklerine değişiklik göstermektedir. Her şirketin ya da e-ticaret firmasının değerlendirmeye tabi tutulması esnasındaki belirleyici unsur, işlem hacmidir.

PCI uyumluluğu, bir işletmenin yıllık olarak işlediği kredi kartı veya banka kartı işlemlerinin sayısına (işlem hacmine) göre Şekil 4'te gösterildiği gibi dört seviyeye ayrılmıştır. Sınıflandırma seviyesi, bir işletmenin uyumlu kalması için yapması gerekenleri belirler.

<p style="text-align: center"><img src="{{site.baseurl}}/assets/img/pci_dss_uyumluluk_seviye.jpg"></p>
<p style="text-align: center">Şekil 4: PCI DSS uyumluluk seviyesi</p>

**Seviye 1:** Yılda altı milyondan fazla kredi kartı veya banka kartı işlemi gerçekleştiren satıcıları kapsar. Yetkili bir PCI denetçisi tarafından yılda bir kez iç denetime tabi tutulmaları gerekmektedir. Ayrıca, üç ayda bir Onaylı Tarama Satıcısı (Approved Scanning Vendor — ASV) tarafından PCI taramasına tabi tutulmaları gerekir.

**Seviye 2:** Yılda bir milyon ile altı milyon arası kredi kartı veya banka kartı işlemi gerçekleştiren satıcıları kapsar. Yılda bir kez Kendi Değerlendirme Anketi (Self-Assessment Questionnaire — SAQ) kullanarak bir değerlendirme tamamlamaları gerekmektedir. Ek olarak, üç ayda bir ASV tarafından PCI taramasına tabi tutulmaları gerekebilir.

**Seviye 3:** Yılda yirmi bin ile bir milyon arası e-ticaret işlemi gerçekleştiren satıcıları kapsar. İlgili SAQ kullanılarak yıllık bir değerlendirme tamamlamaları gerekmektedir. Ayrıca, üç ayda bir ASV tarafından PCI taramasına tabi tutulmaları gerekebilir.

**Seviye 4:** Yılda 20.000'den az e-ticaret işlemi veya maksimum bir milyon kredi kartı veya banka kartı işlemi gerçekleştiren satıcıları veya bir milyon gerçek dünya işlemi gerçekleştirenleri kapsar. İlgili SAQ kullanılarak yıllık bir değerlendirme tamamlanmalı ve üç ayda bir ASV tarafından PCI taramasına tabi tutulmaları gerekebilir.

## Sonuç ##
PCI DSS (Payment Card Industry Data Security Standard), ödeme kartı işlemlerinin güvenliğini sağlamak için belirlenen standartların neden önemli olduğunu beş madde ile açıklayacak olursak:

1. **Kart Sahiplerinin Güvenliği:** PCI DSS, kart sahiplerinin hassas bilgilerini korumak için gerekli önlemleri almayı zorunlu kılar. Bu, kart sahiplerinin bilgilerinin kötü niyetli kullanımını önler ve güvenilirliklerini artırır.
2. **Dolandırıcılığın Önlenmesi:** Standartlar, işletmelerin güvenlik açıklarını kapatmasını sağlayarak dolandırıcılığı önler. Veri ihlalleri ve kart dolandırıcılığı gibi potansiyel riskleri azaltır.
3. **Kurumsal İtibarın ve Güvenin Korunması:** PCI uyumluluğu, işletmelerin müşterilerine güvenilir bir alışveriş ortamı sağladığını gösterir. Bu da müşteri sadakatini artırır ve işletmenin itibarını korur.
4. **Yasal Yükümlülüklerin Karşılanması:** PCI uyumluluğu, ödeme kartı şirketlerinin ve devlet düzenleyicilerinin belirlediği yasal gereksinimleri yerine getirmeyi sağlar. Bu da potansiyel cezalardan kaçınmaya yardımcı olur.
5. **Maliyet ve Verimlilik:** PCI uyumluluğu, veri ihlallerinin ve dolandırıcılığın yol açabileceği maliyetleri önler. Ayrıca, güvenlik açıklarının tespiti ve giderilmesi sürecinde verimliliği artırır.

Bu nedenlerden dolayı, PCI DSS özellikle ödeme kartı işlemlerinde güvenlik, uyumluluk açısından ve günümüzde internet ve teknolojinin devamlı gelişmesine bağlı olarak ortaya çıkan sanal dolandırıcılığın engellenmesi için oldukça önemlidir.

## Kaynaklar: ##
[1] [https://bkm.com.tr/kart-sayilari/](https://bkm.com.tr/kart-sayilari/)

[2] [https://www.statista.com/statistics/1080756/number-payment-cards-in-circulation-worldwide/](https://www.statista.com/statistics/1080756/number-payment-cards-in-circulation-worldwide/)

[3] [https://www.pcitelecom.co.uk/what-is-pci-dss-compliance-the-basics/](https://www.pcitelecom.co.uk/what-is-pci-dss-compliance-the-basics/)

[4] [www.pcisecuritystandards.org](https://www.pcisecuritystandards.org/pci_security/standards_overview)
