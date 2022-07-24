# Archlinux AUR

Installs AUR Packages.

## Requirements

It should work on any archlinux distribution

## Role Variables

| Variable                  | Required | Default | Choices         | Comments                                    |
| ------------------------- | -------- | ------- | --------------- | ------------------------------------------- |
| archlinux_aur\_\_packages | yes      |         |                 | list of packages to be installed or removed |
| archlinux_aur\_\_state    | no       | present | present, absent | present to install, absent to remove        |

## Dependencies

- eliseuvideira.archlinux_aur_setup

## Example Playbook

    - hosts: archlinux
      roles:
        - role: username.archlinux_aur
          archlinux_aur__packages:
            - nvm
            - visual-studio-code-bin
          archlinux_aur__state: present

## License

MIT
