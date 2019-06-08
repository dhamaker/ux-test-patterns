---
title : Required attribute
---
# {{page.title}}

<form action="https://example.com/search-engine" method="post">
  <label>
    Query
    <input id="q" name="q" type="search" required value="" title="Enter search terms">
  </label>
  <button type="submit">Search</button>
</form>

~~~
<form action="https://example.com/search-engine" method="post">
  <label>
    Query
    <input type="search" required value="" title="Enter search terms">
  </label>
  <button type="submit">Search</button>
</form>
~~~

<script>
  document.write('<p>valueMissing: ' & q.validity.valueMissing & '</p><p>badInput: '&q.validity.badInput & '</p><p>customError: ' & q.validity.customError & '</p><p>patternMismatch: '& q.validity.patternMismatch & '</p><p>typeMismatch: ' & q.validity.typeMismatch & '</p><p>valid: ' & q.validity.valid & '</p>');
</script>

## Expectation
User is unable to submit an empty search request.  An onSubmit event will fail and the useragent will prompt the user to fill out the field.
