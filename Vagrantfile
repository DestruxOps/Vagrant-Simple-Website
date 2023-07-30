# -*- mode: ruby -*-

# vi: set ft=ruby :

ENV['VAGRANT_DEFAULT_PROVIDER'] = 'docker'

Vagrant.configure("2") do |config|

  config.vm.network "private_network", ip: "192.168.0.10"

  config.vm.provider "docker" do |d|

    d.image = "httpd"

    d.name = "Web"

    d.ports = ['80:80'] 

    d.remains_running = true

  end

end