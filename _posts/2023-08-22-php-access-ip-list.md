---
layout: post
title: Php ile Sadece Belirli İp Grubuna Erişim Verme İşlemi
categories: [Genel,Laravel,Php,İp,Access]
tags: [ipucu,laravel,php,ip,erişim,access]
fullview: true
---

Yaptığımız projeye sadece belirli bir ip grubunun erişimine izin vermek için aşağıdaki kod yapısını kullanabilirsiniz.
Bu kod yapısını kullandığımız zaman sadece **10.15.xx.xx** ile başlayan ip grubu projemize erişim sağlayacaktır.

Kod Yapısı

{% highlight yaml %}

    $network = ip2long("10.15.0.0");
    $mask = ip2long("255.255.0.0");
    $ip = ip2long($_SERVER['REMOTE_ADDR']);
    if (($network & $mask) != ($ip & $mask)) {
        die("Unauthorized");
    }

{% endhighlight %}



Kolay gelsin.


