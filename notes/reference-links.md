
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
- Quattor: http://www.quattor.org/

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
- "Puppet claims to be forward compatible, but the reality is every version release seems to break something that makes moving forward very difficult. We are still stuck on version 2.6. I spend a week about a year an half ago trying to get to 2.7 and gave up. I'm now two weeks into trying to leap to 3.3. Puppet has numerous times had updates that broke every client on the network which has been very painful to fix. Our VMs configurations have grown to quite long manifests and as a result Puppet is using way too much CPU on our virtual cluster. A typical Puppet run takes 7-10 minutes and consumes a CPU core for the entire time. Multiply that by 250 VMs running one per hour and it adds up to a huge chunk of our CPU time. On a fresh deploy Puppet consumes a CPU core for nearly 20 minutes. The Puppet server scales really well, the client however does very poorly in my opinion."

- This is a decent review but seems to want to stay as neutral as possible. I've used puppet, chef and salt in enterprise environment and for me, salt is the clear winner with puppet being 2nd.

    Salt:
    + \+ easier to get started, learn
    + \+ easily extendable, pillars + yaml produce a very flexible combination
    + \+ quicker to write states w/ yaml then dealing w/ puppet's own language
    + \+ fast
    - \- certain states are buggy
    
    Puppet
    + \+ hiera is awesome, inheritance makes it powerful
    + \+ well established, language works like it should
    + \+ better objects (like iptables) to work w/
    - \- certificate hell (95% it just works but when it doesn't ....)

- CFengine3 on the other hand once again that demonstrates that Mark Burgess is probably 28 years ahead of the rest of us. (A quote from a competitor at the USENIX Configuration Management Summit this past summer.) But the framework has gotten the reputation of having a very steep learning curve. From what I have seen as a consultant if the drive for configuration management comes out of Ops its almost always Puppet. If the drive comes out of engineering it is almost always Chef. Cfengine is only found in shops with a existing knowledge base in CFengine.
