---
title: Radio Set with conditional subfield
---
# {{page.title}}
Is this an example of a radio sandwich?
<style>
  #other ~ #otherCity {display:none;}
  #other:checked ~ #otherCity {display:inline-block;}
  #none ~ #alternate {display:none;}
  #none:checked ~ #alternate {display:none;}
</style>

<form action="#" method="get">
  <fieldset>
    <legend>What is your favorite city?</legend>
    <p>
      <input id="nyc" name="favoriteCity" type="radio" value="newyorkcity" required>
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
      <fieldset id="alternate">
        <legend>I'd rather be...</legend>
        <p>
          <label for="altActivity">Activity</label>
          <input id="altActivity" type="text" name="altActivity">
        </p>
        <p>
          <label for="altLocation">Location</label>
          <input id="altLocation" type="text" name="altLocation">
        </p>
      </fieldset>
    </p>
    <p>
      <input id="null" name="favoriteCity" type="radio" value="null">
      <label for="null">No comment</label>
    </p>    
  </fieldset>
  <button type="submit">Vote</button>
</form>
