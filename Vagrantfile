Vagrant.configure("2") do |config|
  config.vm.provision "shell", inline: <<-SHELL
      apt-get update -y
      echo "192.168.56.100  master-node" >> /etc/hosts
      echo "192.168.56.101  worker-node01" >> /etc/hosts
      echo "192.168.56.102  worker-node02" >> /etc/hosts
  SHELL
  
  config.vm.define "master" do |master|
    master.vm.box = "bento/ubuntu-22.04"
    master.vm.hostname = "master-node"
    master.vm.network "private_network", ip: "192.168.56.100"
    master.vm.provider "virtualbox" do |vb|
        vb.memory = 4048
        vb.cpus = 2
    end
  end

  (1..2).each do |i|

  config.vm.define "node0#{i}" do |node|
    node.vm.box = "bento/ubuntu-22.04"
    node.vm.hostname = "worker-node0#{i}"
    node.vm.network "private_network", ip: "192.168.56.1#{i}"
    node.vm.provider "virtualbox" do |vb|
        vb.memory = 2048
        vb.cpus = 1
    end
  end
  
  end
end
