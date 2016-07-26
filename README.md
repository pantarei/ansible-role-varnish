Ansible Role for Varnish
========================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-varnish.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-varnish)
[![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-varnish.svg)](https://github.com/pantarei/ansible-role-varnish)
[![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-varnish.svg)](https://github.com/pantarei/ansible-role-varnish/blob/master/LICENSE)

Ansible Role for Varnish Installation.

Requirements
------------

This role require Ansible 2.0 or higher.

This role was designed for Ubuntu Server 14.04 LTS and Ubuntu Server 16.04 LTS.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>parameter</th>
<th>required</th>
<th>default</th>
<th>choices</th>
<th>comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>varnish_admin_host</td>
<td>yes</td>
<td>127.0.0.1</td>
<td></td>
<td>Varnish management interface address.</td>
</tr>
<tr class="even">
<td>varnish_admin_port</td>
<td>yes</td>
<td>6082</td>
<td></td>
<td>Varnish management interface port.</td>
</tr>
<tr class="odd">
<td>varnish_listen_host</td>
<td>yes</td>
<td>127.0.0.1</td>
<td></td>
<td>Varnish client request interface address.</td>
</tr>
<tr class="even">
<td>varnish_listen_port</td>
<td>yes</td>
<td>6082</td>
<td></td>
<td>Varnish client request interface port.</td>
</tr>
<tr class="odd">
<td>varnish_secret</td>
<td>yes</td>
<td><a href="https://github.com/pantarei/ansible-role-varnish/blob/master/defaults/main.yml">defaults/main.yml</a></td>
<td></td>
<td>Secret used for authorizing access to the management port.</td>
</tr>
<tr class="even">
<td>varnish_storage</td>
<td>yes</td>
<td>malloc,256m</td>
<td></td>
<td>Specified storage backend, default with memory based backend.</td>
</tr>
<tr class="odd">
<td>varnish_backend</td>
<td>yes</td>
<td><a href="https://github.com/pantarei/ansible-role-varnish/blob/master/defaults/main.yml">defaults/main.yml</a></td>
<td></td>
<td>Backend servers providing the content Varnish will accelerate.</td>
</tr>
</tbody>
</table>

Dependencies
------------

No additional role dependencies.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: hswong3i.varnish

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-varnish/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <a href="https://twitter.com/hswong3i" class="uri" class="uri">https://twitter.com/hswong3i</a>
    -   <a href="https://github.com/hswong3i" class="uri" class="uri">https://github.com/hswong3i</a>

