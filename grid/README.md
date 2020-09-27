# CSS GRID

## Set display to grid
```
display: grid;
```

## Grid columns and rows
```
grid-template-columns: 33.3% 33.3% 33.3%;
grid-template-columns: 1fr 1fr 1fr;
grid-template-columns: repeat(3, 1fr);
grid-template-rows: repeat(4, minmax(150px, auto));
```

## Grid start and end
```
grid-column-start: 1;
grid-column-end: 2;
grid-column: 1 / 2;
grid-column: span 3;
```

## Grid gap
```
grid-column-gap: 10px;
grid-row-gap: 10px;
grid-gap: 10px;
```

## Grid Area
```
#content{
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: minmax(100px, auto);
  max-width: 960px;
  margin: 0 auto;
  grid-gap: 10px;
  grid-template-areas:
  "header header header header"
  "footer footer footer footer"
  "main main main main"
  "main main main main"
  "aside aside nav nav"
  "section section section section"
  "section section section section";
}
header{
  grid-area: header;
}
main{
  grid-area: main;
}
section{
  grid-area: section;
}
aside{
  grid-area: aside;
}
nav{
  grid-area: nav;
}
footer{
  grid-area: footer;
}
```