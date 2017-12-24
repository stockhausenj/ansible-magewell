Magewell
=========

Install desired version of Magewell Pro Capture Family driver.

Requirements
------------

Refer to the Magewell documentation.

Role Variables
--------------

Required variable: `magewell_src`
Example: `magewell_src: http://www.magewell.com/files/drivers/ProCaptureForLinux_3773.tar.gz`

Dependencies
------------

N/A

Example Playbook
----------------
```
$ ansible-galaxy install stockhausenj.magewell
$ ansible-playbook -i inventory.yaml install-magewell.yaml -u <ssh-user> -K
```
```
- hosts: all
  roles:
    - include_role:
        name: stockhausenj.magewell
      vars:
        magewell_src: http://www.magewell.com/files/drivers/ProCaptureForLinux_3773.tar.gz
```

License
-------

MIT
