---
layout: post
title: Kim milyoner olmak ister oyunu yazma denemeleri notları!
date: 2018-03-23 Cuma
---

## Django ile kim milyoner olmak ister oyunu üzerine denemeler.

1. İlk olarak mysite dizini içine `python3 -m venv env_django` komutu ile bir sanal bir Python ortamı oluşturulur.
2. Python sanal ortam aktif edelir `. env_django/bin/activate`
3. Sanal ortam içine django kurulur `pip install django`
4. Proje başlatılır `django-admin startproject mysite .` sonda nokta koyduk sebebi bulunduğumuz dizinin içine oluşturmak istememiz
5. Sunucu ayağa kaldırılır `python manage.py runserver` Bir terslik yoksa `http://127.0.0.1:8000/` tebrikler mesajı alırsın :)
6. Milyoner uygulaması oluşturulur. `python manage.py startapp milyoner`. Django'da uygulamalar app olarak geçiyor. Sonuçta `milyoner` adında taşınabilir bir uygulamamız olacak.
7. Uygulama settings içine installed apps bölümüne eklenir : mysite/settings.py dosyasının içinde installed apps bölümüne `milyoner` eklenir.
8. Veritabanı oluşturulur `python manage.py migrate`
9. Super kullanıcı oluşturulur `python manage.py createsuperuser`
10. Bundan sonraki değişiklikleri kaydetmek için de bir `git init` güzel olur. Tabi `.gitignore` dosyasını oluşturup takip edilmesini istemediğimiz dizin ve dosyaları içine eklemeyi unutmamak lazım.
11. https://ozgurturkiye.github.io/5-g%C3%BCn/ şuradan devam ederiz.
