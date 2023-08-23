---
title: "Curve Fitting"
---
# Curve Fitting
---
## Linear Regression

Let the "Residual" be the distance between the line and the point. Then we want to make r as small as possible.
![[Pasted image 20220914225120.png|300]]

Using the least-squares fit: (n points)
![[Pasted image 20220914225958.png]]
Then line: $y=a_0 + a_1x$

Functionality is built into backslash:
![[Pasted image 20220914231134.png]]
![[Pasted image 20220914231055.png]]

------

## Polyfit
$[a_1, a_0]$ = polyfit(x, y, degree#)
where $y=a_0+a_1x$

