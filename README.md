# CSS-Selectors
## subsequent sibling
<table>
<tr>
<td valign="top" width=450>

HTML:
```html‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ 
<div id="container">
  <p>This is #1</p>
  <p>This is #2</p>
  <div>
    <p>This is #3</p>
  </div>
</div>

<p>This is #4</p>
<p>This is #5</p>
```
CSS:
```css
#container {
  border: 2px solid;
}

#container ~ p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width = 100% src="https://github.com/user-attachments/assets/7d8170d5-8554-4c49-a680-405e00ac07d4" /> </td> </tr> </table>
