CSS-Curved-Corners
==================

CSS technique that manipulates #div margins to create a box with curved corners without using images. Also supports transparency to work on all backgrounds.

The technique was used prior to the CSS3 rounded corners option. However, it can still be used to manipulate margins for other designs.

Info: Works in Internet Explorer, Firefox, and all latest browsers. And is 100% resizable.

The CSS
==================

<style type=”text/css”>

/* ::Please do not remove this:: This is a CSS curved corner technique that doesn’t use images and supports transparency. By Salim Chedrawi. www.salimchedrawi.com */

.container { color:#000 ;margin:3px 15px; } <!– Change the px accordingly –>
.rtop, .rbottom{
display:block;
}
.rtop *, .rbottom *{
display: block;
height: 1px;
overflow: hidden;
background:#fff; /* Choose color here for top and bottom */
}
.r1{margin: 0 5px}
.r2{margin: 0 3px}
.r3{margin: 0 2px}
.r4{margin: 0 1px; height: 2px}
.fff {background:#fff;} /* Choose color here for body */

</style>

The Html
==================

<table width=”100%” height=”100%” border=”0?> <!– Change width and height to resize the box. YOU CAN ALSO USE A DIV instead of table (configure height and width using the DIV style) –>
<tr><td>
<div class=”container”>
<b class=”rtop”><b class=”r1?></b> <b class=”r2?></b> <b class=”r3?></b> <b class=”r4?></b></b>
<div class=”fff”> This is a test </div>
<b class=”rbottom”><b class=”r4?></b> <b class=”r3?></b> <b class=”r2?></b> <b class=”r1?></b></b></div>
</td></tr>
</table>

Extra
==================

If you wish to insert a table between <div class=”fff”> </div>, then please be advised that setting the width of the table to 100% will work in Firefox, but will not work in Internet Explorer. So, in order for it to work on both web browsers, set the table width to a specific length (example: 200px).