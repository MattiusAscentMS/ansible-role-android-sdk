Role Name
=========

An Ansible role to install the Android SDK.


Dependencies
------------
Oracle Java

Role Variables
--------------
- `android_sdk_cache_dir`: (default: `/tmp/ansible-cache`) Cache folder for downloads
- `android_sdk_version`: (default: `24.4.1`) SDK version to download
- `android_sdk_zipfile`: (default: `android-sdk_r{{android_sdk_version}}-linux.tgz`) - Zip file to download
- `android_sdk_folder`:  (default: `android-sdk-linux`) - Folder to extract the SDK to
- `android_sdk_tools`: (default: none) - SDK tools to install


Example Playbook
----------------
    - hosts: servers
      roles:
         - { role: munkyjunky.android-sdk }


License
-------
MIT
