# consul-bootstrap


Variables

```yml
---
systemd:
  path: "{{ systemd_path | default('/lib/systemd/system') }}"
dnsmasq:
  path: "{{ dnsmasq_path | default('/etc/dnsmasq.d') }}"

consul:
  bootstrap_expect: "{{ consul_bootstrap_expect | default('2') }}"
  nginx_hostname_pattern: ""
  config_dir: "{{ consul_config_dir | default('/etc/consul.d') }}"
  iface: "{{ consul_iface | default('eth0') }}"
  aws_region: "{{ consul_aws_region | default('ap-southeast-2') }}"
  agent_mode: "{{ consul_agent_mode | default('client') }}"
  join_tag: "{{consul_join_tag | default('CHANGE_ME_SOMETHING_WENT_WRONG')}}"
```

