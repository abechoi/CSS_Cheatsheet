# SASS

## Compile SASS -> CSS:
```
sass scss/styles.scss css/styles.css
```

## Compile automatically:
```
sass --watch scss/styles.scss:css/styles.css --style expanded --no-source-map
```

## Variables
```
$myColor: #ddd;
$sectionHeading: 24px;
```

## Nested Blocks
```
#main-nav{
  background: $deepBlue;
  ul{
    width: 100%;
  }
  li{
    float: left;
    width: 14%;
  }
}
```