# Ansible Role: jm1.rpi_cmdline

This role helps to setup the kernel cmdline on Raspberry Pi.

**Tested OS images**
- [`Ubuntu 20.04 LTS` (`arm64`) for Raspberry Pi 2B and later](http://cdimage.ubuntu.com/releases/20.04/release/)

Available on Ansible Galaxy: [jm1.rpi_cmdline](https://galaxy.ansible.com/jm1/rpi_cmdline)

## Requirements

None

## Variables

| Name      | Default value         | Required | Description                                     |
| --------- | --------------------- | -------- | ----------------------------------------------- |
| `cmdline` | *depends on os image* | no       | Content written to `/boot/firmware/cmdline.txt` |

## Dependencies

| Name         | Description                                                   |
| ------------ | ------------------------------------------------------------- |
| `jm1.common` | Sets common facts and variables, e.g. `distribution_codename` |

## Example Playbook

```
- hosts: all
  tasks:
    - import_role:
        name: jm1.rpi_cmdline
```

## License

GPL3

## Author

Jakob Meng
@jm1 ([github](https://github.com/jm1), [galaxy](https://galaxy.ansible.com/jm1), [web](http://www.jakobmeng.de))
