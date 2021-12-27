---
layout: post
title: Ağ üzerinde paylaşılan dosyalar
categories: [cmd]
tags: [paylasim, netshare]
fullview: true
---

Windows işletim sistemi için ağ üzerinde paylaşılan dosyaları/klasörleri görmek için
komut satırına

{% highlight yaml %}

>>>net share 

{% endhighlight %}

yazarak ekranda paylaşılan ögeleri görebiliriz.

Paylaşılan dosyaları/klasörleri silmek için komut satırından

{% highlight yaml %}

>>>net share klasorAdi /delete

{% endhighlight %}

yazmamız yeterlidir.

Örnek olarak

{% highlight yaml %}

>>> net share d$ /delete                 // d diskinin tamamını paylaşımını siliyoruz
>>> net share D:\Resimler /delete        // d diskinde resimler klasörünün paylaşımını siliyoruz

{% endhighlight %}


Kolay gelsin.

