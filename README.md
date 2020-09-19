# SASS

## Compile SASS -> CSS:
```
sass scss/styles.scss css/styles.css
```

## Compile SCSS automatically:
```
sass --watch scss/styles.scss:css/styles.css --style expanded --no-source-map
```

## Compile multiple SCSS automatically:
```
sass --watch scss/styles.scss:css/styles.css scss/reset.scss:css/reset.css --style expanded --no-source-map
```

## Variables
```
$myColor: #ddd;
$sectionHeading: 24px;
```

## Nested Styles
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

## Mixins
```
@mixin banner{
  width: 100%;
}
.lead-banner{
  @include banner;
}
```

## Import Files
```
@import "reset";
@import "variables";
@import "mixins"; 
```