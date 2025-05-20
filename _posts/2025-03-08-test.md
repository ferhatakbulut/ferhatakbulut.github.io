---
layout: post
title: Laravel Projemizi Kurarken git ve zip problemi
categories: [Genel,Laravel,Php]
tags: [hata,laravel,git,zip]
fullview: true
---

Laravel projemizi kurarken aşağıdaki hata ile karşılaşırsak


{% highlight yaml %}

	Failed to download laravel/laravel from dist: The zip extension and unzip/7z commands are both missing, skipping.
The php.ini used by your command-line PHP is: C:\xampp\php\php.ini
    Now trying to download from source

In GitDownloader.php line 82:

  git was not found in your PATH, skipping source download

{% endhighlight %}

Yapmamız gereken **php.ini** dosyasını açıp **extension=zip** başındaki **;** kaldırmak. Sonra xampp ı yeninde başlatınca
laravel kurulumuz başarılı bir şekilde tamamlanacaktır.

Kolay gelsin.


