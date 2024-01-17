---
layout: page
title: Contact
permalink: /contact/
feature-img: "img/color.png"
---

Contact Page

<form id="form" action="https://submit-form.com/IqLH7voPN" method="post" data-botpoison-public-key="pk_536bd3c7-42fa-4e17-be49-d8dd64221d95" target="_blank">
  <input type='text' name='name' placeholder='Your Full Name' />
  <input type='email' name='email' placeholder='Your E-mail Address' />
  <textarea name='message' placeholder='Write your message ...'></textarea>
  <input id="submit" type='submit' value='Send Message' />
</form>

<script>
  var formElement = document.getElementById("form");
  var buttonElement = document.getElementById("submit");
  formElement.addEventListener("botpoison-challenge-start", function () {
    buttonElement.setAttribute("disabled", "disabled");
  });
  formElement.addEventListener("botpoison-challenge-success", function () {
    buttonElement.removeAttribute("disabled");
  });
  formElement.addEventListener("botpoison-challenge-error", function () {
    buttonElement.removeAttribute("disabled");
  });
</script>
