---
layout: post
title: Ajax Get Post İşlemleri
categories: [Genel,Laravel,Ajax,Get,Post,Php]
tags: [ipucu,laravel,ajax,get,post,php]
fullview: true
---

Ajax yapısı ile Get/Post işlemleri için aşağıdaki kod yapısını kullanabilirsiniz.
url ile bu url deki işlem sonucunu ve datadaki verilerimizi göndereredek dönen değeri sayfamızda istediğimiz
yerde kullanabiliriz.

Kod Yapısı

{% highlight yaml %}

    $.ajax({
        url: '{{URL::to("urunler/teknik-ozellikler")}}',
        type: "GET",
        data: "teknikId="+$("#teknik_sartname").val(),
        success: function (msg) {	
             $("#icerik").html(msg);		
           }
        });

{% endhighlight %}



Kolay gelsin.

