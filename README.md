# Ansible Role Vagrant Libvirt
This is an Ansible role that installs Vagrant with the Libvirt provider on Fedora.  

Tested on Fedora 36, should work on Fedora 32 and later. Other distros are not supported yet.  

## Requirements
Fedora  
### Base requirements
None  

## Variables
| Variable | Default | Description |
|----------|---------|-------------|
| `vagrant_install_libvirt` | `true` | Whether to install the libvirt plugin |
| `vagrant_libvirt_user` | `{{ ansible_user_id }}` | The user to install the plugin for |
| `vagrant_libvirt_add_user_to_group` | `true` | Add `{{ vagrant_libvirt_user }}` to `libvirt` group. |
