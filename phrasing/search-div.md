---
title: Search Results 
---
<!--
  pattern: search-div
  rational:  result is an generic content block and is only needed for presentation.  result does not play a semantic purpose.
  data model:  title, link, description
  -->
# {{title}}

## Test Case

### <code>article</code> element
<article class="synopsis">
    <h1><a href="resource-address.html">Resource Title</a></h1>
    <p>Resource description</p>
</article>

### <code>div</div> wrapper
<div class="result">
    <h2><a href="resource-address.html">Resource Title</a></h2>
    <p>Resource description</p>
  </div>



## Code

```
<article class="synopsis">
    <h1><a href="resource-address.html">Resource Title</a></h1>
    <p>Resource description</p>
</article>

<div class="result">
    <h2><a href="resource-address.html">Resource Title</a></h2>
    <p>Resource description</p>
  </div>
```
