# Matryoshka Loading Mixin

Defines a loading flag for elements that automatically take into account the loading state of its child elements.

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="demo/mixin/mixin-loader-element.html">
    <link rel="import" href="demo/mixin/non-mixin-loader-element.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<mixin-loader-element countdown="2000">
  <mixin-loader-element countdown="3000">1</mixin-loader-element>
  <mixin-loader-element countdown="5000" defer>
    <mixin-loader-element countdown="10000">1</mixin-loader-element>
  </mixin-loader-element>
</mixin-loader-element>
```
