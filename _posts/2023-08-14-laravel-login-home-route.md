---
layout: post
title: Laravel route home yolunu değiştirme
categories: [Genel,Çözüm,Laravel,Home,Route,Login]
tags: [ipucu,laravel,home,route,login]
fullview: true
---

Laravel projemizde login ekranından sonra **home** linki olarak yönlendirme işlemini değişribiliriz. Örneğin 
login olduktan sonra **site/home** yerine **site/panel** olarak route işlemi için **app/Providers/RouteServiceProvider**
içerisindeki **public const HOME = '/home';** yerine **public const HOME = '/panel';** kodunu yazmamız yeterli olacaktır.
Kod Yapısı

{% highlight yaml %}

    //public const HOME = '/home';
    public const HOME = '/panel';

{% endhighlight %}

Artık projemiz login olduktan sonra **site/panel** linkine direkt yönlendirilecektir.

Kolay gelsin.

