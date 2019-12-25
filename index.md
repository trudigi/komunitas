---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
excerpt: Beranda TRUDIGI Community
---

Selamat datang di halaman komunitas TRUDIGI.

{% for category in site.data.toc %}
---
## {{ category.name }}
{{ category.excerpt }}

{% for article in category.articles %}
### [{{ article.name }}]({{ article.href }})
<small>{{ article.excerpt }}</small>

{% endfor %}
{% endfor %}
