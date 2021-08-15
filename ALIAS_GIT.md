[Regresar al inicio](./README.md)

# Creando alias de comandos para Git

Sintaxis para crear un alias:
```bash
   git config [--global | --system] alias.<nombre_alias> '<comando> [args]'
```

Configurando un alias para el status:
```bash
   git config --global alias.st 'status'
```

Usando el alias del status en git:
```bash
   git st
```

Configurando un alias del status para una salida resumida:
```bash
   ~$ git config --global alias.sts 'status -s'

   ~$ git sts
```

Configurando un alias para commit:
```bash
   ~$ git config --global alias.cm 'commit -m'

   ~$ git cm 'Mensaje para el commit.'
```

Configurando un alias para commit firmado:
```bash
   ~$ git config --global alias.cms 'commit -S -sm'

   ~$ git cms 'Mensaje para el commit.'
```

Configurando un alias para un comando del sistema:
```bash
   ~$ git config --global alias.ls '!ls -lha'

   ~$ git ls
```

Eliminar un alias de git:

```bash
    git config [--global | --system] --unset alias.<nombre_alias>
```

Listar configuraciones (Incluye los alias) de git:

```bash
    git config --list [--global | --system]
```