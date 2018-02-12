# \<spine-contrastor-mixin\>
Mixin which determines to which dark or light theme an element belongs based on its
background color. Provides `darkTheme` and `lightTheme` boolean properties to the element.

Theme detection is based on a background color contrast to black and white colors
respectively. If the contrast to black is higher than the contrast to white - light
theme is used, otherwise - dark theme.
For the algorithm details see:
- https://www.w3.org/TR/WCAG20/#contrast-ratiodef
- https://www.w3.org/TR/WCAG20/#relativeluminancedef
- https://en.wikipedia.org/wiki/Luma_(video)#Rec._601_luma_versus_Rec._709_luma_coefficients
