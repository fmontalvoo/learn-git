[Regresar al inicio](./README.md)

# Creando ramas en Git

<!-- ![imagen](./img/git_branch.png) -->

<p align="center">
    <img src="img/git_branch.png">
</p>

Para crear una nueva rama en git basta con ejecutar el siguiente comnado:

```bash
    git branch <nombre_rama>
```

Para cambiar de rama se debe ejecutar:

```bash
    git checkout <nombre_rama>
```

Para crear una nueva rama e inmediatamente cambiar a esta, se debe ejecutar:

```bash
    git checkout -b <nombre_rama>
```

Para fusionar los cambios de la nueva rama en la rama principal debe realizar los siguientes pasos:

1. Debe cambiarse a la rama principal o la rama en la que deseé integrar los cambios

```bash
    git checkout <rama_destino>
```

2. Luego debe escoger la rama con la cuál funcionará los cambios

```bash
    git merge <rama_integracion> 
```

3. Finalmente debera eliminar la rama que acaba de integrar a su rama principal

```bash
    git branch -d <rama_integracion>
```

## Crear rama a partir de un commit especifico

Para crear unar rama a partir de un commit en especifico sede hacer uso del checksum que genera git cuando se realiza un commit.

```bash
     git log --oneline

    8f92a05 (HEAD -> master, origin/master, origin/HEAD) Se agrega la documentacion para configurar alias en Git.
    9326f6a Se agrega el archivo README.me
    1544dae Configuracion inicial de git.
    6fbd94d Initial commit
```

Por ejemplo, podemos escoger el primer commit para conecer cuál fue el estado inicial del repositorio cuando este fue creado. Para lo cual debemos escoger el primer checksum **6fbd94d** y ejecutar el siguiente comando ` git branch inicio 6fbd94d`. La sintaxis del comando es la siguiente:

```bash
    git branch <nombre_rama> <checksum>
```

Este comando tambien se puede utilizar con la opcion `checkout -b`
