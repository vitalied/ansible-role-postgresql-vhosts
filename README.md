Ansible Role for PostgreSQL Database
====================================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-postgresql-vhosts.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-postgresql-vhosts)
[![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-postgresql-vhosts.svg)](https://github.com/pantarei/ansible-role-postgresql-vhosts)
[![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-postgresql-vhosts.svg)](https://github.com/pantarei/ansible-role-postgresql-vhosts/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/ansible/role/7081.svg)](https://galaxy.ansible.com/detail#/role/7081)

Ansible Role for PostgreSQL Database Management.

Requirements
------------

This role require Ansible 2.0 or higher.

This role was designed for Ubuntu Server 14.04 LTS.

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
<th align="left">parameter</th>
<th align="left">required</th>
<th align="left">default</th>
<th align="left">choices</th>
<th align="left">comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">postgresql_vhosts_id</td>
<td align="left">yes</td>
<td align="left">example</td>
<td align="left"></td>
<td align="left">Unique ID for virtual host shared among other services.</td>
</tr>
<tr class="even">
<td align="left">postgresql_vhosts_name</td>
<td align="left">yes</td>
<td align="left">example</td>
<td align="left"></td>
<td align="left">Pass value as <code>name</code> to <a href="http://docs.ansible.com/ansible/postgresql_user_module.html">postgresql_user module</a>.</td>
</tr>
<tr class="odd">
<td align="left">postgresql_vhosts_password</td>
<td align="left">yes</td>
<td align="left">xaivoo9Z</td>
<td align="left"></td>
<td align="left">Pass value as <code>password</code> to <a href="http://docs.ansible.com/ansible/postgresql_user_module.html">postgresql_user module</a>.</td>
</tr>
<tr class="even">
<td align="left">postgresql_vhosts_encoding</td>
<td align="left">yes</td>
<td align="left">UTF8</td>
<td align="left"></td>
<td align="left">Pass value as <code>encoding</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="odd">
<td align="left">postgresql_vhosts_lc_collate</td>
<td align="left">yes</td>
<td align="left">en_US.UTF-8</td>
<td align="left"></td>
<td align="left">Pass value as <code>lc_collate</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="even">
<td align="left">postgresql_vhosts_lc_ctype</td>
<td align="left">yes</td>
<td align="left">en_US.UTF-8</td>
<td align="left"></td>
<td align="left">Pass value as <code>lc_ctype</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="odd">
<td align="left">postgresql_vhosts_template</td>
<td align="left">yes</td>
<td align="left">template0</td>
<td align="left"></td>
<td align="left">Pass value as <code>template</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="even">
<td align="left">postgresql_vhosts_priv</td>
<td align="left">yes</td>
<td align="left"><a href="https://github.com/pantarei/ansible-role-postgresql-vhosts/blob/master/defaults/main.yml">defaults/main.yml</a></td>
<td align="left"></td>
<td align="left">Pass value as <code>priv</code> to <a href="http://docs.ansible.com/ansible/postgresql_user_module.html">postgresql_user module</a>.</td>
</tr>
<tr class="odd">
<td align="left">postgresql_vhosts_role_attr_flags</td>
<td align="left">yes</td>
<td align="left"><a href="https://github.com/pantarei/ansible-role-postgresql-vhosts/blob/master/defaults/main.yml">defaults/main.yml</a></td>
<td align="left"></td>
<td align="left">Pass value as <code>role_attr_flags</code> to <a href="http://docs.ansible.com/ansible/postgresql_user_module.html">postgresql_user module</a>.</td>
</tr>
</tbody>
</table>

Dependencies
------------

No additional role dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: hswong3i.postgresql_vhosts, postgresql_vhosts_id: 'example', postgresql_vhosts_name: 'example' }

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-postgresql-vhosts/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <https://twitter.com/hswong3i>
    -   <https://github.com/hswong3i>

