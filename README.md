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

## Nesting

```scss
.heading {
  font-size: 1.5rem;

  #{&}__italic {
    font-style: italic;
  }
}
```

### Output

```css
.heading {
  font-size: 1.5rem;
}

.heading .heading_italic {
  font-style: italic;
}
```

## Include a partial .scss file

**@import** keyword is used to add the partial files to the main(styles.scss) scss file.

**Examples of partial files names**

- \_header.scss
- \_footer.scss
- \_variables.scss

[![Include a partial .scss file](previews/import_scss_partial_file.jpg)]
