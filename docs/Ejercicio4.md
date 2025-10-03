Git.

Colaborando

pull request (PR)

JESÚS ÁLVAREZ OLMO

2ASIX

Pulsando en el **botón fork** en el GitHub de Espe creo una copia en mi
cuenta.

![](Pictures/10000000000003AD00000390535F6ADD.png){width="17cm"
height="11.663cm"}

![](Pictures/10000000000003B200000232F84E79B9.png){width="17cm"
height="10.098cm"}

Ahora clono el fork a mi ordenador:

git clone https://github.com/JesusKernel/exercici4.git

cd exercici4

![](Pictures/1000000000000373000000D1878BBA9D.png){width="17cm"
height="4.717cm"}

Creo una rama nueva y entro en ella:

git checkout -b jesus_cambios

![](Pictures/1000000000000372000000515B292F9E.png){width="17cm"
height="2.708cm"}

sudo nano README.md

Añado: - \[Jesus Alvarez Olmo\](files/jao.md)

![](Pictures/100000000000031800000129B3BCA9DA.png){width="17cm"
height="8.855cm"}

Contesto la pregunta Quin mòdul m'agrada més?

Modificando **files/jao.md** en visual studio code:

![](Pictures/10000000000003F1000001656D90215C.png){width="17cm"
height="12.215cm"}

Añado y confirmo los cambios:

git add README.md files/jao.md

git commit -m \"Afegir enllaç amb les meues inicials i resposta en
jao.md\"

![](Pictures/10000000000003B0000000C850818A45.png){width="17cm"
height="7.177cm"}

Ahora hago un push para subir la rama jesus_cambios:

git push origin jesus_cambios

![](Pictures/1000000000000546000000AAD871F0A2.png){width="17cm"
height="4.999cm"}

Pero da un error.

Para solucionar el error he buscado información y cambio el remoto
origin para que apunte a mi fork. Eso significa que ya puedo subir mi
rama jesus_cambios a mi fork, y luego crear el Pull Request hacia el
repositorio de Espe.

Subo mi rama al fork:

git push -u origin jesus_cambios

![](Pictures/1000000000000399000001A2B3C5B1B3.png){width="17cm"
height="11.264cm"}

Creo Pull Request en mi GitHub:

Abro mi fork: https://github.com/JesusKernel/exercici4

Voy al botón Compare & pull request para la rama jesus_cambios.

![](Pictures/1000000000000253000000EB72B2FBB8.png){width="15.739cm"
height="6.216cm"}

Hago clic en Create pull request.

Y añado un título descriptivo, por ejemplo:

Afegir enllaç al README i fitxer jao.md amb la meua resposta

Añado una descripción breve explicando tus cambios y pulso Create pull
request.

![](Pictures/1000000000000552000003004DC1FD58.png){width="17cm"
height="11.912cm"}

![](Pictures/1000000000000780000002BC5047AB02.png){width="17.872cm"
height="11.793cm"}

Esto crea la petición de que el profesor revise e integre tus cambios.

Ahora tengo que esperar a que Espe acepte la petición mia.

Cuando la profesora acepte el PR, los cambios se integrarán en el
repositorio original (espemm/exercici4).

![](Pictures/100000000000077D000001F63EDCA326.png){width="17.739cm"
height="8.468cm"}
