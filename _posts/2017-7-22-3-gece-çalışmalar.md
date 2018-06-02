---
layout: post
title: Kursun 3. gecesi notları!
---

## Çalışmalar iki ayrı proje olacak şekilde planlandı.
### my_class ve my_try dizinleri altında çalışılacak

1. İlk olarak iki ayrı dizin oluşturulup my_class ve my_try içerilerine virtulenviroment kurulur.
   1. **virtualenviroment kurulum** : my_class dizini içine `python3 -m venv env_class`
   1. **virtualenviroment kurulum** : my_try dizini içine `python3 -m venv env_try`
   1. **virtualenviroment aktif etme** : `. env_class/bin/activate` __veya__ `source env_try/bin/activate`
2. **django kurulum** : `pip install django`
3. **django projesi oluşturma** : `django-admin startproject mysite`
4. **veritabanını migrate etme** : `python manage.py migrate` veye `./manage.py migrate`
5. **django'yu ayağa kaldırma** : `python manage.py runserver` veya `./manage.py runserver`
6. **Önemli**: Bundan sonra iki ayrı django projesini aynı bilgisayarda çalıştıracağımız için **my_class** altındaki projeyi standard olan **8000** portundan **my_try**'ı ise **4000** portundan yayına sokacağız. O sebepten **my_try** dizini içerisindeki django'yu `python manage.py runserver 127.0.0.1:4000` şeklinde çalıştıracağız. Not: jekyll server'ı da 4000'den ayarlamışız :)
7. **admin panel için superuser oluşturma** : `./manage.py createsuperuser`
   1. Bu arada userı admin parolayı da unutmayacağınız bişeyler yaparsan güzel olur. Ayrıca basit parolalara izin verilmez.
8. my_class proejesi için **blog** isim yeni bir uygulama oluşturalım : `./manage.py startapp blog`
9. manage.py'ın yanına *requirement.txt* dosyasını oluşturalım.
   1. _requirement.txt_ dosyasının içerisine, *django>=1.11,<1.12* yazalım.
   2. **requirementsleri** kuralım : `pip install -r requirements.txt`
10. Uygulamayı settings içine ekleyelim : `mysite/settings.py` dosyasının içinde installed apps bölümüne **blog** u da ekliyoruz.
1. **templates** ve **static** dizinlerini ve içerisine gereken dosyaları olşuturalım.
   1. **blog** dizini altına **templates** onun altına **blog** onun altına **base.html** ve böyle devam eder.
   1. **blog** dizini altında ki **static** altındaki __css__ dizini altına **tema.css**
   1. **blog** dizini altında ki **static** altındaki __js__ dizini altına **tema.js** ve böyle devam eder.
2. Artık genel yapıyı oluşturduğumuza göre sürüm takibi de başlatabiliriz. Bunu başta da başlatabilirdik daha iyi olurdu :). Sürüm takibi başlatmak için **my_class/mysite** dizini altında `git init` diyerek başlatabiliriz. Not: `.gitignore` dosyasını düzenleyerek `db.sqlite3` ve başka takip etmesini istemediğiniz dosyaları ekleyebilirsiniz.
3. **Temel blog sitesi için ayarlar** [Django at glance](https://docs.djangoproject.com/en/1.11/intro/overview/)
