## AttributeSelectors

### [rel=external] — Точное совпадение значения атрибута
```
  <h1 rel="external">Attribute Equals</h1>
  h1[rel=external] { color: red; }
```
### [rel*=external] — Атрибут содержит некоторое значение в любом месте
```
  <div id="third_post"></div>
  div[id*=post] { color: red; }
```
### [rel^=external] — Атрибут начинается с определенного значения
```
  <h1 rel="external-link yep">Attribute Begins</h1>
  h1[rel^=external] { color: red; }
  a[href^=http://perishablepress.com] { color: red; }
```
### [rel$=external] — Атрибут оканчивается определенным значением
```  
  h1[rel$=external] { color: red; }
  a[href$=#], a[href$=?] { color: red; }
```
### [rel~=external] — Атрибут содержит значение в списке разделенном пробелами
```
  <h1 rel="friend external sandwich">Attribute Space Separated</h1>
  h1[rel~=external] { color: red; }
```
### [rel|=external] — Атрибут содержит значение в списке разделенном тире
```
  <h1 rel="friend-external-sandwich">Attribute Dash Separated</h1>
  h1[rel|=external] { color: red; }
```
### [title=one][rel^=external] — Совпадение нескольких атрибутов
```
  <h1 rel="handsome" title="Important note">Multiple Attributes</h1>
  h1[rel=handsome][title^=Important] { color: red; }
```
