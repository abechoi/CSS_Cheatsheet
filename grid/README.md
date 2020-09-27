# CSS GRID

Set display to grid
```
display: grid;
```

Grid columns and rows
```
grid-template-columns: 33.3% 33.3% 33.3%;
grid-template-columns: 1fr 1fr 1fr;
grid-template-columns: repeat(3, 1fr);
grid-template-rows: repeat(4, minmax(150px, auto));
```

Grid start and end
```
grid-column-start: 1;
grid-column-end: 2;
grid-column: 1 / 2;
grid-column: span 3;
```

Grid gap
```
grid-column-gap: 10px;
grid-row-gap: 10px;
grid-gap: 10px;
```