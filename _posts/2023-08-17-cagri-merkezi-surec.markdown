---
layout: post
title: Yazılım Mühendisi'nden Müşteri'ye uzanan Çağrı Merkezi süreci
date: 2023-08-17 09:00:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: banking.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Technology, Banking, Call Center, Software Engineering, Digital Transformation, Agent, Müşteri Temsilcisi, Bankacılık, Finans] # Add post tags (optional)
---
Teknolojinin hızla ilerlemesiyle birlikte, hayatımızın birçok yönünü artık dışarı çıkmadan dijital olarak yönetebiliyoruz. Banka hesaplarını açmak, kredi başvurusu yapmak, vergi ve fatura ödemelerini çevrimiçi gerçekleştirmek, dünyanın önde gelen üniversitelerinde online eğitim almak gibi işler, sıkça başvurduğumuz olanaklardan sadece birkaçı. Ancak bununla sınırlı kalmayarak, Non-fungible token (NFT — Nitelikli Fikri Tapu) ile sanat eserleri oluşturmak, Metaverse (Sanal Evren) dünyasında düğün törenlerine katılmak, artırılmış gerçeklikle Paris sokaklarını gezmek gibi daha önce pek alışık olmadığımız yenilikler de hayatımıza hızla entegre olmaktadır.

![Banking]({{site.baseurl}}/assets/img/banking.jpg)

Bu dijital evrimle birlikte, şirketler de satış ve pazarlama stratejilerini güncel tutmak adına dijital kanalları etkin bir şekilde kullanma yönünde çaba göstermektedirler. Örneğin, 5 Temmuz 2023 tarihinde Instagram, Facebook ve Whatsapp’ın çatı şirketi Meta, Twitter’a rakip olacak yeni sosyal medya platformu Threads’i [1] yayınladı. Çok kısa bir sürede milyonlarca kişi hesap açtı. Tabii ki bu süreç kişilerle sınırlı kalamazdı. Hem yurt içerisinde hem de dünya çapında bir çok kurumsal şirket/marka Threads’te hesap açarak, bu platformda biz de varız dediler.

Dijital kanalları etkili bir şekilde kullanan şirketler, rekabet avantajı elde edebilmektedir. Finans sektöründe de güçlü rekabet ve teknolojik yenilikler, şirketleri dijital dönüşümü hızlandırmaya yönlendirmektedir. Bankalar Çağrı Merkezi, Mobil Bankacılık ve İnternet Bankacılığı gibi dijital kanallar aracılığıyla teknolojinin en son imkanlarını müşterilere sunmaya devam etmektedir.

Bankanın Çağrı Merkezi’nde çalışan Müşteri Temsilcileri müşteri ile bire bir iletişimle bankanın ses vitrini görevini üstlenmektedir. Temsilciler bilgisayar ekranlarındaki bankacılık uygulamasını kullanarak müşterilere hizmet vermektedir. Temsilciler, müşterinin taleplerine göre ilgili bankacılık ekranlarını açarak işlemleri gerçekleştirmektedir. Peki, bu süreç nasıl işliyor?

![Agent]({{site.baseurl}}/assets/img/agent.jpg)

Bankalarda Bilgi Teknolojileri çatısı altında Çağrı Merkezi Teknolojileri, Mevduat Ürünleri Yönetimi, Müşteri Yönetimi, Ödeme Ürünleri Yönetimi ve Nakit Yönetimi gibi birçok ekip bulunmaktadır. Tabii ki ekip isimleri bankadan bankaya farklılık göstermektedir ancak temelde her bir ekip kendi sorumluluk alanlarına odaklanmış durumdadır. Müşteri temsilcisinin kullandığı bankacılık uygulamasında, ekiplerin geliştirdiği yüzlerce farklı ekran açılabilmektedir. Bu ekranlarda, müşteriyi IVR’a ( (Interactive voice response — etkileşimli sesli yanıt sistemi) aktaran düğme, kurumsal müşterilerin alt hesaplarının listelendiği tablo, kanal aktifliğinin yönetilebildiği açılır menüler gibi birçok farklı bileşen bulunuyor. İşte tüm bunlar, temsilcilerin hizmet verirken kullandığı önyüzün (frontend) parçalarını oluşturuyor.

Önyüz, görsel olarak ekranın nasıl göründüğünü ve buton gibi etkileşimli öğelerle nasıl etkileşime girebileceğimizi belirleyen kodlardan oluşuyor. Bu kodlar, bileşenlerin şekli, rengi, konumu gibi detayları içeriyor. Örneğin, bir butona tıkladığımızda hangi hizmetin çağrılacağı veya hangi aksiyonun gerçekleşeceği gibi işlemler bu kodlar içerisine yazılıyor. Tüm bu kodlar bir araya geldiğinde, görsel bir arayüz oluşturuluyor ve temsilcilerin kullanımına sunuluyor.

Ancak butona tıkladığımızda arka tarafta neler oluyor? İşte burada arkayüz (backend) devreye giriyor. Önyüzdeki ekran kodları ve bileşenler, arkayüzdeki servisleri çağırıyor. Servisler, istenilen girdileri alıp çıktılarını sunan yapılar olarak düşünülebilir. Her bir ekip, kendi amaçları doğrultusunda onlarca-yüzlerce servis sunmaktadır. Bu servisler aynı ekibin başka servisini çağırabildiği gibi, diğer ekiplerin sağladığı servisleri de çağrılabilir. Önyüzden çağrılan bir servis, ilgili verileri getirerek ekran üzerinde görüntülemeyi sağlıyor. Bu sayede temsilciler, müşteri taleplerine göre ekranları açıp, müşteri bilgilerini veya ürün detaylarını görüntüleyerek gerekli işlemleri gerçekleştirebiliyorlar.

![Architect]({{site.baseurl}}/assets/img/architecth.jpg)

Genel mimariye bakacak olursak, Yazılım Mühendisi’nin arkayüzde yazdığı servis, servisi çağıran ekran kodu, ekran kodunun görselleştirilmiş halini müşteri temsilcisine gösteren önyüz uygulaması, uygulamayı kullanarak müşteriye hizmet veren müşteri temsilcisi ve son kullanıcı olarak müşteri.

Müşteri temsilcileri, önyüz ve arkayüz sistemleri aracılığıyla müşterilere hızlı ve etkili bir şekilde hizmet verirken, yazılım mühendisleri de bu sürecin temelini oluşturan servisleri geliştirerek sistemin sağlıklı işlemesini sağlamaktadır. Bu karmaşık yapı, son kullanıcı olan müşteriye daha iyi hizmet sunmak amacıyla bir araya gelir. Sonuç olarak, bu süreçte yazılım mühendisleri ve müşteri temsilcileri işbirliği içinde çalışarak dijital dönüşümün getirdiği yenilikleri en etkin şekilde değerlendirmekte ve hizmet kalitesini artırmaktadır.

Kaynaklar:
1. [Threads](https://www.threads.net/)