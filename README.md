# ansible_role_desktop
This is my simple work env desktop setup for linux

```yaml
---

- hosts: localhost
  roles:
    - role: sattel.desktop
      users:
        - username: matthias
          antigen_libraries:
            - name: oh-my-zsh
          antigen_theme:
            name: robbyrussell
          antigen_bundles:
            # Bundles from the default repo (robbyrussell's oh-my-zsh).
            - name: git
            # - name: pip
            # - name: lein
            - name: command-not-found
            - name: vscode
            - name: vagrant
            # - name: mvn
            # - name: npm
            # - name: dotnet
            - name: emacs
            # Syntax highlighting bundle.
            - name: zsh-syntax-highlighting # `name` is required (any valid file name will do so long as it's unique for the bundles)
              url: zsh-users/zsh-syntax-highlighting
```
