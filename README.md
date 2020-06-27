# radio-group
Use &lt;radio-group> to enhance your radio inputs :smile: So much better than &lt;select> dropdowns!

Simple example:

``` html
<radio-group name="Payment">
  <radio-button value="Monthly" />
  <radio-button value="Annual" />
</radio-group>
```

becomes:

``` html
<div class="RadioGroup" role="radiogroup" aria-label="Payment">
  <label>
    <input type="radio" name="Payment" value="Monthly">
    Monthly
  </label>
  <label>
    <input type="radio" name="Payment" value="Annual">
    Annual
  </label>
</div>
```

All the attributes!:

``` html
<radio-group name="House" legend="Which house are you in?" class="myclass" columns="auto" maxheight="50vh" toggle required>
  <radio-button value="Griffindor" class="redgold" checked>
    <img />
    Some text
    <small>Some description</small>
  </radio-button>
  <radio-button value="Hufflepuff" class="yellowblack">
    <img />
    Some text
    <small>Some description</small>
  </radio-button>
</radio-group>
```

Should output:

``` html
<fieldset role="radiogroup" class="myclass RadioGroup -closed">
<legend>Which house are you in?</legend>
  <div class="RadioGroup-container -colAuto" style="max-height: 50vh; overflow-y: auto;>
    <label class="RadioButton -checked redgold">
      <input type="radio" name="House" value="Griffindor" required checked>
      <img />
      Some text
      <small>Some description</small>
    </label>
    <label class="RadioButton -notChecked yellowblack">
      <input type="radio" name="House" value="Hufflepuff" required>
      <img />
      Some text
      <small>Some description</small>
    </label>
  </div>
  <button expanded="false">Open</button>
</fieldset>
```
