Role: cns.ec2-vol-snapshot
========

This role creates a snapshot of the primary EBS volume for target instance.

Requirements
------------

Nothing, it runs out of the box.

Role Variables
--------------

In the current version, you can specify the following variables:

| Name               | Default |                                                        |
|--------------------|---------|--------------------------------------------------------|
| owner              |   ---   | The owner of the instance for resource tracking (tags) |

Dependencies
------------

This package has no dependencies.

License
-------

GPLv2

Author Information
------------------

Created by Sam Morrison [@samcns](https://www.twitter.com/samcns)

Examples
--------

```yaml
---
- name: cns.ec2-vol-snapshot role test
  hosts: all
  roles:
    - { role: cns.ec2-vol-snapshot, tags: ["ec2volsnapshot"] }
```
