---
title: Buttons
---

<p>Inputs use <code>&lt;p&gt;</code> semantics following examples in HTML 5 spec.</p>
<form action="# method="get">
  <h2>Label structure comparison: parent vs sibling</h2>
  <p>
    <label>
      Parent
      <input type="text" id="labelParent" value="">
    </label>
  </p>
  <p>
    <label for="labelSibling">Sibling</label>
    <input type="text" id="labelSibling" value="">
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
      Autocomplete/filter List
      <input list="autocomplete id="alpha">
    </label>
    <datalist id="autocomplete">
      <option value="aardvark">
      <option value="absolute">
      <option value="abscond>"
      <option value="admit>"
      <option value="adrift>"
      <option value="aesop>"
      <option value="affect>"
  </p>
</form>
