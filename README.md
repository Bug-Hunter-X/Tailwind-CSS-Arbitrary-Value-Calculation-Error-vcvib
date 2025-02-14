# Tailwind CSS Arbitrary Value Calculation Error

This repository demonstrates a common error when using Tailwind's arbitrary value feature with calculations.  Specifically, the example shows an attempt to calculate the height of a div based on the viewport height minus a fixed value.  The issue lies in the syntax and how Tailwind interprets it. 

## Bug Description

The `h-[calc(100vh_-_50px)]` class intends to set the height to 100vh minus 50px. However, Tailwind might not correctly parse the double minus sign (`_-_`). This would result in unexpected behavior or rendering errors, possibly resulting in an incorrect height or even CSS parsing errors. 

## Solution

The solution involves correcting the calculation syntax within the arbitrary value declaration. 