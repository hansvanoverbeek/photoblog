---
layout: default
title: Contact
description: Een contactformulier voor uw bericht. A contact form for your message.
permalink: /contact/
---

<section class="portfolio-container">
 <h3>Your message is welcome</h3>
  <form action="https://formspree.io/havov@live.nl"
      method="POST">
    <fieldset>
      <label>Enter your Name:</label>
      <input type="text" name="name">
      <label>Enter your Email:</label>
      <input type="email" name="_replyto">
      <label>Your message:</label>
      <input id="text" type="textarea" name="text" maxlength="500" placeholder="U heeft max 500 tekens voor uw bericht">
      <input id="submit" type="button" value="Send">
      </fieldset>
  </form>
</section> 