---
title: Advanced HTML Form Techniques
layout: default
---
# Advanced HTML 5.1 Forms Techniques

## Pattern Test Case

><form id="t3" action="#" method="get">
>  <p>
>    <label for="mobile">Mobile Phone</label>
>    <input type="tel" id="mobile" name="mobile" value="" required pattern="((\(\d{3}\))) ?\d{3}-\d{4}" autocomplete="tel" placeholder="(###) ###-####" title="Enter area code and phone number using parenthese and hyphen.  We will only use this phone number to protect access to your account.">
  </p>
>  <button type="submit">Test</button>
> </form>


## Code
```
<form id="t3" action="#" method="get">
  <p>
    <label for="mobile">Mobile Phone</label>
    <input type="tel" id="mobile" name="mobile" value="" required pattern="((\(\d{3}\))) ?\d{3}-\d{4}" autocomplete="tel" placeholder="(###) ###-####" title="Enter area code and phone number using parenthese and hyphen.  We will only use this phone number to protect access to your account.">
  </p>
      <button type="submit">Test</button>
</form>
```

## Presentation: NVDA on Firefox
### <code>onfocus</code> event
_Syntax:_

label + valid status + "edit" + required + title + placeholder + value

_Actual:_

> Mobile Phone edit required invalid  number has autocomplete Enter area code and phone number using parenthese and hyphen.  We will only use this phone number to protect access to your account. [pause] number number number [pause] number number number and four number blank.

### <code>oninvalid</code> event</h5>
_Syntax:_

"Alert: Please match the requested format:" + title

_Actual:_
> Alert: Please fill out this field.

> Alert: Please match the requested format: Enter area code and phone number using parenthese and hyphen.  We will only use this phone number to protect access to your account.</q>


## Advantages
  * HTML Standards no custom
  * Future scalable
  * Backward compatible.  Degrades gracefully, falling back to basic validation experience.


## Disadvantages
 * Additional markup and ARIA labeling
 * Hard for QA review and open to production copy and paste errors because copy is invisible.
 * Placeholder text may not be accessible to users with reduced vision.  Low color contrast may impact many of your users because eyes change as people age beginning in our 40s.
 * Placeholder value disappears once user begins typing, depriving them of a visual model, user will not be able to proof the format.
 * Preferred formats is less clear.  So higher error rates.
 * Consistent validation matching needs close integration between  publishing and form validation applications so front-end matches back-end instructions.


## Notes
* Must have server-side validation.  This is the starting point for user experience.
* Client-side validation should be used as progressive enhancement and guidance, not as data validation; it's function is to enhance the user experience, speed completion, reduce negative 'error' flows,  and increase conversions.  Forms can be easily hacked to bypass native validation and javascript enhancements.
* Use HTML 5.2 forms.  Older user agents should degrade gracefully.


## Input Attributes.
Help with proactive and reactive messaging.  Older user agents should ignore them and use the basic validation experiece (server-side)

* <code>maxlength</code>
* <code>minlength</code>
* <code>required</code>
* <code>pattern</code> fine grain validation matching using regex.
* <code>type</code> identifies the type of control the user agent will expose to the user.
* <code>autocomplete</code>  with the appropraite value.  identifies the values the input will represent.
* <code>title</code> tooltip and validation message
* <code>placeholder</code> enhancement for some users

## References
*  <a href="https://www.w3.org/TR/2017/REC-html52-20171214/sec-forms.html#clientside-form-validation">Client-Side Form Validation</a>
*   <a href="https://www.w3.org/WAI/tutorials/forms/">Web Accessibility Tutorials Forms</a>
