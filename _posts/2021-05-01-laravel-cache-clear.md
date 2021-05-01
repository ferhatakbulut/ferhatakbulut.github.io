---
layout: post
title: Larvel cache clear (laravel tüm cache temizleme) 
categories: [laravel, programming]
tags: [cache,clear]
fullview: true
---

Larevelin yeni sürüüyle tüm ccahe temizleme artık daha kolay

{% highlight yaml %}

cmd ekranında 
  >>>php artisan optimize:cleare  

{% endhighlight %}

yada route sayfasında

{% highlight yaml %}


 Route::get('test',function89{
	Artisan::call('optimize:clear');
 });

{% endhighlight %}