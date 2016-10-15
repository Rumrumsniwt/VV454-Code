a = Plot[1/
    6 ((3 - 3 I) E^(-I t) + (3 + 3 I) E^(I t) - 
      I Sqrt[3] E^(-I Sqrt[3] t) + I Sqrt[3] E^(I Sqrt[3] t)), {t, 0, 
    60}, AspectRatio -> 1/5, PlotRange -> {{0, 60}, {-5, 5}}, 
   AxesStyle -> Thick, 
   Epilog -> {Text[Style[Velocity, Bold, Black, 15], {2, 4}], 
     Text[Style[Time, Bold, Black, 15], {30, 2}]}, 
   PlotStyle -> {RGBColor[0, 1, 0]}, 
   TicksStyle -> Directive["Label", 14, Black]];
b = Plot[-((I E^(-I Sqrt[3] t) (-1 + E^(2 I Sqrt[3] t)))/Sqrt[3]), {t,
     0, 60}, AspectRatio -> 1/5, PlotRange -> {{0, 60}, {0, 16}}, 
   AxesStyle -> Thick, 
   Epilog -> {Text[Style[Displacement, Bold, Black, 15], {3, 12.5}], 
     Text[Style[Time, Bold, Black, 15], {30, 1}]}, 
   PlotStyle -> {RGBColor[0, 0, 1]}, 
   TicksStyle -> Directive["Label", 14, Black]];
c = Plot[1/
    6 ((-3 + 3 I) E^(-I t) - (3 + 3 I) E^(I t) - 
      I Sqrt[3] E^(-I Sqrt[3] t) + I Sqrt[3] E^(I Sqrt[3] t)), {t, 0, 
    60}, AspectRatio -> 1/5, PlotRange -> {{0, 60}, {0, 16}}, 
   AxesStyle -> Thick, 
   Epilog -> {Text[Style[Displacement, Bold, Black, 15], {3, 12.5}], 
     Text[Style[Time, Bold, Black, 15], {30, 1}]}, 
   PlotStyle -> {RGBColor[1, 0, 0]}, 
   TicksStyle -> Directive["Label", 14, Black]];
Show[a, b, c]