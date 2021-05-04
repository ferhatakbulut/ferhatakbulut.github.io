---
layout: post
title: Rar parolası kaldırma (rar password remove) 
categories: [genel, çözüm]
tags: [rar, şifre]
fullview: true
---

Rarlı bir dosyanın şifreli olarak sürekli açılması can sıkan bir olay. Heleki internet
ortamında paylaşılan bir dosyanın rar şifresi konularak paylaşılmasına anlam vermiyorum!!!

Bu can sıkıcı durumu ortadan kaldırmak için 
<br>

**TÜRKÇE**
Araçlar > Aşivleri Döünüştür > Sıkıştırma > Genel > Parolayı Ayarla 
 
bölümünde parolayı boş bırakarak tamam diyoruz.

**ingilizce**
Tools > Convert Archives > Compression > General > Set Password > 

password line leave blank and ok

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