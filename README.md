FIX_LINT
=========

## Permet de corriger les erreurs de syntaxe uniquement, sans altérer la sémantique du code.

A noter que le rôle devrait être exécuter plusieurs fois pour être certains que toutes les erreurs de syntaxe sont corrigées.


Role Variables
--------------

### Chemin vers les dossiers contenant les fichiers à corriger.
```yaml
fix_directories:
  - /foo/bar/install_apache/
```

### Paterne des fichiers à corriger.
```yaml
files_pattern: '*.yml'
```

### Mettre à true si la chaine de caractères renseignées dans la variable files_pattern est une regex.
```yaml
use_regex: false
```

### Nombre de caractères max pour chaque ligne
```yaml
line_max_length: 160
```


Example Playbook
----------------

```yaml
---
- hosts: localhost
  roles:
     - role: fix_lint
``` 


License
-------

GLPv3


Author Information
------------------

Dany ZAHER APP CNMOSI-S
