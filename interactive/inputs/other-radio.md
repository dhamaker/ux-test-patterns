---
title: Radio Set with conditional subfield
---
# {{page.title}}

<style>
  #other ~ #favoriteCity {display:none;}
  #other:checked ~ #favoriteCity {display:inline-block;}
</style>

<form action="#" method="get">
  <fieldset>
    <legend>What is your favorite city?</legend>
    <p>
      <input id="nyc" name="favoriteCity" type="radio" value="newyorkcity">
      <label for="nyc">New York City</label>
    </p>
    <p>
      <input id="sf" name="favoriteCity" type="radio" value="newyorkcity">
      <label for="sf">San Francisco</label>
    </p>
    <p>
      <input id="other" name="favoriteCity" type="radio" value="newyorkcity">
      <label for="other">Other</label>
      <input id="otherCity" type="text" name="otherCity" value="" title="Favorite city">
    </p>
    <p>
      <input id="none" name="favoriteCity" type="radio" value="newyorkcity">
      <label for="none">None, cities suck!</label>
    </p>
  <fieldset>
</form>
