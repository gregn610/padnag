# padnag
padnag is a utility to synchronize PostgreSQL database roles with Active Directory groups & group members.

## Features

### Flexible
Create the database role hierarchy you need, even when the AD is differently organised.

Straight one-to-one mapping from AD to DB or link multiple OUs, groups and roles.
Database roles can associated with one or several Active Directory groups - and vice versa -
    an Active Directory group can be tied to one or several database roles.


### Safe
Fully tested against PostgreSQL versions 9.2, 9.3, 9.4, 9.5 & 9.6.

padnag safely handles removing users from a group by transferring any objects owned back to the group
    role.

padnag has <i>--test</i> mode to safely preview it's intended actions. This will not make any changes on
    the database.

padnag has <i>--verbose</i> mode and logging levels keep you informed.


### Practical
Do you need to remove leading &#35; signs or trailing suffixes from the user names?
    Active Directory attributes can be tweaked with powerful regular expressions.


### Easy to install

padnag is easy to install, it comes ready packaged for Centos7 and Ubuntu 1604 LTS distributions.
padnag is a stand alone executable with no dependencies other than the normal libc system library.


<h4>Simple to Configure</h4>
Install, provide the PostgreSQL and Active Directory parameters and you're good to go.
    The config file is TOML text file ( similar to .INI ) and can be edited with your favourite text editor.



### Integrated
Choose to use the provided Systemd service unit or run from the command line or from cron.

### Focused
padnag does one thing well.

## License
padnag is licensed under the <a href="https://mariadb.com/bsl-faq-mariadb">Business Source License</a>.
The <a href="https://bitbucket.org/teampadnag/beta/src">Source code</a> is available over at bitbucket.

