---
layout: post
title: Ağ üzerinde paylaşılan dosyalar
categories: [cmd]
tags: [paylasim, netshare]
fullview: true
---

Windows işletim sistemi için ağ üzerinde paylaşılan dosyaları/klasörleri görmek için
komut satırına

{% highlight text 1-2 %}
    >>>net share
{% endhighlight %}


yazarak ekranda paylaşılan ögeleri görebiliriz.

Paylaşılan dosyaları/klasörleri silmek için komut satırından

{% highlight text 1-2 %}

    >>>net share klasorAdi /delete

{% endhighlight %}

yazmamız yeterlidir.

Örnek olarak

{% highlight text 1-2 %}

    >>>net share $d /delete             //d diskinin tamamını paylaşımdan siliyoruz
    >>>net share D:\Resimler /delete    //d diskinde resimler klasörünü paylaşımdan siliyoruz

{% endhighlight %}


Kolay gelsin.

