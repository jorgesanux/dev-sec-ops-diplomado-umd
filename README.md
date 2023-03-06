# 🔒 DEV-SEC-OPS diplomado UMD

<p align="center">
    <img src="./images/logo-umd.jpg" alt="logo" width="256"/>
    <img src="./images/logo-git.png" alt="logo" width="256"/>
</p>

Repositorio con comandos y usos básicos de Git, herramienta para la gestión y el versionamiento del código en diferentes sistemas operativos.

---

## Tabla de contenido

1. [Contexto](#-comandos-básicos-de-git)
2. [Crear un repositorio](#-crear-un-repositorio)
3. [Agregar token de autenticación de GitHub](#-agregar-token-de-autenticación-de-github)
4. [Subida y bajada de cambios a un repositorio remoto](#-subida-y-bajada-de-cambios-a-un-repositorio-remoto)
5. [Flujo global de trabajo de Git](#-flujo-global-de-trabajo-de-git)
6. [Autores](#autores)

## ⌨ Comandos básicos de GIT
Git es un software que se puede denominar como un sistema de control de versiones distribuido. Como lo menciona en su [pagina principal](https://git-scm.com/):

> Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

> Git is easy to learn and has a tiny footprint with lightning fast performance. It outclasses SCM tools like Subversion, CVS, Perforce, and ClearCase with features like cheap local branching, convenient staging areas, and multiple workflows.

Git es una herramienta muy poderosa que se utiliza en la mayoría de proyectos y empresas dedicadas al desarrollo del software. Su potencial y versatilidad ha permitido su rápida adopción sobre todo tipo de proyectos alrededor del mundo. Las compañías y proyectos más grandes hacen uso de Git para gestionar su flujo de desarrollo con miles de desarrolladores de forma simultánea.

![Imagen de ejemplos de comandos de git](https://res.cloudinary.com/practicaldev/image/fetch/s--AS0ya8UC--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/rixan4h4z8y94eq89som.png)
*Tomada de: [🌳🚀 CS Visualized: Useful Git Commands](https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1)*

### 🛠 Crear un repositorio
Encargado: Johan

### 🔑 Agregar token de autenticación de GitHub
Un Personal access token es una alternativa al uso de contraseñas para la autenticación en GitHub cuando se usa la API de GitHub o la línea de comandos. El Personal access token está diseñado para acceder a los recursos de GitHub en tu nombre.

### 💻 Subida y bajada de cambios a un repositorio remoto
Existen varios comandos que permiten realizar todo el proceso de subida y bajada de cambios desde y hacia un repositorio remoto. Estos comandos son:
- Add: Agrega los cambios/archivos a la sección de stage del repositorio local.\
```bash
git add [--verbose | -v] [--dry-run | -n] [--force | -f] [--interactive | -i] [--patch | -p]
        [--edit | -e] [--[no-]all | --[no-]ignore-removal | [--update | -u]]
        [--intent-to-add | -N] [--refresh] [--ignore-errors] [--ignore-missing] [--renormalize]
        [--chmod=(+|-)x] [--pathspec-from-file=<file> [--pathspec-file-nul]]
        [--] [<pathspec>...]
```
- Commit: Confirma los cambios que están en el area de stage. Crea una confirmación con un numero de hash que lo identifica en el árbol de git.
```bash
git commit  [-a | --interactive | --patch] [-s] [-v] [-u<mode>] [--amend]
            [--dry-run] [(-c | -C | --fixup | --squash) <commit>]
            [-F <file> | -m <msg>] [--reset-author] [--allow-empty]
            [--allow-empty-message] [--no-verify] [-e] [--author=<author>]
            [--date=<date>] [--cleanup=<mode>] [--[no-]status]
            [-i | -o] [--pathspec-from-file=<file> [--pathspec-file-nul]]
            [-S[<keyid>]] [--] [<pathspec>...]
```
- Push: Envía, los cambios confirmados(commits), al repositorio remoto(GitLab, GitHub, BitBucket, etc.).
```bash
git push [--all | --mirror | --tags] [--follow-tags] [--atomic] [-n | --dry-run] [--receive-pack=<git-receive-pack>]
        [--repo=<repository>] [-f | --force] [-d | --delete] [--prune] [-v | --verbose]
        [-u | --set-upstream] [-o <string> | --push-option=<string>]
        [--[no-]signed|--signed=(true|false|if-asked)]
        [--force-with-lease[=<refname>[:<expect>]] [--force-if-includes]]
        [--no-verify] [<repository> [<refspec>...]]
```
- Fetch: Descarga los cambios del repositorio remoto y los aloja en el repositorio local.
```bash
git fetch [<options>] [<repository> [<refspec>...]]
git fetch [<options>] <group>
git fetch --multiple [<options>] [(<repository> | <group>)...]
git fetch --all [<options>]
```
- Pull: Descarga los cambios del repositorio remoto y los une(merge) a la rama actual.
```bash
git pull [<options>] [<repository> [<refspec>...]]
```

### ⚒ Flujo global de trabajo de Git
\
![Estado de trabajo de Git](https://www.git-tower.com/learn/media/pages/git/ebook/en/command-line/remote-repositories/introduction/ca91d7d832-1673968486/basic-remote-workflow.png)
*Tomada de: [Learn Version Control with Git](https://www.git-tower.com/learn/git/ebook/en/command-line/remote-repositories/introduction)*

### Autores
🤵[Jorge Sanabria](https://github.com/jorgesanux)

👨‍💻[Alberto Salazar](https://github.com/albersamart)

👨‍🍳[Jhoan Torres](https://github.com/jhoant1510)
