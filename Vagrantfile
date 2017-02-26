VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(2) do |config|
  config.vm.network :forwarded_port, guest: 443, host: 4443, auto_correct: true
  config.vm.network :forwarded_port, guest: 80, host: 8080, auto_correct: true
  config.vm.network :forwarded_port, guest: 22, host: 2202, auto_correct: true, id: 'ssh'
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "footy"
  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.cpus = 1
  end
end
