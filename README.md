### Name of selectors for componentes
```
.MyComponent {}
.MyComponent.is-animating {}
.MyComponent--modifier {}

.MyComponent-part {}
.MyComponent-anotherPart {}
```

### Structure of components with Sass
```
@import 'variables';

.Container{
  background: $color-container;
  border-radius: $container-radius;
  overflow: auto;
  padding: 0 15px;
  box-shadow: $container-shadow;

  &-heading{
    display: inline-block;
    margin: 0 0 12px 0;

    & h2{
      font-size: 18px;
    }
  }

  &-body{
    display: block;
    padding: 6px 0;
  }

  &-footer{
    padding: 12px 0;
  }
}

```

### Using modular media-queries in components
```
.Section{
  border-bottom: 1px solid $border-color;
  padding: 0 0 35px 0;

  &-header{
    padding: 15px 0 10px;
    overflow: auto;
  }

  &-title{
    font-family: $font-title;
    font-size: 20px;
    letter-spacing: 1px;
    line-height: 1.1em;
    text-align: left;
    float: left;
    margin-top: 0;
    margin-bottom: 10px;
    @include mobile{
      text-align: center;
      float: none;
    };

    &:hover{
      color: $grey;
      text-decoration: underline;
    }
  }
```
