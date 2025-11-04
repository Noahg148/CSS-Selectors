# CSS-Selectors
## Descendant
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

#container p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width="439" height="368" alt="image" src="https://github.com/user-attachments/assets/6bda8acc-6b00-4a88-a4e6-98ffc8bd4a7d" /> </td> </tr> </table>

## Child
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

#container > p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width="438" height="368" alt="image" src="https://github.com/user-attachments/assets/bab5b229-c331-4bb3-a34f-c7c0af77dd47" /> </td> </tr> </table>

## Subsequent sibling
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
<td valign="top" width=450> <img width="443" height="372" alt="image" src="https://github.com/user-attachments/assets/44dab9fc-99ae-4fcb-8831-410562af6f83" /> </td> </tr> </table>
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

<div>
<p>This is #4</p>
<p>This is #5</p>
</div>
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
<td valign="top" width=450> <img width="438" height="378" alt="image" src="https://github.com/user-attachments/assets/46dfc602-8d5f-419d-a764-37b7eaa24cd7" /> </td> </tr> </table>

## Next sibling
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

#container + p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width="441" height="369" alt="image" src="https://github.com/user-attachments/assets/252e2203-047b-4048-b3ca-d36a830c612c" /> </td> </tr> </table>

## Pseudo classes
<table>
<tr>
<td valign="top" width=450>

HTML:
```html‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ 
<div id="container">
    <p>This is #1</p>
    <p>This is #2</p>
    <div>
        <p>This is <span>#3</span></p>
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

#container p:nth-child(even):hover + div p span {
    background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width="441" height="369" src="https://github.com/user-attachments/assets/99866799-b372-4f51-a032-506b82f92d3d" /> </td> </tr> </table>
