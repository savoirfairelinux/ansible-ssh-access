# ssh-access

Facilitates SSH access from one remote to other(s). This role first creates a private key on a
remote hosts, and then propagates that key's public key to specified hosts (must be in the
inventory) `authorized_keys`.

## Requirements

* Ansible 2.0+

## Example invocation

```
- role: ssh-access
  ssh_access_username: myuser
  ssh_access_targets:
    - host: host1
      username: user1
    - host: host2
      username: user2
```
