---
title: Repeated input groups
---
<form action="#" method="get">
<h1>Your Family</h1>
  <fieldset id="uid-01">
    <legend>You</legend>
    <p>
      <label for="uid01Name">Name</label>
      <input id="uid01Name" type="text" name="uid01Name" value="Cy Jones">
    </p>
    <p>
      <label for="uid001DOB" title="Date of Birth">DOB</label>
      <input id="uid01DOB" type="date" name="uid01DOB" value="1991-01-01">
    </p>
  </fieldset>
  <fieldset id="uid002">
    <legend>Spouse</legend>
    <p>
      <label for="uid002Name">Name</label>
      <input id="uid002Name" type="text" name="uid002Name" value="Sam Jones">
    </p>
    <p>
      <label for="uid001DOB" title="Date of Birth">DOB</label>
      <input id="spouseDOB" type="date" name="spouseDOB" value="1992-01-01">
    </p>
  </fieldset>
  <fieldset>
    <legend>Dependent 1</legend>
    <p>
      <label for="dependent1Name">Name</label>
      <input id="dependent1Name" type="text" name="dependent1Name" value="Jai Jones">
    </p>
    <p>
      <label for="dependent1DOB" title="Date of Birth">DOB</label>
      <input id="dependent1DOB" type="date" name="dependent1DOB" value="2011-01-01">
    </p>
  </fieldset>
  <fieldset>
    <legend>Dependent 2</legend>
    <p>
      <label for="dependent2Name">Name</label>
      <input id="dependent2Name" type="text" name="dependent2Name" value="Jai Jones">
    </p>
    <p>
      <label for="dependent1DOB" title="Date of Birth">DOB</label>
      <input id="dependent2DOB" type="date" name="dependent2DOB" value="2011-01-01">
    </p>
  </fieldset>
  <buton type="submit">Save</button>
</form>
