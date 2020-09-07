# Drag And Drop

DAD interface in Vanilla JS

### index.html
------

To drag an html element, set attribute draggable as true in html tag

### style.css
------

To show different effect while dragging, change opacity of the dragging element

### script.css
------

Get all draggable Contents present (i.e., HTML tags with class draggable, also set those elements draggable attribute as true)

`const draggables = document.querySelectorAll(".draggable");`

Get all containers present 

`const containers = document.querySelectorAll(".container");`

Set event listeners to monitor dragging action

For start of drag `dragstart` event and for end of drag `dragend`.

Event Listeners

```javascript
draggables.forEach((draggable) => {
  draggable.addEventListener("dragstart", () => {
    draggable.classList.add("dragging");
  });

  draggable.addEventListener("dragend", () => {
    draggable.classList.remove("dragging");
  });
});```

