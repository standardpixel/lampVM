lampVM
======

This is a [vagrantfile](http://docs.vagrantup.com/) and some supporting [Ansible](http://www.ansible.com/) configurations. The idea is to have a simple way to run LAMP applications in dev. Clone this and build your application in the root. Running should just be a few steps

This was almost compleatly ripped off from the [GeoVM](http://github.com/bdon/geovm) [Brandon](http://twitter.com/bdon) made.

Things you will need to do first
--------------------------------
  * Install the [Vagrant binary](http://www.vagrantup.com/downloads)
  * Install Ansible using your OS package manager. For mac: `brew install ansible`

Running the dev server
----------------------
  * `cd` to the root directory of this repo
  * `vagrant up`
  * Go to http://localhost:8999/

  _The port 8999 might have been changed because it was already being used on this system. The actual port will be shown under this line in the output:_
  `default: Forwarding ports...`

Apache logs
-----------
`vagrant ssh -c "tail -f /var/log/apache2/error.log"`
or
`vagrant ssh -c "tail -f /var/log/apache2/error.log"`
