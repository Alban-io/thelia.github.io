---
layout: home
title: Hooks List - Modules
sidebar: plugin
lang: en
subnav: plugin_hooks_list
---

<div class="page-header">
    <h1>Hooks : <small>list of hooks</small></h1>
</div>

<div class="alert alert-warning">
<p>This functionality is only available since version 2.1</p>
</div>


- [Front Office](#front-office)
- [Back Office](#back-office)
- [PDF](#pdf)


## Front Office

{% for files in site.data.hook_front %}
### {{ files[0] }}
    {% for hook in files[1] %}
- **{{ hook.code }}**: {{ hook.title }} 
    {% endfor %}
{% endfor %}

## Back Office

{% for files in site.data.hook_back %}
### {{ files[0] }}
    {% for hook in files[1] %}
- **{{ hook.code }}**: {{ hook.title }} 
    {% endfor %}
{% endfor %}

## PDF

{% for files in site.data.hook_pdf %}
### {{ files[0] }}
    {% for hook in files[1] %}
- **{{ hook.code }}**: {{ hook.title }} 
    {% endfor %}
{% endfor %}


