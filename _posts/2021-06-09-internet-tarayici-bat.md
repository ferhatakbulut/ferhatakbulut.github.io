---
layout: post
title: bat dosyası ile web sayfası açma
categories: [Genel, Bat, İpucu]
tags: [chrome, edge, bat, kısayol]
description: Sürekli kullandığınız web sitelerini tek tek el ile açmak yerine bat dosyası ile tek seferde çalıştırabilirsiniz.
---


Text dosyası açıyoruz. Text dosyasını **.bat** uzantılı olarak kaydediyoruz.
Yada cmd ile komut satırı ile aşağıdaki komutları çalıştırabiliriz.
Ben kullandığım biden fazla web sitesi olduğu için komut dosyalarımı bat dosyasına yazıyorum ve tek seferde tüm web sayfalarımı
açmamda bana yardımcı oluyor.

Aşağıdaki komut satırı ile yeni sekmede istediğimiz web sitesini açıyoruz.

{% highlight yaml %}

    start chrome www.google.com
    start chrome www.ferhatakbulut.com
    start msedge www.w3school.com

{% endhighlight %}

Üst komut ile aynı chrome içerisinde **www.google.com** ve **www.ferhatakbulut.com** açılacaktır. **www.w3shool.com** microsft edge içesinde açılacaktır.

Eğer faklı sekmelerde açmak istersek

{% highlight yaml %}

    start chrome /new-window www.google.com
    start chrome /new-window www.ferhatakbulut.com

{% endhighlight %}

farklı chrome larda sayfalar açılacaktır.

Tercih sizin :)

Kolay gelsin.

