---
layout: post
title: Jekyll yerel makina kurulum adımları
---

Canımız sıkıldı biraz jekyll üzerine birşeyler yazalım derken en basit olacak şekilde kurulum adımlarını yazayım dedim.

### jekyll kurulum

Tabi öncelikle bilgisayarınızda [Ruby](https://www.ruby-lang.org/en/downloads/) ve [RubyGems](https://rubygems.org/pages/download) kurulu olmalı.

1. `$ gem install jekyll bundler` : jekyll'ı kuruyoruz. (Buradaki gem ve bundler konuları da ayrı bir konu :) gem ruby için bir paket yöneticisi, bundler da Ruby'nin gem bağımlılıkları yönetir.) Kısaca gem ve bundlar jekyll'nin sorunsuz kululması için gerekli :)
2. `$ jekyll new my-awesome-site` : my-awesome-site isminde jekyll sitemizi oluşturuyoruz.
3. `$ cd my-awesome-site` : my-awesome-site dizinine giriyoruz.
4. `$ bundle exec jekyll serve` : Son olarak jekyll sunucusunu aktif ediyoruz.

Sonuç: # => Now browse to http://localhost:4000 adresinden jekyll sitemize ulaşabiliriz.

kaynak: [jekyll temel kurulum](https://jekyllrb.com/)
