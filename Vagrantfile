Vagrant.configure("2") do |config|

  # Testing different boxes
  config.vm.define "stretch" do |subconfig|
    subconfig.vm.box = "debian/stretch64"
  end

  #config.vm.define "xenial" do |subconfig|
  #  subconfig.vm.box = "ubuntu/xenial64"
  #end

  #config.vm.define "bionic" do |subconfig|
  #  subconfig.vm.box = "ubuntu/bionic64"
  #end

  # Provisionning
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "test.yml"
  end
end

# vi:syntax=ruby
