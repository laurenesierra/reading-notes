## HTML Lists

- Unordered
- Ordered
- Definition
```
<dl>
  <dt>Parmasan</dt>
  <dd>An Italian cheese</dd>
</dl>
  
  ```
  - Nested lists(a list within a list)

  Remember that evrything is a box...
  You can adjust the height and width of a box/ container (eg. paragraph/divider). Use _pixels_, _percentages_ or _ems_.

  Use _min-width_, _max-width_, _mid-height_ and _max-height_ to control legibility when people view your page on different size browsers.

  Every box has:
  1. Border (border-width/border-style/border-color)
  1. Margin
  1. Padding

_White Space_:
The space between items on your page.

_Border Images_:

1. The URL
1. Where to slice the image
1. What to do with straight edges (stretch, repeat and round)
 
 _Box-shadow_(It must use at least 2 values):
 - Horizontal
 - Vertical
 - Blur Distance
 - Spread of Shadow

 _Border Radius_:
 - This gives you the ability to round corners.

 ## Decisions and Loops


 #### __Comparison Operators__

 Use these to compare one value in the script to what you expect it might be. The result is a _Boolean_ = TRUE or FALSE.

```
== (is equal to)
Ex. 'Hello' == 'Goodbye' FALSE

!= (is not equal to) 
Ex. 'Hello' != 'Goodbye' TRUE

=== (strict eqaul to)
'3' === 3 FALSE
'3' === '3' TRUE

!== (strict not equal to)
'3' !== 3 TRUE
'3' !== '3' FALSE

> (greater than)
4 > 3 TRUE
3 > 4 FALSE

< (less than)
3 < 4 TRUE
4 < 3 FALSE

>= (greater than or equal to)
4 >= 3 TRUE
3 >= 4 FALSE
4 >= 4 TRUE

<= (less than or to eqaul to)
4 <= 3 FALSE
3 <= 4 TRUE
3 <= 3 TRUE

```

_Operands_:
These are placed on either side of the operator. They can be values or variables.

#### __Logical Operators__
These allow you to compare the results of more then one comparision operator.

```
&& (Logical And)
This tests more then one condition

|| (Logical Or)
This tests at least one condition

! (Logical Not)
This takes a single Boolean value and inverts it

```

[<----- Back to About Me](README.md)