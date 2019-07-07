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

### Test OpenLDAP Server
`ldapsearch -x | grep result`
* If result: 0 Success ; then its configured correctly.
* result: 32 No such object ; then its not configured correctly.

### Install phpLDAPadmin

``

### Enable memberOf overlay
https://devopsideas.com/planning-of-ldap-dit-structure-and-config-of-overlays-access-ppolicy/

### Configuring credentials for cn=config
https://devopsideas.com/installation-configuration-openldap-utilities-ubuntu/




https://devopsideas.com/openldap-graylog-ldap-integration/


https://serverfault.com/questions/73213/how-do-i-configure-reverse-group-membership-maintenance-on-an-openldap-server
