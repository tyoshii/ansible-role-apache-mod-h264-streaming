Ansible Role: apache-mod-h264-streaming
=======================================

Build and install apache-mod-h264-streaming.

Requirements
------------

install follows yum packages:

- httpd-devel
- mod_ssl

Role Variables
--------------

- (array) h264_streaming_extensions
    - support extension value
    - default: .mp4

Dependencies
------------

no

Example Playbook
----------------

    - hosts: servers
      vars:
        h264_streaming_extensions:
          - .mp4
      roles:
         - tyoshii.apache-mod-h264-streaming

License
-------

CC-BY
