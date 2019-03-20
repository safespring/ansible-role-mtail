mtail setup
=========

This playbook installs mtail binary from github release page.

Requirements
------------

Only systemd-based systems are supported for now. Pull-requests are welcome.


Role Variables
--------------

### mtail_version

mtail release version, defaults to newest version in the [page](https://github.com/google/mtail/releases).

### mtail_args

Raw argument to `mtail` program, defaults to `-progs /usr/local/etc/mtail -logs /var/log/syslog`

There is a default mtail program directory, which contains a simple log line counter for `NetworkManager`.

When you set this value, don't forget setting progs argument.


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
      - role: hkwi.mtail
        mtail_version: v3.0.0-rc26

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
