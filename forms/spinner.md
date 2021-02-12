---
title: Input type=number
---
# {{page.title}}
Creating spinners using HTML5 native input type=number.

<form>
  <style>
    .spinner input:before {content:"-"};
    .spinner input:after {content:"+"};    
  </style>
  <p>
    <label for="noStyle">Number, no style</label>
    <input id="noStyle" name="count" type="number" min="0" max="10"  value="0">
  </p>
  <p class="spinner">
    <label for="styled">Number, no style</label>
    <input id="styled" name="countStyled" type="number" min="0" max="10"  value="0">
  </p>
</form>
