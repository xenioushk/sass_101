# Useful SASS commands.

## Define a SASS variable

```scss
$primaryColor: #edf0ec;
```

### Use example

```scss
.headline {
  color: $primaryColor;
}
```

## map-get function

Define an array for the font weights. Add the Key value pairs like JavaScript and PHP.

```scss
$font-weight: (
  "regular": 400,
  "medium": 500,
  "bold": 700,
  "extra-bold": 900,
);
```

### Use example

```scss
.heading {
  font-weight: map-get($font-weight, regular);
}
```
