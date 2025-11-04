# CSS Selectors
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

/* alle p's die in container zitten */
#container p { 
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img  width="456" height="368" alt="image" src="https://github.com/user-attachments/assets/6bda8acc-6b00-4a88-a4e6-98ffc8bd4a7d" /> </td> </tr> </table>

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

/* alle p's die directe kinderen zijn van container */
#container > p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img  width="456" height="368" alt="image" src="https://github.com/user-attachments/assets/bab5b229-c331-4bb3-a34f-c7c0af77dd47" /> </td> </tr> </table>

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

/* alle p's die directe siblings zijn van container */
#container ~ p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img  width="456" height="372" alt="image" src="https://github.com/user-attachments/assets/44dab9fc-99ae-4fcb-8831-410562af6f83" /> </td> </tr> </table>
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

/* alle p's die directe siblings zijn van container */
#container ~ p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img  width="456" height="378" alt="image" src="https://github.com/user-attachments/assets/46dfc602-8d5f-419d-a764-37b7eaa24cd7" /> </td> </tr> </table>

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

/* de eerste p die volgt op container */
#container + p {
  background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img  width="456" height="369" alt="image" src="https://github.com/user-attachments/assets/252e2203-047b-4048-b3ca-d36a830c612c" /> </td> </tr> </table>

## Pseudo class
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
<td valign="top" width=450> <img width="456" height="249"" src="https://github.com/user-attachments/assets/9756983b-8005-4318-8b54-a4737a0a7d1f" /> </td> </tr> </table>

## Pseudo element
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

#container p::first-letter {
    background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width="456" height="249" alt="image" src="https://github.com/user-attachments/assets/38412a4c-24e7-4885-ad27-8f0f519eaa5e" /> </td> </tr> </table>

## Join selector
<table>
<tr>
<td valign="top" width=450>

HTML:
```html‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ 
<body>
<div id="container">
    <p>This is #1</p>
    <p>This is #2</p>
    <div>
        <p class="highlight">This is #3</p>
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

/* alle p's om het even waar die de class highlight hebben */
p.highlight {
    background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width="456" height="249" alt="image" src="https://github.com/user-attachments/assets/43b90d12-fd2c-4716-bfea-a7b903e9f891" /> </td> </tr> </table>

## Attribute
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

/* alle p's die directe kinderen zijn van alle divs met een id */
div[id] > p {
    background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img width="456" height="249" alt="image" src="https://github.com/user-attachments/assets/48aff295-a620-4331-9255-ab5843d8bffc" /> </td> </tr> </table>

## Convoluted
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

/* zelfde resultaat als #container > p + p ~ div > p
of #container > p ~ div > p */
#container p ~ div p {
    background-color: hsl(60, 100%, 70%);
}
```
</td>
<td valign="top" width=450> <img  width="456" height="259" alt="image" src="https://github.com/user-attachments/assets/eb7c0245-ff20-4098-9656-b6bb25a37e15" /> </td> </tr> </table>
