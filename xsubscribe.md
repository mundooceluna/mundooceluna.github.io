---
layout: page
title: suscríbete
alt_title: Suscríbete a mi blog
permalink: /subs_es/
lang: es
ref: subscribe
---

Introduce tu email si quieres seguir mi trabajo y mantenerte al día de los nuevos productos y promociones que vaya subiendo a la tienda.

<form class="wj-contact" action="https://formspree.io/{{site.subsemail}}" method="POST">
<input type="text" name="email" placeholder="Tu email">
<input type="hidden" name="_next" value="http://www.oceluna.com">
<input type="hidden" name="_subject" value="New Contact Form Submission">
<input type="text" name="_gotcha" style="display:none">
<input type="submit" value="Suscríbete">
</form>

<style>
form.wj-contact input[type="text"], form.wj-contact textarea[type="text"] {
    width: 100%;
    vertical-align: middle;
    margin-top: 0.25em;
    margin-bottom: 0.5em;
    padding: 0.75em;
    font-family: monospace, sans-serif;
    font-weight: lighter;
    border-style: solid;
    border-color: #444;
    outline-color: #2e83e6;
    border-width: 1px;
    border-radius: 3px;
    transition: box-shadow .2s ease;
}

form.wj-contact input[type="submit"] {
    outline: none;
    color: white;
    background-color: #2e83e6;
    border-radius: 3px;
    padding: 0.5em;
    margin: 0.25em 0 0 0;
    border: 1px solid transparent;
    height: auto;
}
</style>