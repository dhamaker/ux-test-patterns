---
title: Forms
---

<p>Inputs use <code>&lt;p&gt;</code> semantics following examples in HTML 5 spec.</p>
<form action="#" method="get">
  <h2>Label structure comparison: parent vs sibling</h2>
  <p>
    <label>
      Parent
      <input type="text" id="labelParent1" value="">
    </label>
  </p>
   <p>
    <label>
      Parent plus
      <input type="text" id="labelParent2" value="">
      <small>Additional label</small>
    </label>
  </p>
  <p>
    <label for="labelSibling">Sibling</label>
    <input type="text" id="labelSibling" value="">
  </p>
  <p>
   <label id="siblingLabel3" for="labelSibling3">Sibling plus</label>
   <input type="text" id="labelSibling3" aria-labelledby="siblingLabel3 instruction3" value="">
   <small id="instruction3">ARIA label</small>
  </p>
  <p>
    <label for="labelSibling2">Sibling plus</label>
    <input type="text" id="labelSibling2" aria-describedby="instruction2" value="">
    <small id="instruction2">ARIA description</small>
  </p>  
  
</form>

<form action="#" method="get">
  <h2>Input <code>type</code></h2>
  <p>Parent labels used to minimize coding. HTML types  have native support for:</p>
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
      Counter
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
    <label>
      Autofilter list
      <input type="text" list="myList" id="alpha" />
      <datalist id="myList">
       <option value="aardvark">
       <option value="absolute">
       <option value="abscond">
       <option value="admit">
       <option value="adrift">
       <option value="aesop">
       <option value="affect">
     </datalist>
    </label>
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
    <label><input name="emotion" type="radio" value="Well" checked />Yes</label>
    <label><input name="emotion" type="radio" value="Unwell" />No</label>
  </fieldset>
  <fieldset>
    <legend>Spices</legend>
    <label><input type="checkbox" value="salt" />Salt</label>
    <label><input type="checkbox" value="pepper" />Pepper</label>
    <label><input type="checkbox" value="curry" />Curry</label>
  </fieldset> 
</form>
