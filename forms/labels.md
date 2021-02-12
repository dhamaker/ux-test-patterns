---
title: Input labels
---

<p>Inputs use <code>&lt;p&gt;</code> semantics following examples in HTML 5 spec.</p>

<form action="#" method="get">
  <h2>Input labels</h2>
  <p>A 'parent' label wraps the input in a <code>&lt;label&gt;</code> element.  A 'sibling' label uses the label's <code>for</code> attribute to reference the sibling id.</p>
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
    <label for="sibling2">Sibling</label>
    <input type="text" id="sibling2" value="">
  </p>
  <p>
    <label id="sibling3Label" for="sibling3">Sibling</label>
    <input type="text" id="sibling3" aria-labelledby="sibling3Label instruction3" value="">
    <small id="instruction3">with ARIA labelled by</small>
  </p>
  <p>
    <label for="labelSibling2">Sibling</label>
    <input type="text" id="labelSibling2" aria-describedby="instruction2" value="">
    <small id="instruction2">with ARIA description</small>
  </p>
</form>
<form id="query" action="#" method="get">
  <p>
    <input placeholder="keyword" type="search" id="sibling2" value="" title="Label by title">
  </p>
  <button type="submit">Search</button>
</form>
