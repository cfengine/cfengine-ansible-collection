# Ansible Collection - cfengine.cfengine

This collection integrates CFEngine into Ansible workflows.

## Quickstart

### Collection installation

To install this collection, run the following command:

```
ansible-galaxy collection install cfengine.cfengine
```

### Use the `cfengine` module

The `cfengine` module can be used in playbooks by adding a task like this:

```yaml
- name: Install and bootstrap CFEngine
  cfengine.cfengine.cfengine:
    policy_server: hub.example.com
    version: 3.27.1
```

The Enterprise edition is installed by default. Use the `edition` option to install the Community edition instead:

```yaml
- name: Install and bootstrap CFEngine Community
  cfengine.cfengine.cfengine:
    policy_server: hub.example.com
    edition: community
```

Check out the blog post [Installing CFEngine with Ansible](https://cfengine.com/blog/2026/install-cfengine-with-ansible/) for a more complete example.
