Vagrant.configure("2") do |config|
  config.vm.define "k8smaster01" do |vm1|
    vm1.vm.box = "ubuntu/xenial64"
    vm1.vm.hostname = 'k8smaster01'
    vm1.vm.network "private_network", ip: "10.0.0.11"

    vm1.vm.provider :virtualbox do |vb|
      vb.name = "k8smaster01"
      vb.gui = false
      vb.memory = "2048"
      vb.cpus = "2"
    end
  end

  config.vm.define "k8smaster02" do |vm2|
    vm2.vm.box = "ubuntu/xenial64"
    vm2.vm.hostname = 'k8smaster02'
    vm2.vm.network "private_network", ip: "10.0.0.12"

    vm2.vm.provider :virtualbox do |vb|
      vb.name = "k8smaster02"
      vb.gui = false
      vb.memory = "2048"
      vb.cpus = "2"
    end
  end

  config.vm.define "k8smaster03" do |vm3|
    vm3.vm.box = "ubuntu/xenial64"
    vm3.vm.hostname = 'k8smaster03'
    vm3.vm.network "private_network", ip: "10.0.0.13"

    vm3.vm.provider :virtualbox do |vb|
      vb.name = "k8smaster03"
      vb.gui = false
      vb.memory = "2048"
      vb.cpus = "2"
    end
  end

  config.vm.define "worker" do |vm4|
    vm4.vm.box = "ubuntu/xenial64"
    vm4.vm.hostname = 'worker'
    vm4.vm.network "private_network", ip: "10.0.0.14"

    vm4.vm.provider :virtualbox do |vb|
      vb.name = "worker"
      vb.gui = false
      vb.memory = "512"
    end
  end

  config.vm.define "haproxy" do |vm5|
    vm5.vm.box = "ubuntu/xenial64"
    vm5.vm.hostname = 'haproxy'
    vm5.vm.network "private_network", ip: "10.0.0.15"

    vm5.vm.provider :virtualbox do |vb|
      vb.name = "haproxy"
      vb.gui = false
      vb.memory = "512"
      
    end
  end
end

