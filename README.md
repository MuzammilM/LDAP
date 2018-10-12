# LDAP
`sudo apt install slapd ldap-utils`
`sudo dpkg-reconfigure slapd`
* Omit LDAP server configuration: NO.
* Enter DN
* Enter Organization name
* Database backend: MDB.
* Do you want the database to be removed when slapd is purged? No.
* Move old database? Yes.
* Allow LDAPv2 protocol? No

`sudo nano /etc/ldap/ldap.conf`
BASE     dc=your-domain,dc=com
URI      ldap://localhost