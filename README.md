sass-css-grid
=============
<br />
CSS grid calculated with SASS
<br /><br />
This is a simple SASS that caluculates given values into specified grid. 
<br /><br />
<b>How to compile:</b><br />
1. set up $content-width - a default max width for your page in px (eg. 980px) <br />
2. set up $spans - as a number of 'columns' you want your grid to be divided into (eg. 16) <br />
3. set up $spacing and $padding (both optional) - $spacing as a margin between columns and $padding as padding between them (eg. 20px).
    In my example I set $spacing: $base-gutter; because I have already prepared $base-gutter variable as a base value for margins and paddings throught the page.
<br /><br />
<b>How to use in HTML:</b><br />
1. use #content or .content-grid for main holders<br />
2. use .row class for element containing row of specified columns (might be one .row for multiple rows though)<br />
3. put .span# class for every column: eg. if you set up your $spans to 16, and you want 2 columns, place two elements with .span8 class (eg. 2 divs) - and going further, if you want 4 columns with same width, create 4 elements with span(16/4) = that means .span4 class.<br />
4. You can create less columns and push them to right or to left in place of empty space by applying the class .push-l-#
  or .push-r-# where # is the number of spans divided by 2.
