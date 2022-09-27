---
layout: post
title: Laravel Cache Temizleme
categories: [Genel, Xampp, Php, Laravel]
tags: [laravel, cache]
fullview: true
---

cmd komut ekranından laravel projemizin olduğu klasöre gidiyoruz.
Sonra aşağıdaki komutları giriyoruz.

{% highlight yaml %}

    
    php artisan config:cache
    php artisan config:clear
    php artisan config:cache
    php artisan cache:clear
    php artisan route:clear
    php artisan route:cache
    php artisan view:clear
    php artisan view:cache
    php artisan config:cache
    php artisan optimize:clear 

{% endhighlight %}

yazmamız yeterlidir.

Kolay gelsin.

