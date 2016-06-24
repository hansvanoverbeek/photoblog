---
layout: default
title: Contact
description: Een contactformulier voor uw bericht. A contact form for your message.
permalink: /contact/
---

<main>
 <h3>Your message is welcome</h3>
  <form action="post">
    <fieldset>
      <label for="">Enter your Name:</label>
      <input type="text" name="name">
      <label for="">Enter your Email:</label>
      <input type="email" name="email">
      <label for="">Your message:</label>
      <input id="text" type="textarea" name="text" maxlength="500" placeholder="U heeft max 500 tekens voor uw bericht">
      <input id="submit" type="button" name="submit" value="Submit">
      </fieldset>
  </form>
</main>