# Ansible playbook for Amnotbot

This playbook installs my [amnotbot](https://github.com/gpoppino/amnotbot) fork as a Docker container into a Linux machine (RedHat or Raspbian).

## Running the playbook

You can run this playbook in the following way after cloning the repo:

`# ansible-playbook -i inventory playbook.yml`

## Variables

You should edit the following variables:

- **amnotbot_config_path** in `roles/amnotbot/defaults/main.yml`. This is the directory of the config files of amnotbot in docker_host.
- **ansible_host** in `host_vars/docker_host`. You should replace *YOUR_REAL_HOSTNAME* to point to your docker host.
- OPTIONAL: **amnotbot_image** in `roles/amnotbot/defaults/main.yml`. Amnotbot's image location.
