# fire2a-on-boarding

## git
<img src="https://imgs.xkcd.com/comics/git_2x.png"  alt='cannot load image' width="500px" >

### main usage
```bash
git clone git@github.com:fire2a/C2F-W.git
cd C2F-W

   # estos comandos sirven para generar una copia en el dispositivo local de repositorio github "git@github.com:fire2a/C2F-W.git" y se usa "cd C2F_W" pa

# alternative A
git pull
   # Permite visualizar los cambios hechos por otras personas al main original, "como actualizar el main" y aplicarlos.

# B
git fetch 
git switch [-c] branch-name-is-at-least-a-half-sentence-explaining-the-feature/issue [main]
   # fetch: sirve para descargar los cambios como branch nuevas o commit sin aplicarlos directamente.
   # switch -c: crea una nueva branch del main

git diff
git add new_or_changed_text_file
git commit -m "sentence that explains the purpose of the change"

   # git diff: visualizador de diferencias existentes entre eñ main y mi branch creada
   # git add: agregaga archivos para ser enlazados y enviados en el próximo commit, 
   # git commit -m: crea un commit nuevo y guarda los cambios hechos en el código y los archivos agregados con git   add, además sirve para dejar un mensaje que en este caso es "sentence that explains the purpose of the change"


git push [--set-upstream origin my-feature-branch]
   # sube mi branch creada con los commit para al repositorio de github sin alterar el main orignial, sólo sube las actualziaciones a mi rama para que estén disponibles en el repositorio gihub

# CASOS DE USOS COMANDOS 

   #1 MANIPULAR SCRIPT DE ANALISIS LIDAR PARA OTRA ÁREA Y OBJETIVO DE ESTUDIO
      # Existen script completos para ser utilizados para el análisis de terreno, análisis estructura de bosques con diferentes objetivos. 
      # Para poder manipular este comando sin afectar al main original hacemos una copia en nuestro dispositovo usando #git clone  ..." utilizando el enlace del código y luego nos situamos dentro de la carpeta, que para el cado de cell2fire se llama C2F.W/
      # podemos usar "git pull" para visualizar los nuevos cambios que se han hecho al main original, esto podría super la visualización de mejoras dentro de los comandos entregados por nuevos usuarios y si nos gustaría aplicar estos usamos "git fetch" para descargarlos.
      # con el repositorio descargado "clonado", y descargadas las mejoras de este con "fetch" creamos una branch nueva para trabajar independientemente del main y así no generar problemas con el código original y hacer las modificaciones que estimemos convenientes para nuetro objetivo de trabajo. 
      # "git diff" observamos las diferencias entre el main original y nuestros cambios. 
      # si estamos trabajando con diferentes archivos podemos guardar todos en un mismo commit con "git add" y dejar un mensaje con "git commit -m"
      # sube la branch con el código nuevo ya terminado, pero de manera independiente del codigo orignial. 

   #2 trabajar con diferentes archivos para un mismo proyecto. 
      # Al iniciar cada avance del proyecto se tendría que usar todos los comandos hasta "git switch" ya que luego de esto ya se establecieron las nuevas rutas o branch de trabajo, pero si en un mismo dia se trabajan con mas de un proyecto o branch a la vez todos se pueden guardar usando "git add" luego "git commit -c" dejando el mensje claro de hasta donde quedaste en el avance para todos los proyectos o branch agregadas con "git add".

   #3  trabajar en sinmultaneo en un mismo codigo con una persona en otro lugar de trabajo 
