# radio-group
Use &lt;radio-group> to enhance your radio inputs :smile: So much better than &lt;select> dropdowns!

``` html
<radio-group name="House" legend="Which house are you in?" class="myclass" toggle>
  <radio-button value="Griffindor" class="redgold" checked>
    <img />
    Some text
    <br />
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
<fieldset role="radiogroup" class="myclass RadioGroup -checked">
<legend>Which house are you in?</legend>
  <label class="redgold" class="redgold RadioButton -checked">
    <input type="radio" name="House" value="Griffindor" checked>
    <img />
    Some text
    <small>Some description</small>
  </label>
  <label class="yellowblack" class="yellowblack RadioButton -notChecked">
    <input type="radio" name="House" value="Griffindor">
    <img />
    Some text
    <small>Some description</small>
  </div>
</fieldset>
```
