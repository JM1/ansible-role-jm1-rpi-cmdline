# Ansible Role `jm1.rpi_cmdline`

This role helps to setup the kernel cmdline on Raspberry Pi.

**Tested OS images**
- [`Ubuntu 20.04 LTS` (`arm64`) for Raspberry Pi 2B and later](http://cdimage.ubuntu.com/releases/20.04/release/)

Available on Ansible Galaxy: [jm1.rpi_cmdline](https://galaxy.ansible.com/jm1/rpi_cmdline)

## Requirements

TODO.

## Variables

| Name      | Default value         | Required | Description                                     |
| --------- | --------------------- | -------- | ----------------------------------------------- |
| `cmdline` | *depends on os image* | no       | Content written to `/boot/firmware/cmdline.txt` |

## Dependencies

TODO.

## Example Playbook

```
- hosts: all
  tasks:
    - import_role:
        name: jm1.rpi_cmdline
```

For instructions on how to run Ansible playbooks have look at Ansible's
[Getting Started Guide](https://docs.ansible.com/ansible/latest/network/getting_started/first_playbook.html).

## License

GNU General Public License v3.0 or later

See [LICENCE.md](LICENSE.md) to see the full text.

## Author

Jakob Meng
@jm1 ([github](https://github.com/jm1), [galaxy](https://galaxy.ansible.com/jm1), [web](http://www.jakobmeng.de))
