---
layout: post
title: Bazı Cmd Komutları
categories: [Windows,Cmd]
tags: [cmd,komutlar]
description: Bazı Cmd Komutları ve Açıklamaları
---


**Bazı Cmd Komutları**

{% highlight yaml %}

   -> tree /f                          -> Bulunduğu klasörün ağaç yapısını gösterir.
   -> taskkill /IM "explorer.exe" /F   -> explorer.exe kapat
   -> start explorer.exe               -> explorer.exe başlat
   -> taskkill /f /im chrome.exe       -> chrome.exe kapat 
   -> pskill \\10.99.0.19 chrome.exe   -> uzak bilgisayar chrome.exe kapat
   
   -> ipconfig /release                -> dhcp'den dagıtılan ip adresini geri bırakır.
   -> ipconfig /renew                  -> dhcp'den dagıtılan yeni ip adresi almaya yarar.
   -> ipconfig /flushdns               -> dns bellegini temizler.

{% endhighlight %}



<table border='1'>
	<tr>
	<th>Komut</th>
	<th></th>
	<th>Açıklama</th>
	</tr>
	<tr>
	<td>shutdown /r /m \\192.168.1.22</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan yeniden başlat</td>
	</tr>
	<tr>
	<td>shutdown /s /m \\192.168.1.22</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan kapat</td>
	</tr>

	<tr>
	<td>shutdown /s /m  \\192.168.1.22 /f /c "Selamlar"</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan kapatır ve ekranda mesaj gösterir</td>
	</tr>

	<tr>
	<td>msg /SERVER:192.168.1.22 * /TIME:60 "selamlar"</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan mesaj gönderir</td>
	</tr>
</table>


<br>

Çalıştır geçmişini temizleme komutu

{% highlight yaml %}

   reg delete HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\RunMRU /va /f

{% endhighlight %}



Kolay gelsin.

