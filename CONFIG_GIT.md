# Configurando git

Configurando los datos del usuario a nivel del S.O para git:

```bash
    git config --system user.name 'fulano'

    git config --system user.email 'fulano@email.com'
```

Configurando los datos del usuario a nivel de usuario(home/user) git:

```bash
    git config --global user.name 'fulano'

    git config --global user.email 'fulano@email.com'
```

Configurando los datos del usuario en repositorio local de git:

```bash
    git config user.name 'fulano'

    git config user.email 'fulano@email.com'
```

Listar configuraciones de git:

` git config --list [--global | --system] `
