- [About](#about)
- [Installation](#installation)
- [Defaults](#defaults)

# About

This role changes the defaults users password, creates a new group and a new user, generates a ssh key for the new user and add the new user to the sudo group.
Additionally, the ssh key of the user executing the playbook will be copied to the new and the default user.

# Installation

Add the following to `requirements.yml`:

```
- src: git@gitlab.com:carbonique/ansible-role-user.git
  scm: git
  name: user
  version: #Leave empty for latest. To download a specific version: use the tag as listed in repo
```

For system wide installation:
`ansible-galaxy install -r requirements.yml`

For installation to the current directory:
`ansible-galaxy install --roles-path . -r requirements.yml`

# Defaults

Defaults have been prefilled. Variables have to be added by user

For defaults see: `defaults/main.yml`
For variables see: `vars/main.yml`
