### Clonar el repositorio
```bash
git clone git@github.com:fire2a/C2F-W.git
```
Clona el repositorio remoto de forma local.

### Cambiar al directorio del repositorio clonado
```bash
cd C2F-W
```
Accede al directorio donde está el repositorio clonado.

### Opción A: Actualizar el repositorio local con `git pull`
```bash
git pull
```
Descarga y fusiona los cambios más recientes del repositorio remoto con la rama local.

### Opción B: Actualizar el repositorio local con `git fetch` y cambiar de rama
```bash
git fetch
git switch [-c] my-feature-branch [main]
```
- `git fetch`: Descarga los cambios recientes del repositorio remoto, sin fusionarlos automáticamente.
- `git switch`: Cambia a una rama existente o crea una nueva rama (`-c`) basada en otra (en este caso `main`).

### Añadir y registrar cambios
```bash
git add new_or_changed_text_file
git commit -m "sentence that explains the purpose of the changes"
```
- `git add`: Prepara los archivos modificados o nuevos para el commit.
- `git commit`: Guarda los cambios con un mensaje.

### Subir cambios al repositorio remoto
```bash
git push [--set-upstream origin my-feature-branch]
```
Sube los cambios realizados en la rama al repositorio remoto.

### Crear un pull request
```bash
firefox https://github.com/fire2a/C2F-W/compare/main...my-feature-branch
```
Abre la página de GitHub mediante firefox para comparar la rama con `main` y hacer un pull request.

## Diferencia entre las opciónes A y B

- **Opción A (`git pull`)**: Esto combina `fetch` y `merge` automáticamente. Es más rápida, pero te da menos control.
- **Opción B (`git fetch` + `git switch`)**: Permite inspeccionar los cambios antes de fusionarlos, lo que es más seguro.
- **Opción B pull request**: Abre GitHub desde el terminal, ahorrándose el tener que ir a la página para hacer la solicitud.