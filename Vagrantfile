Vagrant.configure(2) do |config|
	config.vm.define "devops-box" do |devbox|
		devbox.vm.box = "envimation/ubuntu-xenial-docker"
    		#devbox.vm.network "public_network", ip: "192.168.0.4", bridge: "br-10611e8c8f5f"
    		devbox.vm.hostname = "devops-box"
      	devbox.vm.provision "shell", path: "scripts/install.sh"
    		devbox.vm.provider "virtualbox" do |v|
    		  v.memory = 4096
    		  v.cpus = 2
    		end
	end
end
