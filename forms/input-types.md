---
title: Native HTML5 Input types
---

<form action="#" method="get">
  <h2>Input <code>type</code></h2>
  <p>Examples of native HTML5 input types:</p>
  <ul>
    <li>Accessibility</li>
    <li>Mobile dynamic keyboard</li>
    <li>Auto complete</li>
    <li>Client-side validation</li>
    <li>Input masking</li>
  </ul>
  <p>
    <label>
      Email
      <input type="email" id="email" value="">
    </label>
  </p>
  <p>
    <label>
      Telephone
      <input type="tel" id="mobile" value="">
    </label>
  </p>
  <p>
    <label>
      URL
      <input type="url" id="url" value="">
    </label>
  </p>
  <p>
    <label>
      Spinner
      <input type="number" id="counter" value="" min="0" max="12">
    </label>
  </p>
  <p>
    <label>
      Slider
      <input type="range" name="slider" id="slider" value="0" min="-100" max="100" step="10">
    </label>
    <output for="slider"></output>
  </p>

  <p>
    <label>
      Date
      <input type="date" id="date" value="">
    </label>
  </p>
  <p>
    <label>
      Time
      <input type="time" id="time" value="">
    </label>
  </p>
  <p>
    <label>
      Search
      <input type="search" id="search" value="">
    </label>
  </p>
  <p>
    <label for="combo">Combobox</label>
    <input id="combo" list="list1">
    <datalist id="list1">
      <option value="aardvark">
      <option value="absolute">
      <option value="abscond">
      <option value="admit">
      <option value="adrift">
      <option value="aesop">
      <option value="affect">
    </datalist>
  </p>
  <p>
    <label>
      Select
      <select id="select">
        <option value="0">Select One</option>
        <option value="1">January</option>
        <option value="2">February</option>
        <option value="3">March</option>
        <option value="4">April</option>
        <option value="5">May</option>
        <option value="6">June</option>
        <option value="7">July</option>
      </select>
    </label>
  </p>
  <fieldset>
    <legend>Are you ok?</legend>
    <label><input name="emotion" type="radio" value="Well" checked>Yes</label>
    <label><input name="emotion" type="radio" value="Unwell">No</label>
  </fieldset>
  <fieldset>
    <legend>Spices</legend>
    <label><input type="checkbox" value="salt">Salt</label>
    <label><input type="checkbox" value="pepper">Pepper</label>
    <label><input type="checkbox" value="curry">Curry</label>
  </fieldset>
</form>
