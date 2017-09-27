# Ansible-Sonar
Role to Install SonarQube on CentOS with PostgreSQL as a backend

This playbook is composed of a single role of SonarQube. Inside of that role PostgreSQL, Java, SonarQube, and Apache are installed. Each set of steps are configured in their own yml file and simply included in the main role. There are two pretasks, one that updates packages, and the second that installs dependencies.

Apache is installed in order to be a reverse proxy for the server so ports are unecessary.

This playbook only supports CentOS and RHEL systems and assumes that the whole setup is on one machine.

There are variables to be set, in regards to DB UN and PW, and the Apache settings, in the group vars files.

And example hosts file has also been included.
