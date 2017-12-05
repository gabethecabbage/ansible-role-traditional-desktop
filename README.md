# ansible-role-traditional-desktop

Ensure a traditional desktop enviroment (gnome 2/mate) is installed on RHEL

On RHEL 6 this means Gnome 2 is installed, on RHEL 7 MATE is installed from the ELREPO

## Requirements

None

## Role Variables

| Variable Name             | Defaults | Description                                                        |
|---------------------------|----------|--------------------------------------------------------------------|
| headless                  |False     | If true, the display manager won't be enabled                      |
| remove_gnome_3            |True      | by default role removes gnome 3, set to false is this is not wanted|

## Dependencies

gabethecabbage.elrepo

## Example Playbook

    ---
    - hosts: servers
      roles:
        - role: gabethecabbage.gnome2-mate
    ...

## License

BSD

## Author Information

This role was created by [Gabe Schrecker](https://github.com/gabethecabbage).

