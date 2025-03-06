breakfix4/SCENARIO_HTTPD
========================

The role breaks the Satellite by setting the crypto policy to a custom unsupported policy.

The role performs the following:

* Creates a new crypto policy called FIP.
* Applies the policy on the system.
* Reboot the system.

Requirements
------------

This ansible role requires the [foreman ansible modules](https://github.com/theforeman/foreman-ansible-modules/). Please install them before executing the role.

Role Variables
--------------

NA

Dependencies
------------

NA

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

~~~
# cat breakfix4yaml
---
- name: Deploy ansible role breakfix_httpd on target systems
  hosts: satellite
  become: True
  roles:
    - role: breakfix_httpd
      tags: break
~~~

License
-------

It is free software licensed under the terms of the GNU General Public License GPL v3 or later. A copy of the license can be obtained here: http://www.gnu.org/licenses/gpl-3.0.html

Author Information
------------------

This role is developed by Manu Sunil <msunil@redhat.com>, Soham Majumdar <smajumda@redhat.com>, <csedeepm@gmail.com>.
