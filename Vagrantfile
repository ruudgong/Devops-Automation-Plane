Vagrant.configure(2) do |config|
	config.vm.define "devops-box" do |devbox|
		devbox.vm.box = "bento/ubuntu-18.04"
    		devbox.vm.network "private_network", ip: "192.168.33.50"
    		#devbox.vm.network "public_network", bridge: "wlo1"
    		devbox.vm.hostname = "DevOps-Automation"
      		devbox.vm.provision "shell", path: "scripts/install.sh"
    		devbox.vm.provider "virtualbox" do |v|
    		  v.memory = 2048
    		  v.cpus = 1
    		end
	end
end
