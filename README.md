cig Ansible role
=================

Installs and configures [cig], the git productivity tool that answers
the age-old question "Can I go?"

Requirements
------------

Assumes a Debian-based host.

Role Variables
--------------
```yaml
# Base repo URL of project maintainer, used for downloading.
cig_github_repo_url: "https://github.com/stevenjack/cig"

# Version string is interpolated in URL for downloading.
# If you change the version, you must update the checksum below.
cig_version: "0.1.5"

# SHA256 checksum used to validate the download, since we don't have
# GPG signatures a la apt.
cig_checksum: "9a89351098f7f750c6972cfdb2c6aeb9753744a91ab2e2c162ac94fdc4ebbf30"
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: desktops
  roles:
    - role: conorsch.cig
```

License
-------

MIT

[cig]: https://github.com/stevenjack/cig
