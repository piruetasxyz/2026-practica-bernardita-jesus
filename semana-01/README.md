# Semana-01

## Resumen de días, temas y horas

| Fecha      | Día      | Temas                                                | Lugar     | Horas día / hora semana |
| :--------- | :------- | :--------------------------------------------------- | :-------- | :---------------------- |
| 2026-07-20 | Lunes    | git, github cli, planificación, referentes           | Rep180    | 004 / 004               |
| 2026-07-21 | Martes   | git, markdown, visual studio code, C++               | Casa      | 007 / 011               |
| 2026-07-22 | Miercoles | git, referentes                                     | Casa      | 002 / 013               |

### Copia del repositorio

Hice una copia del repositorio de la práctica en mi computador desde la terminal. Estoy utilizando **Windows PowerShell** y **Visual Studio Code** para subir varios archivos a la nube de **GitHub**.

Voy a hacer una distinción; hay dos versiones de este repositorio. Una es el **repositorio remoto**, que está alojado en GitHub, y la otra es la **copia local** que se encuentra en mi computador.

Por el momento, lo que tengo que hacer es abrir la terminal y encontrar mi repositorio.

Con **cd** busco este espacio y puedo simplemente escribir github, luego 2026 y presionar la tecla **Tab** para que autocomplete la búsqueda, ya que realmente no tengo ningún otro repositorio copiado. Por eso, me redirige automáticamente a la única opción disponible.

```bash

PS C:\Users\berni> cd .\github\2026-practica-bernardita-jesus\
PS C:\Users\berni\github\2026-practica-bernardita-jesus>
```

Luego consulto el estado de mi repositorio con el comando **git status** para conocer los cambios que se han realizado.

```bash
PS C:\Users\berni\github\2026-practica-bernardita-jesus> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   semana-01/README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\berni\github\2026-practica-bernardita-jesus>
```

Para asegurarnos de que no haya ningún conflicto, deberíamos partir con el comando **git pull** para traer los cambios subidos al repositorio remoto y actualizar el repositorio local.

```bash
PS C:\Users\berni\github\2026-practica-bernardita-jesus> git pull
Already up to date.
```

En caso de un posible conflicto, en donde las líneas vayan a chocar, podemos utilizar el comando **git pull --rebase origin main** para traer los cambios del repositorio remoto y reaplicar nuestros cambios sobre ellos.

```bash
PS C:\Users\berni\github\2026-practica-bernardita-jesus> git pull --rebase origin main
remote: Enumerating objects: 2, done.
remote: Counting objects: 100% (2/2), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (2/2), 1.73 KiB | 253.00 KiB/s, done.
From https://github.com/Bernardita-Jesus/2026-practica-bernardita-jesus
 * branch            main       -> FETCH_HEAD
   31edce7..bbbbada  main       -> origin/main
Successfully rebased and updated refs/heads/main.
```

En este caso, modifiqué el archivo README de la carpeta semana-01, que, por cierto, corresponde a estos mismos apuntes.

Con el comando **git add .** se preparan todos los cambios realizados para el próximo commit. También es posible agregar únicamente un archivo o una carpeta específica, indicando su ruta en lugar del punto (.).

```bash
PS C:\Users\berni\github\2026-practica-bernardita-jesus> git add .
PS C:\Users\berni\github\2026-practica-bernardita-jesus>
```

Con el comando **git commit -m** se crea un commit con un mensaje que nombra los cambios realizados. Es necesario haber agregado previamente los archivos con git add, ya que solo los cambios preparados serán incluidos en el commit.

```bash
PS C:\Users\berni\github\2026-practica-bernardita-jesus> git commit -m "ejemplo de cambio"
[main 8c1098b] ejemplo de cambio
 1 file changed, 36 insertions(+), 2 deletions(-)
PS C:\Users\berni\github\2026-practica-bernardita-jesus>
```

Por último, para enviar los cambios al repositorio en GitHub, utilizamos el comando **git push**. Para que este comando funcione, es necesario haber agregado previamente los archivos con **git add** y haber creado un commit con **git commit -m**. De esta manera los cambios se sincronizan con el repositorio en GitHub.

```bash
PS C:\Users\berni\github\2026-practica-bernardita-jesus> git push
fatal: unable to access 'https://github.com/Bernardita-Jesus/2026-practica-bernardita-jesus.git/': Could not resolve host: github.com
PS C:\Users\berni\github\2026-practica-bernardita-jesus>
```

En este caso, y qué interesante haberlo podido probar, me dice que hubo un error fatal, ya que por las lluvias se me cortó la luz y no tengo internet, por lo que esta función es de las pocas que sí requieren conexión a Internet.

**git stash**: con esto se guardan temporalmente los cambios sin hacer un commit, dejando el repositorio como estaba en el último commit.

**git push y git pull** son los comandos que requieren conexión a Internet, ya que son los que se conectan con el repositorio en GitHub.

#### Comandos

Punto (.) podriamos definirlo como aquí mismo, dos puntos (..)

```bash
code .
open .
mkdir
gr
history
pwd
cd
```

### Investigación de referentes sonoros

#### Alvin Lucier

I Am Sitting in a Room (45 min)

Alvin Lucier interpreta esta canción, la cual es más un experimento de frecuencias de resonancia. Él graba un audio en el cual narra un poco su propuesta; es un audio de aproximadamente un minuto que se reproduce en una habitación, en la cual se graba y vuelve a reproducir, y esto se va repitiendo. De a poco se van perdiendo las palabras y se transforman en un sonido casi ambiental, en donde el espacio se vuelve una variable importante para el resultado.

Solo puedo pensar ¿cuántos sonidos están encriptados entre la reverberación?

Realmente es interesante cuando repites algo, y lo repites, lo exageras y lo distorsionas hasta que se convierte en eso, un encriptado de algo, de algo a lo que no puedes retroceder.

También pienso que se convirtió en algo armónico. Esa fue una de mis primeras impresiones, pero más que armónico, se homogeneizó.

¿Qué es la resonancia?

La imaginé como la distorsión del sonido, el sonido rebotando, pero por supuesto, eso se queda corto, porque muchas cosas pueden ser distorsión.

Realmente la resonancia es un fenómeno acústico. Cuando un elemento es afectado por una frecuencia, este comienza a vibrar, lo cual genera un efecto de amplificación.

https://www.tabakalera.eus/es/alvin-lucier/

https://www.moma.org/explore/inside_out/2015/01/20/collecting-alvin-luciers-i-am-sitting-in-a-room/

https://umma.umich.edu/exhibitions/alvin-lucier-i-am-sitting-in-a-room/

https://iberacustica.cl/blog/resonancia-acustica-como-el-sonido-puede-hacer-vibrar-y-romper-objetos/

#### Steve Reich

Álbum drumming (4 canciones - 56 min)

Steve Reich, uno de los principales referentes de la música minimalista, compone esta obra de percusión dividida en cuatro partes. Cada una incorpora un instrumento distinto que va variando a lo largo de la pieza, acompañado por voces que imitan estos sonidos instrumentales. La obra está inspirada en la cultura africana; cada parte explora diferentes instrumentos y la cuarta reúne todos ellos. Se construye a partir de un patrón rítmico básico que se repite constantemente, mientras las escalas y las armonías van cambiando de forma progresiva.

Al igual que el minimalismo en otras disciplinas, su música busca reducir los elementos a lo mínimo. Steve Reich explora esta reducción mediante variaciones que transforman gradualmente la percepción de la estructura.

Me gustó que en obras como Phase Patterns cuestione el uso tradicional de los instrumentos. Me parece interesante esta idea de deconstruir la función para la que fueron creados y explorar nuevas posibilidades sonoras a partir de ellos.

https://stevereich.com/

https://www.drummingat50.com/

https://www.allclassical.org/the-story-of-minimalism-part-one-a-new-way-of-listening/

#### Referentes de diseño paramétrico

- Tommy.sh
- Oskitone
- benjiaomodular

## Pendientes

Robert Ashley, Robert Wilson, David Behrman y Gordon Mumma. (por mi)

Investigar Parla y Relo.

