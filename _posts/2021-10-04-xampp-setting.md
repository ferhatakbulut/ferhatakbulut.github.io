---
layout: post
title: php, xampp bazı ayarlar
categories: [Genel,Xampp,Php]
tags: [php,xampp]
fullview: true
---

xampp ve php için bazı ayarlar

kod bloğu içerisinde

{% highlight yaml %}

    
    ini_set('max_execution_time', '300');  //işlem süresi ayarlama
    ini_set('memory_limit', -1);           //maximum hafıza 

{% endhighlight %}

maximun dosya yükleme işlemi için **php.ini** dosyası içerisindeki

{% highlight yaml %}

    upload_max_filesize = 10M
    post_max_size = 10M

{% endhighlight %}


yazmamız yeterlidir.


Kolay gelsin.

