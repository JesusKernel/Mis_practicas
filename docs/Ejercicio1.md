1

Git

GitHub

JESÚS ÁLVAREZ OLMO

2ASIX

!!! success "Objectius" Recordar l'ús de git per a realitzar el control
de versions dels projectes. Configu- rar un compte a GitHub, servei que
ens ofereix repositoris remots. Recordar el cicle de vida de la gestió
dels nostres repositoris: creació, clonatge, sincronització, ... i els
nostres fitxers: creació, modificació, esborrat.

> Qué has de fer?

Crea un compte a GitHub (Si no el tens!!!). La forma d'accedir als
repositoris remots de GitHub serà per SSH, per tant has de copiar la
teua clau pública RSA a GitHub, per això:

> Crea a GitHub un repositori amb el nom prova_el_teu_nom (inicialitza
> el repositori amb un fitxer README) i la descripció Repositorio de
> prueba 2ASIX.

![](Pictures/10000001000004C80000052DE2DAC901.png){width="12.965cm"
height="15.901cm"}

1.  Instal·la git en el teu ordinador (si no el tens instalado!!!).

> apt-get install git

![](Pictures/100000010000025D0000003F1FA89168.png){width="15.901cm"
height="1.64cm"}

Configuració de git. El primer que hauries defer quan instal·les Git és
establir elteu nom d'usuari i adreça de correu electrònic (Assegura't
que les dades són correctes i que has posat el teu nom complet). Això és
important perquè les confirmacions de canvis (commits) a Git utilitzen
aquesta informació, i és introduïda de manera immutable en els commits
que envieu:

git config \--global user.name \"John Doe\"

git config \--global user.email
[**johndoe@example.com**](mailto:johndoe@example.com)

![](Pictures/10000001000003B30000003FE836ABCE.png){width="15.901cm"
height="1.058cm"}

![](Pictures/100000010000047A0000003FA68C6A04.png){width="15.901cm"
height="0.873cm"}

De nou, només cal fer-ho una vegada si especifiques l'opció --global, ja
que Git sempre utilitzarà aquesta informació per a tot el que facis en
aquest sistema.

Clonar el repositori remot. Copia la url SSH del repositori (no copiïs
la URL https) i clonarem el repositori al nostre ordinador.

![](Pictures/1000000100000484000000D228116181.png){width="15.901cm"
height="6.75cm"}

Crearem un nou fitxer, l'afegirem al nostre repositori local i després
ho sincronitzarem amb el nostre repositori remot de GitHub. Cada vegada
que fem una modificació en un fitxer ho podem assenyalar creant un
commit. Els missatges dels commits són fonamentals per explicar
l'evolució d'un projecte. Un commit ha de ser un petit conjunt de canvis
dels fitxers del projecte amb una certa coherència.

echo \"Açò és una prova\"

git add exemple.txt

![](Pictures/100000010000042900000037A9A18AC4.png){width="15.901cm"
height="0.82cm"}

![](Pictures/10000001000004470000006CAFFB881E.png){width="15.901cm"
height="1.561cm"}

git commit -m \"He creat el fitxer exemple.txt\"

![](Pictures/10000001000004B3000001AC7DA695E6.png){width="15.901cm"
height="5.662cm"}

git push

![](Pictures/10000001000003F40000017A86DE8334.png){width="15.901cm"
height="7.916cm"}

**Resultado del «push» en el repositorio de la nube.**

![](Pictures/1000000100000984000001E9A41C468D.png){width="15.901cm"
height="7.736cm"}

Si modifiqueu un fitxer al vostre repositori local, no l'heu de tornar a
afegir al vostre repositori (git add). Però has de fer servir l'opció -a
en fer el commit.

![](Pictures/1000000100000560000000A2E7FD1B22.png){width="15.901cm"
height="1.879cm"}

**git commit -am \"He modificado el fichero ejemplo.txt\"**

![](Pictures/100000010000056000000081E82D66B9.png){width="15.901cm"
height="1.482cm"}

**git push**

![](Pictures/10000001000003F700000197C17DDEEE.png){width="15.901cm"
height="8.183cm"}

Si vols canviar el nom d'un fitxer o directori del teu repositori:

**git mv ejemplo.txt ejemplo2.txt**

![](Pictures/10000001000003F70000004CC2B5BEBF.png){width="15.901cm"
height="1.191cm"}

**git commit -am \"He cambiado el nombre del fichero\"**

![](Pictures/10000001000005870000008DBCBD3CA2.png){width="15.901cm"
height="1.588cm"}

**git push**

![](Pictures/10000001000005A20000021BAEEDA6EC.png){width="15.901cm"
height="5.953cm"}

Resultado del «push» en el repositorio de la nube.

![](Pictures/10000001000005A20000021B4EBEF0BC.png){width="15.901cm"
height="10.622cm"}

Si vols esborrar un fitxer del teu repositori:

**git rm exemple2.txt**

![](Pictures/1000000100000311000000BBDA5C7319.png){width="15.901cm"
height="3.784cm"}

**git commit -am \"He esborrat el fitxer exemple2\"**

![](Pictures/10000001000004B1000000BB29E7A107.png){width="15.901cm"
height="3.9cm"}

**git push**

![](Pictures/10000001000003E50000019893D765CB.png){width="15.901cm"
height="8.237cm"}

Pots clonar el teu repositori de GitHub a diversos ordinadors (per
exemple, si vols treballar a casa teva i a l'institut), per tant abans
de treballar en un repositori local has de sincronitzar els possibles
canvis que s'hagin produït al repositori remot, per això:

**git pull**

Per comprovar l'estat del meu repositori local:

**git status**

![](Pictures/1000000100000352000001180A5BAF19.png){width="15.901cm"
height="5.239cm"}

**Busca informació per a crear un nou repositori anomenat prueba2_jesus.
**

En aquesta ocasió, crea primer el repositori local (usant git init) i
després cerca informació per sincronitzar-lo i crear el repositori remot
a GitHub.

**Primero crear un reposito local prueba2_jesus con mkdir y entramos
dentro:**

![](Pictures/10000001000004B4000000DF6141C5FE.png){width="15.901cm"
height="2.937cm"}

«git init» para iniciar git

![](Pictures/10000001000005CD0000019A9C1CCFE0.png){width="15.901cm"
height="4.392cm"}

Creo un README.md y añado un contenido al README.md

![](Pictures/100000010000046900000028BB448EC4.png){width="15.901cm"
height="1.09cm"}

![](Pictures/1000000100000469000000280D51D6F8.png){width="15.901cm"
height="1.27cm"}

**Y hago el primer commit:**

git add .

**git commit -m "Hago el primer commit"**

![](Pictures/100000010000042C000000D84C57A61C.png){width="15.901cm"
height="3.228cm"}

La primera línea asegura que la rama local se llama main (que es lo que
GitHub usa por defecto).

git branch -M main

![](Pictures/10000001000003160000002E8916D456.png){width="15.901cm"
height="0.926cm"}

La segunda línea sube tu commit a GitHub y deja el enlace establecido.

git push -u origin main

![](Pictures/10000001000004420000017FDBEDC384.png){width="15.901cm"
height="5.583cm"}

Resultado en la nube:

![](Pictures/10000001000001CE0000015B9FDC6A1C.png){width="15.894cm"
height="7.096cm"}
