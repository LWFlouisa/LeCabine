# LeCabine
Documenting my own implementation of mapping neurosymbolic theory.

##
~~~
                0                     1
                braun                 vert
0 le_maizon    le_maizon(braun).     le_maizon(vert).
1 le_domicile  le_domicile(braun).   le_domicile(vert).
2 le_cabine    le_cabine(braun).     le_cabine(vert).
 
                0                    1
                oublier              ne_oublier
0 le_maizon    le_maizon(oublier).  le_maizon(ne oublier).
1 le_domicile  le_domicile(oublier. le_domicile(oublier).
2 le_cabine    le_cabine(oublier).  le_cabine(oublier).
~~~

~~~
0,0; 0,0 le_maizon(braun, oublier).     or "le_maizon(braun)   :-      le_maizon(oublier)."
0,1; 0,1 le_maizon(vert, oublier).      or "le_maizon(vert)    :-   le_maizon(ne_oublier)."
1,0; 1,0 le_domicile(braun, oublier).   or "le_domicile(braun) :-    le_domicile(oublier)."
1,1; 1,1 le_domicile(vert, ne_oublier). or "le_domicile(vert)  :- le_domicile(ne_oublier)."
2,0; 2,0 le_cabine(braun, oublier).     or "le_cabine(braun)   :-      le_cabine(oublier)."
2,1; 2,1 le_cabine(vert, ne_oublier).   or "le_cabine(vert)    :-   le_cabine(ne_oublier)."
~~~
