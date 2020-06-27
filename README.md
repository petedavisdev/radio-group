# radio-group
Use &lt;radio-group> to enhance your radio inputs :smile: So much better than &lt;select> dropdowns!

``` html
<radio-group name="House" legend="Which house are you in?" class="myclass" columns="auto" maxheight="50vh" toggle>
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
      <input type="radio" name="House" value="Griffindor" checked>
      <img />
      Some text
      <small>Some description</small>
    </label>
    <label class="RadioButton -notChecked yellowblack">
      <input type="radio" name="House" value="Griffindor">
      <img />
      Some text
      <small>Some description</small>
    </label>
  </div>
  <button>Open</button>
</fieldset>
```
