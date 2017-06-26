# Ansible role for dehydrated


Setup [dehydrated](https://github.com/lukas2511/dehydrated).

## Requirements

- Debian
- Ubuntu

## Role Variables

see defaults/main.yml

## Dependencies

None.

## Example Playbook

Example:

    - hosts: servers
      become: yes
      roles:
         - role: znz.dehydrated
           dehydrated_domains: |
             example.net

Another example:

    - hosts: all
      become: yes
      roles:
      - role: znz.dehydrated
        dehydrated_domains: |
          example.org www.example.org
          example.com www.example.com wiki.example.com
        dehydrated_contact_email: "root@example.net"

## License

MIT License
