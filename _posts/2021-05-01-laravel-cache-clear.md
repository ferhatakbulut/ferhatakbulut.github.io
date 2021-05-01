---
layout: post
title: Larvel cache clear (laravel tüm cache temizleme) 
categories: [laravel, programming]
tags: [cache,clear]
fullview: true
---

Larevelin yeni sürüüyle tüm cache temizleme artık daha kolay

{% highlight yaml %}

cmd ekranında 
  >>>php artisan optimize:cleare  

{% endhighlight %}

yada route sayfasında
ve daha sonra **/test** link adresine giderek komutu çalıştırmız oluyoruz.
{% highlight yaml %}


 Route::get('test',function(){
    Artisan::call('optimize:clear');
 });

{% endhighlight %}