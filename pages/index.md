---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
title: "Donationsoperationssalen"
teaser: "Donationsoperationssalen vid Vävnadsbanken i Lund."
sidebar: right
lang: sv

widget1:
  url: './verksamheten/'
  title: "Donationsoperationssalen vid Vävnadsbanken i Lund"
  image: op.jpg
  text: 'På Vävnadsbanken finns en donationsoperationssal som fungerar som en experimentell operationssal med en tillhörande forskningsavdelning. '
widget2:
  url: './steg_for_steg/'
  title: "Forskning på donerade vävnader - steg för steg"
  text: 'Lathund för forskningsprojekt.<br/>1. Etikprövning<br/>2. Projektbeskrivning<br/>3. Avtal<br/>4. Utbildning.<br/>5. Försök.'
  image: heart.png
  #video: '<a href="#" data-reveal-id="videoModal"><img src="http://phlow.github.io/feeling-responsive/images/start-video-feeling-responsive-302x182.jpg" width="302" height="182" alt=""/></a>'
widget3:
  url: './utbildning/'
  title: "Utbildning"
  image: books.jpg
  text: 'För att få arbeta i donationsoperationssalen behöver du gå en utbildning'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: mailto:vavnadsbanken@skane.se
  text: Kontakta Vävnadsbanken ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---
{% assign header.title = "Hej" %}
<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
