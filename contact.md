---
layout: default
title: Contact
description: Een contactformulier voor uw bericht. A contact form for your message.
permalink: /contact/
---

<main>
<h3 class="text-center">Uw bericht wordt op prijs gesteld</h3>
<h5 class="text-center">Your message is welcome</h5>
  <form action="https://formspree.io/havov@live.nl" method="POST">
    <fieldset>
      <label>Uw naam: | Enter your Name:</label>
      <input type="text" name="name">
      <label>Uw email: | Enter your Email:</label>
      <input type="email" name="_replyto">
      <label>Uw bericht: | Your message:</label>
      <input id="text" type="textarea" name="message" maxlength="500" placeholder="U heeft max 500 tekens voor uw bericht">
      <input id="submit" type="submit" value="Verstuur | Send">
      </fieldset>
  </form>
</main>
