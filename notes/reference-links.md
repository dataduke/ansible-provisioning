
# Ansible

- http://docs.ansible.com/
- http://docs.ansible.com/ansible/list_of_all_modules.html
- https://galaxy.ansible.com/
- https://groups.google.com/forum/#!forum/ansible-project
- https://github.com/ansible/ansible-modules-core

# Competition

- Salt (py, push): http://saltstack.com/
- Fabric (py): http://www.fabfile.org/
- Capistrano (rb): http://capistranorb.com/
- Chef (rb): https://www.chef.io/
- Puppet (rb): https://puppetlabs.com/
- CFEngine (C): http://cfengine.com/

# Containers (Virtual Machines, Images)

- Vagrant https://www.vagrantup.com/
- LinuxContainer (LXC, LXD) https://linuxcontainers.org/
- Docker https://www.docker.com/
- Packer https://www.packer.io/

# Plattforms

- OpenStack (Kilo, Glance) https://www.openstack.org/
- DigitalOcean
- Amazon EC2

# Reviews

- The leading configuration management and orchestration tools (Puppet vs. Chef vs. Ansible vs. Salt): http://www.infoworld.com/article/2609482/data-center/data-center-review-puppet-vs-chef-vs-ansible-vs-salt.html
- "Puppet, unlike the other three solutions, uses a *declarative* paradigm, while the others are *imperative*. Which means that, with Puppet, you specify what your configuration needs to look like, and Puppet will figure out what needs to happen to get you there. E.g, you'll say "I need nginx, node.js, php5-fpm, .... on this server, and I need these configuration files created with these contents, while respecting such and such dependencies". Puppet Master compiles the manifest and takes care of the order of execution, resulting in a configuration that matches your specified parameters. 
As mentioned, the other tools listed here (i'm not sure about Salt, but definitely Chef and Ansible), use an imperative style. Meaning, they are more script-like. You have to be mindful of the order of execution, and take care of dependencies in a linear fashion, which gets complicated fairly quickly, and is not as maintainable in a complex configuration with multiple dependency chains."
