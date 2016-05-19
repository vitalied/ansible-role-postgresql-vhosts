Ansible Role for PostgreSQL VirtualHost
=======================================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-postgresql-vhosts.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-postgresql-vhosts)
[![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-postgresql-vhosts.svg)](https://github.com/pantarei/ansible-role-postgresql-vhosts)
[![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-postgresql-vhosts.svg)](https://github.com/pantarei/ansible-role-postgresql-vhosts/blob/master/LICENSE)

Ansible Role for PostgreSQL VirtualHost Management.

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
<th>parameter</th>
<th>required</th>
<th>default</th>
<th>choices</th>
<th>comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>postgresql_vhosts_encoding</td>
<td>yes</td>
<td>UTF8</td>
<td></td>
<td>Pass value as <code>encoding</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="even">
<td>postgresql_vhosts_id</td>
<td>yes</td>
<td>example</td>
<td></td>
<td>Unique ID for virtual host shared among other services.</td>
</tr>
<tr class="odd">
<td>postgresql_vhosts_lc_collate</td>
<td>yes</td>
<td>en_US.UTF-8</td>
<td></td>
<td>Pass value as <code>lc_collate</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="even">
<td>postgresql_vhosts_lc_ctype</td>
<td>yes</td>
<td>en_US.UTF-8</td>
<td></td>
<td>Pass value as <code>lc_ctype</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
</tr>
<tr class="odd">
<td>postgresql_vhosts_name</td>
<td>yes</td>
<td>example</td>
<td></td>
<td>Pass value as <code>name</code> to <a href="http://docs.ansible.com/ansible/postgresql_user_module.html">postgresql_user module</a>.</td>
</tr>
<tr class="even">
<td>postgresql_vhosts_password</td>
<td>yes</td>
<td>xaivoo9Z</td>
<td></td>
<td>Pass value as <code>password</code> to <a href="http://docs.ansible.com/ansible/postgresql_user_module.html">postgresql_user module</a>.</td>
</tr>
<tr class="odd">
<td>postgresql_vhosts_privs</td>
<td>yes</td>
<td><a href="https://github.com/pantarei/ansible-role-postgresql-vhosts/blob/master/defaults/main.yml">defaults/main.yml</a></td>
<td></td>
<td>Pass value to <a href="http://docs.ansible.com/ansible/postgresql_user_module.html">postgresql_user module</a>.</td>
</tr>
<tr class="even">
<td>postgresql_vhosts_template</td>
<td>yes</td>
<td>template0</td>
<td></td>
<td>Pass value as <code>template</code> to <a href="http://docs.ansible.com/ansible/postgresql_db_module.html">postgresql_db module</a>.</td>
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
        - role: hswong3i.postgresql_vhosts
          postgresql_vhosts_id: "example"
          postgresql_vhosts_pass: "xaivoo9Z"
          postgresql_vhosts_user: "example"

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-postgresql-vhosts/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <a href="https://twitter.com/hswong3i" class="uri" class="uri">https://twitter.com/hswong3i</a>
    -   <a href="https://github.com/hswong3i" class="uri" class="uri">https://github.com/hswong3i</a>

