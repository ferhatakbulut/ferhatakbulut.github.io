---
layout: post
title: apache ve mysql hizmetlere ekleme
categories: [Genel,Xampp,Apache,Mysql]
tags: [apache,mysql]
description: xampp yada diğer php serveler için apache ve mysql yapılarını hizmetlere ekleme
---

xampp yada diğer php serveler için **apache** ve **mysql** yapıları bilgisayarın hizmetler kısmında görünmüyorsa
bunu kısa bir komut ile çözebiliriz.

Komut satırını yöneti olarak çalıştırı diyerek açıyoruz.

**apache** için

{% highlight yaml %}

    cd xampp/apache/bin
    httpd -k install

{% endhighlight %}

**mysql** için

{% highlight yaml %}

    cd xampp/mysql/bin
    mysqld --install mysql

{% endhighlight %}

yazmamız yeterlidir.
Artık apache ve mysql yapıları hizmetler kısmında oluşturulmuş olarak görünecektir.

Kolay gelsin.

