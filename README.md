# Travelport Styles

Package for everything styles-related. Includes fonts and icons too.

# How to use

All files in the root of this package are expected to be loaded in all Travelport sites,

```html
<head>
  <link href="reset.css" rel="stylesheet">
  <link href="main.css" rel="stylesheet">
  <link href="icons.css" rel="stylesheet">
</head>
```

Additional styles specific to a project may be appended to these,

```html
<head>
  <link href="reset.css" rel="stylesheet">
  <link href="main.css" rel="stylesheet">
  <link href="icons.css" rel="stylesheet">
  <!-- additional styles -->
  <link href="smartpoint.css" rel="stylesheet">
  <link href="modules.css" rel="stylesheet">
</head>
```

When creating a component, assume that the necessary styles have already been provided on the page.

If a component requires a specific style, the style should draw inspiration from these basic styles. The style for that component should then be inserted into a stylesheet that handles all the components. For example, using css modules and webpack, all module styles should be included into `webpacked-styles.css`, but styles used by the application, such as a new color that is used by many of the components or for a particular notification background that is not part of the basic color palette, should go into `trip-quotes.css`.

When creating a new component, you should load the three default styles, and insert all component specific styles into another stylesheet called `modules.css`. If you rely on styles specific to the product the component is for, you should too load the styles for the specific product, such as `smartpoint.css`.

## Colors

## Fonts

## Icons
