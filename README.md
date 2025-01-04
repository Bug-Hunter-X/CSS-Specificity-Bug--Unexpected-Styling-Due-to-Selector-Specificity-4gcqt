# CSS Specificity Bug

This repository demonstrates a common CSS bug related to selector specificity.  The issue arises when selectors with different specificity levels conflict, and the more specific selector overrides the less specific one.  This example showcases how unexpected styling results from not properly managing selector specificity in your CSS.

## Problem

The CSS file (`bug.css`) contains selectors that conflict due to specificity.  The intention was for all `.item` elements to be blue, but due to the more specific selector `.container .item`, items within a container are unexpectedly styled red.

## Solution

The solution (`bugSolution.css`) addresses the specificity conflict.  The order of CSS rules matters, but you need to make sure your most specific selector appears last in your code, as well as making sure you're using proper specificity rules when possible.