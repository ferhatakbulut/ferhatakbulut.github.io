---
layout: post
title: Xampp Mysql Hatası
categories: [Genel,Çözüm,Excel]
tags: [excel]
description: Excel de kullanabileceğiniz yararlı bilgiler
---

1- Excel dosyamız açık iken birden fazla sayfa var ise **sayfa1** deki verileri **sayfa2** ye otomatik alma formülü

{% highlight yaml %}

    =Sayfa1!A1

{% endhighlight %}

Bu şekilde sayfa1 deki A1 hücresindeki veriyi sayfa2 yada başka sayfadaki hücrelere taşıyabiliriz.

2- Excelde **if else** yapısı için aşağıdaki kodu kullanabilirsiniz.

{% highlight yaml %}

    =EĞER(A1=1,1,2)
    =EĞER(Sayfa1!A1="",1,Sayfa1!A1)

{% endhighlight %}

İlk formülde A1 hücresindeki değer 1'e eşit ise hücreye 1 yaz değilse hücreye 2 yaz.
İkinci formülde Sayfa1 deki A1 hücresi boş ise 1 yaz değil ise hücreye Sayfa1 deki A1 hücresindeki değeri yaz


Kolay gelsin.

