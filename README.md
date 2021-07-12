- [About](#about)
- [Variables](#variables)

# About

This role changes the defaults users password, creates a new group and a new user, generates a ssh key for the new user and add the new user to the sudo group.
Additionally, the ssh key of the user executing the playbook will be copied to the new and the default user.

# Variables

For defaults see `defaults/main.yml`.

| Variable                  | Description                       | Default | Optional/Required |
|---------------------------|-----------------------------------|---------|-------------------|
| default_user              | Username of the default user      | null    | Required          |
| default_user_new_password | New password for the default user | null    | Required          |
| new_user                  | Username of the new user          | null    | Required          |
| new_user_password         | Password for the new user         | null    | Required          |
| new_user_PUID             | UID for the new user              | null    | Required          |
| new_user_PGID             | GID for the new user              | null    | Required          |