# grid-overlay

This code will add an adaptive grid overlay to your page.

## Install:

1. link `grid-overlay.css` as an external style or copy and paste source code in your own styles.
2. just add the `grid-overlay` class to the element in which you want to display the grid
 
Example:
```html
<body class="grid-overlay"></body>
```
or
```html
<div class="wrapper grid-overlay"></div>
```
3. Enjoy adaptive grid overlay.


## Setting up the grid:
  `--grid-indent` - margins on the edges of the grid
  
  `--grid-gap` - distance between columns
  
  `--columns-count` - number of columns
  
  `--columns-color` - column color
  
  ## media queries example
  
  ```css
  @media (max-width: 767px) {
  .grid-overlay::before {
    --columns-count: 4;  //set 4 columns
    --grid-indent:0;     //set zero margins on the edges of the grid
  }
}

@media (min-width: 768px) {
  .grid-overlay::before {
    --columns-count: 8;  //set 8 columns
  }
}

@media (min-width: 1024px) {
  .grid-overlay::before {
    --columns-count: 12;  //set 12 columns
    --grid-gap: 24px;     //set the distance between the columns to 24px
    --grid-indent: 16px;  //set the margins at the edges of the grid to 16 pixels
  }
}
```

## Screenshot
  ![image](https://user-images.githubusercontent.com/26135033/129493451-5de61778-ca1b-4761-9540-4338b5fcc7d7.png)
