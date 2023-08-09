Vagrant.configure("2") do |config|

  config.vm.define "jenkins" do |jenkins|
    jenkins.vm.box = "ubuntu/bionic64"
	jenkins.vm.network "private_network", ip: "192.168.40.11"
	jenkins.vm.provider "virtualbox" do |vb|
     vb.memory = "2000"
	 vb.cpus = 2
   end
   
   jenkins.vm.provision "shell", path: "jenkins.sh"

end