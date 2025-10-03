Mkdocs

Github Pages

JESÚS ÁLVAREZ OLMO

2ASIX

Primero instalo en el terminal de linux las dependencias necesarias:

sudo apt update

sudo apt install python3 python3-pip git -y

pip install mkdocs mkdocs-material

sudo apt install mkdocs

Así se instala MkDocs y el tema ****Material****.

Ahora voy a crear un proyecto con MkDocs

mkdocs new Proyecto_MkDocs_GitHub_Pages

![](Pictures/100000000000038F00000077501D48EF.png){width="17cm"
height="3.533cm"}

cd Proyecto_MkDocs_GitHub_Pages

![](Pictures/100000000000038E0000006890C91D3D.png){width="17cm"
height="2.291cm"}

Esto crea:

mkdocs.yml → archivo de configuración

docs/index.md → página inicial

En el siguiente paso edito docs/index.md con editor nano docs/index.md):

![](Pictures/100000000000038200000078AF5026DB.png){width="17cm"
height="5.696cm"}

Modifico el archivo **/Proyecto_MkDocs_GitHub_Pages/index.md**

![](Pictures/100000000000039D0000020ED1CF9805.png){width="17cm"
height="11.4cm"}

Ahora genero la WEB estática:

mkdocs build

![](Pictures/100000000000037500000091BCD9F7FC.png){width="17cm"
height="6.634cm"}

Cuando ejecuto mkdocs build:

MkDocs buscará el archivo mkdocs.yml (que está en la raíz del proyecto).

Tomará los archivos Markdown que tengo en la carpeta docs/.

Y creará una carpeta nueva llamada site/ con el HTML generado.

Pruebo en un servidor local

mkdocs serve

![](Pictures/10000000000007800000040CA2D858E5.png){width="17cm"
height="13.002cm"}

En el navegador:

![](Pictures/10000000000004B60000028A4030E426.png){width="17cm"
height="9.162cm"}

Creo un nuevo repositorio con el mismo nombre que el proyecto:

![](Pictures/10000000000003A20000034836BD5C46.png){width="19.507cm"
height="23.915cm"}

El el terminal dentro de la carpeta repositorio
/Proyecto_MkDocs_GitHub_Pages:

echo \"# Proyecto_MkDocs_GitHub_Pages\" \>\> README.md

git init

git add README.md

git commit -m \"first commit\"

git branch -M main

![](Pictures/10000000000003BF0000025B9220424A.png){width="17cm"
height="8.999cm"}**git remote add origin**
**https://github.com/JesusKernel/Proyecto_MkDocs_GitHub_Pages.git**

![](Pictures/100000000000040E00000148223EAC87.png){width="17cm"
height="9.303cm"}

git push -u origin main

![](Pictures/10000000000003B3000000D4358B9FDF.png){width="17cm"
height="5.805cm"}

Publicar en GitHub Pages:

Cuando mi repositorio ya esté en GitHub, ejecuto:

mkdocs gh-deploy

![](Pictures/1000000000000403000001D2080B8DD3.png){width="17cm"
height="10.114cm"}

Se construye el sitio (site/)

Y lo sube automáticamente a una nueva rama gh-pages en mi repositorio.

URL : https://github.com/JesusKernel/Proyecto_MkDocs_GitHub_Pages
