## Ansible Consul Role

This is taken from ansible galaxy and added some chnages as per requirement.

To get original galaxy role,
`$ ansible-galaxy install savagegus.consul`

Original Git,
`https://github.com/savagegus/ansible-consul`

## Changes

1. Service installation issue with RedHat environment with systemctl.
2. Changed the nginx conf to point correctly to UI.
3. Added new lines to setup htpassword correctly.
4. Variables changed.
`consul_use_systemd: true`
`consul_use_upstart: false`
`consul_use_initd: false`
`consul_ui_require_auth: true`
