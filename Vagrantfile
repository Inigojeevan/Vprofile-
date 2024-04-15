Vagrant.configure("2") do |config|
    config.hostmanager.enabled = true
    config.hostmanager.manage_host = true

    # database vm
    config.vm.define "db" do |db|
        db.vm.box = "eurolinux-vagrant/centos-stream-9"
        db.vm.hostname = "db"
        db.vm.network "private_network", ip: "192.168.56.15"
        db.vm.provider "virtualbox" do |vb|
            vb.memory = "600"
        end

    end
    
    # memcache vm
    config.vm.define "memcache" do |memcache|
        memcache.vm.box = "eurolinux-vagrant/centos-stream-9"
        memcache.vm.hostname = "memcache"
        memcache.vm.network "private_network", ip: "192.168.56.14"
        memcache.vm.provider "virtualbox" do |vb|
            vb.memory = "600"
        end
    end

    # RabbitMQ vm
    config.vm.define "rabbitmq" do |rabbitmq|
        rabbitmq.vm.box = "eurolinux-vagrant/centos-stream-9"
        rabbitmq.vm.hostname = "rabbitmq"
        rabbitmq.vm.network "private_network", ip: "192.168.56.13"
        rabbitmq.vm.provider "virtualbox" do |vb|
            vb.memory = "600"
        end
    end

    # Tomcat vm
    config.vm.define "tomcat" do |tomcat|
        tomcat.vm.box = "eurolinux-vagrant/centos-stream-9"
        tomcat.vm.hostname = "tomcat"
        tomcat.vm.network "private_network", ip: "192.168.56.14"
        tomcat.vm.provider "virtualbox" do |vb|
            vb.memory = "800"
        end
    end

    # Nginx vm
    config.vm.define "nginx" do |nginx|
        nginx.vm.box = "eurolinux-vagrant/centos-stream-9"
        nginx.vm.hostname = "nginx"
        nginx.vm.network "private_network", ip: "192.168.56.15"
        nginx.vm.provider "virtualbox" do |vb|
            vb.memory = "800"
        end
    end
end