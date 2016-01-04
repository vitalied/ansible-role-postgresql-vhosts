Ansible Role for PostgreSQL Database
====================================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-postgresql-db.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-postgresql-db)
 [![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-postgresql-db.svg)](https://github.com/pantarei/ansible-role-postgresql-db)
 [![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-postgresql-db.svg)](https://github.com/pantarei/ansible-role-postgresql-db/blob/master/LICENSE)
 [![Ansible Role](https://img.shields.io/ansible/role/5982.svg)](https://galaxy.ansible.com/detail#/role/5982)

Ansible Role for PostgreSQL Database Management.

Requirements
------------

This role require Ansible 1.9 or higher.

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
<td align="left">postgresql_db_encoding</td>
<td align="left">yes</td>
<td align="left">UTF8</td>
<td align="left"></td>
<td align="left">Pass value as <code>encoding</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="even">
<td align="left">postgresql_db_lc_collate</td>
<td align="left">yes</td>
<td align="left">en_US.UTF-8</td>
<td align="left"></td>
<td align="left">Pass value as <code>lc_collate</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="odd">
<td align="left">postgresql_db_lc_ctype</td>
<td align="left">yes</td>
<td align="left">en_US.UTF-8</td>
<td align="left"></td>
<td align="left">Pass value as <code>lc_ctype</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="even">
<td align="left">postgresql_db_name</td>
<td align="left">yes</td>
<td align="left">example</td>
<td align="left"></td>
<td align="left">Pass value as <code>name</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="odd">
<td align="left">postgresql_db_template</td>
<td align="left">yes</td>
<td align="left">template0</td>
<td align="left"></td>
<td align="left">Pass value as <code>template</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
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
        - { role: hswong3i.postgresql_db, postgresql_db_name: 'example' }

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-postgresql-db/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <https://twitter.com/hswong3i>
    -   <https://github.com/hswong3i>

