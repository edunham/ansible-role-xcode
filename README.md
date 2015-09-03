Xcode Ansible Role
==================

Installs Xcode 6.4 and the Command Line Tools. 

Requirements
------------

YOU MUST USE YOUR OWN APPLE DEVELOPER ACCOUNT TO DOWNLOAD THE .DMG FILES.

WITHOUT THE .DMG FILES, THIS ROLE WILL NOT WORK.

I'm sorry, but proprietary software is proprietary, and also the Xcode .dmg is
2.6GB. 

* Go to [developer.apple.com](https://developer.apple.com) and make an account
* Download the [Xcode DMG](http://adcdownload.apple.com/Developer_Tools/Xcode_6.4/Xcode_6.4.dmg)
  into the `files/` directory of this role
* Download the [Command Line Tools DMG](http://adcdownload.apple.com/Developer_Tools/Command_Line_Tools_OS_X_10.10_for_Xcode_6.4/Command_Line_Tools_OS_X_10.10_for_Xcode_6.4.dmg) 
  into the `files/` directory of this role
* Leave the files' names exactly as they are, so that this playbook can find them.

Role Variables
--------------

```
xcode_dmg - filename of Xcode dmg that you downloaded
cmdline_tools_dmg - filename of the command line tools dmg
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
