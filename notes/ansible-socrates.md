# ansible

- ansible on your client accesses hosts (no agent needed, no puppet master/chef/musto server wehere you push to (middleman) needed)
- jumphost ssh server (for security, not so big attack surface)

playbook
hosts: app-server
  name: install xyz
  apt: packagexyz
  when: {{ os }} == "ubuntu"

use several inventory files for
- production
- staging
- vagrant dev machnine

from windows:
- vagrant up
- shell provisioner - use ansible local on linux (doesnt work from win client)

ps aux|grep ngnix
tail /var/log/ngnix.loh

ansible doc 
(like man pages)

pre_tasks:
 before

roles concept (configuration injection / DI / SOLID)
with_items: ngnix_hosts  (loop through task)

advanced when roles are introduced only use roles

----
```yml
Deployemnt
hub: <branchname>


provison with ansible secrets.yml:
add user and password line
task: ansible build es
task: ansible demo es (sample data/sandbox/demo/load)
task: ansible run es

one dir for es
one dir for logstash
one dir for demo data
one dir for long storage
```
