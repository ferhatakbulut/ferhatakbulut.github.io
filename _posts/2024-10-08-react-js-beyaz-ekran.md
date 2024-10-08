---
layout: post
title: React js dosyasını derledikten sonra beyaz ekran sorunu
categories: [Genel,React]
tags: [ipucu,react]
fullview: true
---

React.js projemizi derledikten sonra build dizinindeki dosyaları başka yere taşıdıktan sonra 
index dosyasını çalıştırdığımızda beyaz ekran sorununu halletmek için; **package.json** dosyasına
aşağıdaki satırı ekledikten sonra tekrar derleyince hata gidicektir.



{% highlight yaml %}

    "homepage": ".",

{% endhighlight %}


Kolay gelsin.


