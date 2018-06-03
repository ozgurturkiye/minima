---
layout: post
author: "Özgür Bayraktaroğlu"
---

Bugün hatta son bir iki gün tekrardan `Jekyll` ve `GitHub Pages` kullanımı ile uğraştım. Şuan ruby ve jekyll altyapısını kullanıp bundan iğriti olur mu insan ahanda ben oldum. GNU/Linux Mint üzerinde `ruby` kurmak onun üzerinde `RubyGems` onun üzerinde `bundler` ve onunla birlikte `jekyll` kurulumu nasıl bir keyif veriyor anlatılamaz. Ek olarak kurulum belgelerini okumaya üşenip hızlı ilerleyince gelen hatalar beni çok yordu. Ruby'nin Linux paket yöneticisi üzerinde güncel paketi neden olmaz, güncel kararlı sürümü kurmak için neden fazladan ek araçlara ihtiyaç olur anlamış değilim. Burada `python3` e atıfta bulunarak gözünü seveyim diyorum.

Sonuç olarak uzun uğraşlar sonunda, hem yerelde çalışan hemde GitHub Pages ile sorunsuz çalışan bir jekyll kurulumu başardım. En zorlayan ve hata veren kısım bundler ile bağımlılıkları hatasız kurmak oldu bir de Rubyi kaynak koddan derleme uğraşları var tabi :) Sonuç kaynak koddan derlemeden vaz geçtim ve eski sürümü paket yöneticisi ile kurmak oldu. Sorunsuz kullandığım tema `minima` oldu bunu da ekleyelim.

Jekyll kendi sitesinde kurulumu şöyle güzel 3 satır komutta anlatmış:

{% highlight ruby %}
gem install bundler jekyll
jekyll new my-awesome-site
cd my-awesome-site
bundle exec jekyll serve
# => Now browse to http://localhost:4000
{% endhighlight %}

Web sitesini incelemek için: [Jekyll docs][jekyll-docs]
GitHub sayfası için: [Jekyll’s GitHub repo][jekyll-gh].
Sorular için: [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
