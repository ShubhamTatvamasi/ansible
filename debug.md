# Debug

Ansible Debug Task:
```yaml
- name: Print all available facts
  ansible.builtin.debug:
    var: ansible_facts
```
