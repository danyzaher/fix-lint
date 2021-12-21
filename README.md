FIX_LINT
=========

## Permet de corriger les erreurs de syntaxe sans altérer le code.

Role Variables
--------------

### Chemin vers les dossiers contenant les fichiers à corriger
```yaml
fix_directories:
  - /foo/bar/cis-tomcat/
```

### Paterne des fichiers à corriger
```yaml
files_pattern: '*.yml'
```

### Mettre à true si la chaine de caractères renseignées dans la variable files_pattern est une regex
```yaml
use_regex: false
```

Example Playbook
----------------

```yaml
    - hosts: localhost
      roles:
         - role: fix_lint
``` 

License
-------

GLPv3

Author Information
------------------

Dany ZAHER APP
