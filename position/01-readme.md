# Lean CSS Position

- link (https://www.youtube.com/watch?v=jx5jmI0UlXU)

## absolute

```css
.parent {
  background: lightblue;
}

.child-one {
  background: green;

  /* Eftersom .parent  default position:static;
 toopen av skärmen, ett element inuti någon överordnad
 behållare som det kan refererar till 
  position: absolute;
  
  för att ändra ett element så att positionerna något ab
  absolut eller relativt */

  /* Flytta ner 10px från toppen ,Flytta 20px från vänster till höger*/
  /* position: relative;
 top: 10px; 
 left: 20px;  */
}

.child-two {
  background: orange;
}

.child-three {
  background: pink;
}
```

## relativ och abosolute

- Föräldra till position:relativ
  vilket detta är vanligaste användningsfallet
  för position

- child position som absoluta positioselement
  är relativt till positinen relativ föräldra och
  det här är relativ är verkligen användbar,

```css
.parent {
  background: lightblue;
  position: relative;
}

.child-one {
  background: green;
  position: absolute;
}

.child-two {
  background: orange;
}

.child-three {
  background: pink;
}
```

## position:absolute och position:absolute

- Du kan se fortfarande att ett element
  är relativt till föräldra eftersom föräldern
  har någon annan position än statisk och
  det är verkligen viktigt.

- när du har en annan position än statiska
  absolut element, vi använder det som
  förälder som det är absolut placerat inuti

```css
.parent {
  background: lightblue;
  position: absolute;
}

.child-one {
  background: green;
  position: absolute;
}

.child-two {
  background: orange;
}

.child-three {
  background: pink;
}
```

- så ta bort föräldra position:absolute;

- ändra till föräldra position:relative;

```css
.parent {
  background: lightblue;
  position: relative;
}

.child-one {
  background: green;
  position: absolute;
}

.child-two {
  background: orange;
}

.child-three {
  background: pink;
}
```
