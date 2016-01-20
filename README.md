# Vagrant

Short introduction about Vagrant / Docker provided on the 20th of January 2016

[ ] [Why Vagrant?](http://devdocs.io/vagrant/why-vagrant/index)

 * for a developer

    * consistent, disposable environment without sacrifices
    (editors, debuggers, browsers)

    * all team members can run code in the same conditions
    => say goodbye to "works on my machine" bugs

 * for an operations engineer

    * disposable environment, consistent workflow
    to develop and test infrastructure management scripts
    (Chef cookbooks, Puppet modules, Ansible playbooks)

    * test scripts on remote clouds (AWS, RackSpace) 
    with same workflow

 * for a designer

    * set up everything up to focus on design

[ ] [Getting started](http://devdocs.io/vagrant/getting-started/index)

```
export PROVIDER=virtualbox

$PROVIDER

test -e Vagrantfile && echo "Box already initialized (you might want to destroy initialized box and remove Vagrantfile)?"

vagrant init ubuntu/trusty64

VAGRANT_LOG=error vagrant up

vagrant destroy
```
