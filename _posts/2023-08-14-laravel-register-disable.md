---
layout: post
title: Laravel register disable
categories: [Genel,Çözüm,Laravel,Register]
tags: [ipucu,laravel,register,route]
fullview: true
---

Laravel projemizde register yani misafir kullanıcının kendi kullanıcısını oluşturmasını engellemek için 
**routes -> web.php** dosyasında aşağıdaki satırı eklemek yeterlidir. 

Kod Yapısı

{% highlight yaml %}

    Auth::routes([
      'register' => false, // Yeni Kayır Routes...
      'reset' => false,    // Şifre Sıfırlama Routes...
      'verify' => false,   // Email Doğrulama Routes...
    ]);

{% endhighlight %}



Kolay gelsin.

