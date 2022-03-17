---
layout: post
title: Laravel Login Sayfası
categories: [Laravel]
tags: [login,auth,page]
fullview: true
---
Laravel projemizde kullanıcı giriş sayfası(login page) için el ile tekrar yazmamıza gerek yoktur. Laravel in kendi 
kütüphanesinden yararlanarak hem güvenilir hemde hızlı bir şekilde oluşturabiliriz.

{% highlight yaml %}

    composer require laravel/ui:^2.4
    php artisan ui vue --auth
    npm install && npm run dev
    php artisan migrate

{% endhighlight %}

Satırlarnı komut satırından hangi larevel projesinde kullanacak isek, orada yazabiliriz.

{% highlight yaml %}

    php artisan migrate

{% endhighlight %}

**Not:** Bu kodu **php artisan migrate**  yazmadan önce projemizin veritabanını oluşturmalıyız.Bu komut ile veritanında kullanıcılar için 
tabloları otomatik olarak projemiz için laravel oluşturacaktır.

Kolay gelsin.

