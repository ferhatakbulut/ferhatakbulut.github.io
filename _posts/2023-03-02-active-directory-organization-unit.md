---
layout: post
title: json return null problemi
categories: [Genel,Çözüm,İpucu,Json,Php,Larevel]
tags: [ipucu,php,json,laravel]
description: file get content ile sayfa içeriğini json_encode ile çevirdikten sonra diğer sayfada json_decode ile array olarak döndürürken alınan null hatası
---

Problemin asıl sebebi utf-8 probleminde kaynaklı. Ben kodlamamı **notpead ++** ile yaptığım için aşağıdaki yolu izeleyerek
çözdüm. Yapmanız gereken resimdeki gibi


<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/not.png">


1. **ANSI' ye Dönüştür** tıklamak sonra
2. **UTF-8' e Dönüştür** tıklamak

İşlem bukadar.

Örnek Kod Yapısı

{% highlight yaml %}

    $data=array('ad'=> $ad,'soyad'=> $soyad);
    echo json_encode($data);

{% endhighlight %}


{% highlight yaml %}

    $arrContextOptions=array("ssl"=>array("verify_peer"=>false,"verify_peer_name"=>false,),);  

    $response = file_get_contents("https://www.ornek.com", false, stream_context_create($arrContextOptions));
    echo $response;

{% endhighlight %}



Kolay gelsin.

