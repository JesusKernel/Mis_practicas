Git.

Trabajando

con

ramas y uniones

JESÚS ÁLVAREZ OLMO

2ASIX

1\. Crea una branca que s'anomene primera al teu repositori local, i
executa la instrucció necessària

per comprovar que s'ha creat.

a- Hago pongo el comando para ver en que rama estoy:

git branch

![](Pictures/1000000000000215000000553311BF25.png){width="15.66cm"
height="2.247cm"}

b- Creo la primera rama:

git branch 1_rama

![](Pictures/100000000000024E00000089FEBBB670.png){width="15.609cm"
height="5.106cm"}

c- Salgo de la rama main y voy a la creada:

git checkout 1_rama

![](Pictures/10000000000002610000009B98A004A9.png){width="15.769cm"
height="5.71cm"}

2\. Crea un nou fitxer en aquesta branca i fusiona'l amb la principal.
S'ha produït un conflicte? Raona la resposta.

![](Pictures/10000000000003FB000000BAF162CDFA.png){width="17cm"
height="5.221cm"}

![](Pictures/10000000000002BD0000009066EE47A0.png){width="17cm"
height="4.872cm"}

Ahora fusiono 1_rama en main:

git merge 1_rama

![](Pictures/100000000000027B000000B6F903AEEA.png){width="16.798cm"
height="6.824cm"}

*RESPUESTA*: Como el archivo_1_rama.txt solo existe en 1_rama no hay
conflicto.

3\. Esborra la branca primera.

git branch -d 1_rama

![](Pictures/100000000000028A0000005026FE7682.png){width="17cm"
height="2.092cm"}

4\. Crea una branca que s'anomene segona, i modifica un fitxer per
produir un conflicte en unir-lo a la branca principal. Lliura el
contingut del fitxer on s'ha produït el conflicte.

git checkout -b segunda

git branch -v (para verificar el cambio de rama)

![](Pictures/10000000000002F70000009D82164FD2.png){width="17cm"
height="5.253cm"}

echo \"Línea añadida desde la rama segunda\" \>\> README.md

git add README.md

git commit -m \"Modificar README.md desde rama segunda\"

![](Pictures/100000000000040D0000009295160BBA.png){width="17cm"
height="5.165cm"}

Volvemos a rama main y modificamos el mismo archivo:

git checkout main

echo \"Línea añadida desde la rama main\" \>\> README.md

git add README.md

git commit -m \"Modificar README.md desde rama main\"

Y fusionamos la rama segunda en main:

git merge segunda

![](Pictures/10000000000004270000016C418937A1.png){width="17cm"
height="5.821cm"}

5\. Soluciona el conflicte que has creat al punt anterior i sincronitza
la branca segona al remot.

cat README.md

![](Pictures/10000000000001C8000000B4D90AAE5C.png){width="12.063cm"
height="4.761cm"}

![](Pictures/10000000000001E10000007EC7B42F60.png){width="12.725cm"
height="3.334cm"}Hago cambios con **nano README.md**

git add README.md

git status

![](Pictures/10000000000002FD000001442A516CCC.png){width="17cm"
height="7.198cm"}

git commit -m \"Resolver conflicto en README.md al fusionar segunda en
main\"

![](Pictures/1000000000000438000000A31A189CA7.png){width="17cm"
height="3.859cm"}

git push origin main

![](Pictures/1000000000000378000001308E572573.png){width="17cm"
height="5.819cm"}

Ahora subo todos los cambios al GitHub:

git status

git push origin main

git push origin segunda

![](Pictures/100000000000039A000001D80187CF61.png){width="17cm"
height="8.703cm"}

![](Pictures/1000000000000491000001BF5B2D350E.png){width="17cm"
height="6.537cm"}

URL al GitHub: https://github.com/JesusKernel/prueba_markdown.git
