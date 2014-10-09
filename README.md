Premise
=======

Another CSS framework

Yes, Premise is just another CSS framework. The key thing about premise is that it is meant to avoid repetitive and redundant css by offering you a variety of classes that do all the most common things for you. To keep the framework lightweight we only focus on optimizing code for the most common structure and design elements people want and need. So with Premise you get two things: 1) Build layouts in minutes and easily create common elemnets like mobile navs, or form elemnets. 2) Get non-repetitive, non-redundant lightweight CSS and JS with most common UI/UX lements design and functionality. Integrated with Font Awesome.

<h1>Examples</h1>
<h3>Basic elements</h3>
These basic classes give you the most common attributes you probably write in CSS. Just by adding these classes to your elements you cut so much redundant CSS.
<pre>
&lt;!-- Basic classes --&gt;
&lt;!-- by simply adding these basic classes to any 
element in your HTML you can save yourself a lot
of time writing CSS --&gt;
&lt;!-- Give an element a display:block --&gt;
&lt;div class="block"&gt;
	&lt;span&gt;
		Hello!
	&lt;/span&gt;
&lt;/div&gt;
&lt;!-- CSS: text-align: left --&gt;
&lt;p class="left"&gt;This is aligned to the left&lt;/p&gt;
&lt;!-- CSS:text-align: right --&gt;
&lt;h3 class="right"&gt;Title aligned to the right&lt;/h3&gt;
&lt;!-- CSS: text-align: center --&gt;
&lt;div class="center"&gt;
	&lt;span&gt;Anything in this element will be centered&lt;/span&gt;
&lt;/div&gt;
&lt;!-- CSS: text-align: justify --&gt;
&lt;p class="justify"&gt;Text is justified.&lt;/p&gt;
</pre>

<h3>Column Layouts</h3>
The column layout allows you to create a row with upi to 6 columns of the same width. This is by default responsive and scales down depending on the amount of columns per row. So 6 columns go from 6 to 3 in tablet and 1 in mobile devices, while a 2 column row simply goes from 2 to 1 on mobile devices and stays as 2 columns in tablets.
<pre>
&lt;!-- Columns --&gt;
&lt;!-- The parent element with the class "row"
removes any floating issues, aligns the 
margins correctly. Columns are created with
every direct child with a class "col2(2-6)".
col2 = 2 columns of equal width.
col3 = 3 columns of equal width.
col4 = 4 columns of equal width.
col5 = 5 columns of equal width.
col6 = 6 columns of equal width.
NOTE: Columns are meant to be of equal widths
per row. To display columns with different
widths, see Fluid Layout. --&gt;
&lt;!-- Example: Output 4 columns --&gt;
&lt;div class="row"&gt;
	&lt;div class="col4"&gt;
		&lt;span&gt;4 Columns&lt;/span&gt;
	&lt;/div&gt;
	&lt;div class="col4"&gt;
		&lt;span&gt;4 Columns&lt;/span&gt;
	&lt;/div&gt;
	&lt;div class="col4"&gt;
		&lt;span&gt;4 Columns&lt;/span&gt;
	&lt;/div&gt;
	&lt;div class="col4"&gt;
		&lt;span&gt;4 Columns&lt;/span&gt;
	&lt;/div&gt;
&lt;/div&gt;
</pre>

<h3>Fluid Layout</h3>
The fluid layout allows you to create rows with up to 12 different columns and with different widths. These columns will also behave differently in responsive mode depending on the amount of columns per row as well as the widths of the columns.
<pre>
&lt;!-- Fluid Layout --&gt;
&lt;!-- Fluid layout allows you to create columns
width different widths within the same row.
Much like columns, we start with a parent element
with the class "row". Then for the child elements
that we want to display as columns, we assign the
"span(1-12)". This makes it possible to create rows
with up to 12 columns and to create columns with 
different widths --&gt;
&lt;!-- Example: 3 columns --&gt;
&lt;div class="row"&gt;
	&lt;div class="span4"&gt;
		&lt;span&gt;span4&lt;/span&gt;
	&lt;/div&gt;
	&lt;div class="span7"&gt;
		&lt;span&gt;span7&lt;/span&gt;
	&lt;/div&gt;
	&lt;div class="span1"&gt;
		&lt;span&gt;span1&lt;/span&gt;
	&lt;/div&gt;
&lt;/div&gt;
</pre>

<h4>Tip:</h4>
By adding the class <span><pre>same-height</pre></span> to each column you can easily force the columns to have the same height based on the tallest one.