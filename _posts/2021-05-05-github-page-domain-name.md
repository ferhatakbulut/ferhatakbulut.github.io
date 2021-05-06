---
layout: post
title: Github page özel alan adına yönlendirme (Github page domain name configuration)
categories: [genel, github]
tags: [github, githubpage,page, domainname]
description: Github Page aldığımız özel domain adresine yönlendirme
---

Github üzerinde **ferhatakbulut.github.io** url ile bir web sitesimiz yayındaysa, biz bu yayınımızı özel alan adımıza
yani örnek olarak **ferhatakbulut.com** adresi ile ulaşmak için aşağıdaki işlemleri yapabilirsiniz.

Öncelik bir alan adı satın alıyoruz.
Ben turhost.com üzerinden **ferhatakbulut.com** adını satın aldım.

Github depomuza yani ferhatakbulut.github.io gidiyoruz ve CNAME kaydı oluturuyoruz. Bu CNAME aldığımız alan adını giriyoruz
ve bunu depomuzun içerisine atıyoruz.

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/q1.png">

Alan adı aldığımız alan adı sağlayıcıya gidiyoruz ve aldığımız alan adının ayarlarına giriyoruz.
Buradan alan adımızın **DNS Yönetimi** bölümüne giriyoruz.

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/q2.png">

Daha sonra A türünde yeni DNS Kaydı oluşturuyoruz. Github page ip adresleri 4 tane her biri için tek tek oluşturuyoruz.
Yeni DNS kaydı için girilecek değerler aşağıdaki resimlerde mevcuttur.

{% highlight yaml %}

   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153

{% endhighlight %}


<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/q5.png">

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/q4.png">

İşlemlerimiz bu kadar fakat turhost alan adı sağlayıcının ekstra bir ayarı daha var. Oda isim sunucusunu ayarlarma
yani şöyle düşünebiliriz. Turhosttan alan adı aldığımız için host alanınıda kendi içerisinde otomatik olarak aramaya
çalışır. Fakat biz host olarak github kullanıyoruz. Bunun için host tu dışarıda bul diye bir ayar var.

Öncelikle alan adımızın **İsim Sunucular** menüsüne giriyoruz. Başka alan adı sağlayıcılarında bu menü **Nameserver** olarak 
görülebilir. İsim sunucuları değerleri olarak turhost un bize dış olarak verdiği aşağıdaki değerler girip kaydetmemiz yeterlidir.
Bu sayade host alanımızın Turhost dışında bir yerde olduğunu söylemiş olduk.

{% highlight yaml %}

   dns1.turhost.com
   dns2.turhost.com

{% endhighlight %}


<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/q6.png">

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/q7.png">


Son olarak github depomuza geliyoruz. **Settings -> Pages** bölümünde **Custom domain** alanına aldığımız alan adını giriyoruz
ve kaydediyoruz.

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/q8.png">

Artık işlemlerimiz tamamlandı ve 24 saat içerisinde aldığımız özel alan adımızla ulaşabiliriz.

Github kendi sayfalarında bunu detaylı anlatmakdır. Oradan da yardım alabilirsiniz -> **[Github Page Ayarları](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)**

Kolay gelsin.

