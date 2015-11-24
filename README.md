Ansible md5 check
=========

Using a md5 check when downloading a file using an Ansible playbook.

Requirements
------------

Ansible Version 2.0 - for the checksum task on the get_url module

Role Variables
--------------

``` yaml
deploy_user: _user who is deploying the app_
deploy_app_name: _the app name_
download_app: _app url ex. https://dl.dropboxusercontent.com/u/6735750/Declaration.txt_
download_app_md5: _md5 file url ex. https://dl.dropboxusercontent.com/u/6735750/Declaration.md5_
deploy_dir: _where the app is downloaded to ex. "/home/{{ deploy_user }}/apps"_
deploy_app_md5: _location of the md5 file once downloaded ex. "{{ deploy_dir }}/{{ deploy_app_name }}.md5"_
```

Dependencies
------------



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GNU

Author Information
------------------

Chris Livermore

[@e30chris](https://twitter.com/e30chris)

[Sandors Systems Scribbles](http://sandorsscribbl.es/)
