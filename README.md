Xcode Ansible Role
==================

Installs Xcode 6.4.

Requirements
------------

YOU MUST USE YOUR OWN APPLE DEVELOPER ACCOUNT TO DOWNLOAD THE .DMG FILE.

WITHOUT THE .DMG FILE, THIS ROLE WILL NOT WORK.

I'm sorry, but proprietary software is proprietary, and also the Xcode .dmg is
2.6GB. 

* Go to [developer.apple.com](https://developer.apple.com) and make an account
* Download the [Xcode DMG](http://adcdownload.apple.com/Developer_Tools/Xcode_6.4/Xcode_6.4.dmg)
  into the `files/` directory of this role
* Make sure that the downloaded file's name matches the value in
  `defaults/main.yaml`

Role Variables
--------------

```
xcode_dmg - filename of Xcode dmg that you downloaded
```

Example Playbook
----------------

    - hosts: mac 
      roles:
         - { role: edunham.xcode }

License
-------

MIT

Author Information
------------------

Email `ansible-xcode-role` at `edunham` dot `net`. 
