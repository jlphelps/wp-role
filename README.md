# wp-role

Contributors  
============
Jeremy Phelps ([jeremy.lee.phelps@gmail.com](mailto:jeremy.lee.phelps@gmail.com)) and Jessica de la Cruz [@jdlc](https://github.com/jdlc)

Mission
==========
Our mission is to create an open-source Wordpress role for Ansible. This automates tasks and manages configurations that would be performed each time when creating a new Wordpress site.

Wordpress-role is licensed under the MIT license, the text of which is available [here](https://github.com/jlphelps/wp-role/blob/master/LICENSE). Each working version and iteration will be uploaded to Ansible Galaxy in the future.

Variables
=========
The following variables must be set in the Ansible job template for this role to function properly:
```yaml
  dest: /path/to/installation
  mysql_db: WordPress db username
  mysql_password: WordPress db password
  mysql_user: Wordpress db user
  ntpserver: nist.netservicesgroup.com
  remote_user: user to SSH as
  repo_url: URL of repo
  root_db_password: DB Password set upon installation
  timeout: Time in MS to wait for SSH handshake
  track_submodules: "yes" - grab submodules if necessary
  version: master
  vhosts:
    vhost.to.configure.com:
      aliases:
        - vhost.to.configure.com
        - 127.0.0.1
      enabled: "yes"
      listen:
        - "*:80"
        - "127.0.0.1:8080"
      name: vhost.to.configure.com
      root: /path/to/vhost/root
````

Version History
==========
We are in pre-release. The first completed released version will be v1.0.

Milestones
==========
Our milestones are located here on Github: [Milestones](https://github.com/jlphelps/wp-role/milestones)

Related Projects
==========
[Ansible](http://www.ansible.com) Automation software

[Ansible Galaxy] (http://galaxy.ansible.com) Hosts Ansible roles

[WordPress] (http://www.wordpress.com) Create blogs, websites, CMS
Information for Developers
==========
Want to help develop? You'll need Ansible and Ansible Tower installed. Anyone can contribute, just submit a pull request.

Information for Users
==========
This role is not functional yet. Please check back often or follow this repository to see our progress.

Want to use this in the future? You'll need Ansible and Ansible Tower installed. Here's an [introduction to Ansible Playbook Roles](http://docs.ansible.com/playbooks_roles.html).

Mailing List
==========
No mailing list for now, because it's just us two. If we get many contributors/users and need one, we'll create a Google group as mailing list.

Issue Tracker
==========
Our issue tracker is located here on Github: [Issues](https://github.com/jlphelps/wp-role/issues)

You'll need a Github account to create an issue on our tracker. Please select a Label and/or Milestone for your issue before submitting!
