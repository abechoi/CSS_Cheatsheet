# SASS

## Install SASS:
```
npm install -g sass
```

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

## Variables:
```
$myColor: #ddd;
$sectionHeading: 24px;
```

## Nested Styles:
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

## Mixins:
```
@mixin banner{
  width: 100%;
}
@mixin grid($cols, $mgn){
  float: left;
  margin-right: $mgn;
  margin-bottom: $mgn;
  width: ((100% - (($cols - 1) * $mgn)) / $cols );
  &:nth-child(#{$cols}n){
    margin-right: 0;
  }
}
.lead-banner{
  @include banner;
}
#projects li{
  @include grid(4, 2%);
}
```

## Import Files:
```
@import "reset";
@import "variables";
@import "mixins"; 
```

## Psuedo Classes:
```
a{
  &:hover{
    color: red;
  }
}
```

## Math Operators
```
li{
  width: (100% / 3);
}
```