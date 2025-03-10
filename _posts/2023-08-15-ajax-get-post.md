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
        url: "",
        type: "GET",
        data: "degisken="+$("#degisken").val(),
        success: function (msg) {
           $("#icerik").html(msg);
          }
    });

{% endhighlight %}

{% highlight yaml %}

    $.ajax({
        url: "",
        type: "POST",
        data: "_token="+"{{ csrf_token() }}"+"degisken="+$("#degisken").val(),
        success: function (msg) {
           $("#icerik").html(msg);
          }
    });

{% endhighlight %}



Kolay gelsin.


