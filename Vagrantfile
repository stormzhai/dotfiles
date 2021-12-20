# -*- mode: ruby -*-
# vi: set ft=ruby :

$centos_script = <<-SCRIPT
mv /etc/yum.repos.d /etc/yum.repos.d.orig.$(date -Iseconds)
mkdir -p /etc/yum.repos.d/
wget -qO /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-7.repo
SCRIPT

$rhel7_script = <<-SCRIPT
mv /etc/yum.repos.d /etc/yum.repos.d.orig.$(date -Iseconds)
mkdir -p /etc/yum.repos.d/
wget -qO /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-7.repo
sed -i 's/$releasever/7/g' /etc/yum.repos.d/CentOS-Base.repo
sed -i 's/PasswordAuthentication.*/PasswordAuthentication yes/g' /etc/ssh/sshd_config
systemctl restart sshd
SCRIPT

$debian_script = <<-SCRIPT
cp /etc/apt/sources.list /etc/apt/sources.list.orig.$(date -Iseconds)
sed -i 's http://.*.debian.org http://mirrors.aliyun.com g' /etc/apt/sources.list
SCRIPT

$ubuntu_script = <<-SCRIPT
cp /etc/apt/sources.list /etc/apt/sources.list.orig.$(date -Iseconds)
sudo sed -i 's http://.*.ubuntu.com http://mirrors.ustc.edu.cn/ g' /etc/apt/sources.list
SCRIPT


Vagrant.configure(2) do |config|
  if Vagrant.has_plugin?("vagrant-vbguest")
    config.vbguest.auto_update = false
  end

    config.vm.define "node1" do |s|
       s.vm.box = "bento/ubuntu-16.04"
        s.vm.box_url = "http://files.saas.hand-china.com/vagrant/bento_ubuntu-16.04.box"
        s.vm.hostname = "node1"
        s.vm.network "private_network", ip: "192.168.56.11"
        # s.vm.network "forwarded_port", guest: 6443, host: 6443
        # s.vm.network "forwarded_port", guest: 8443, host: 8443
        #s.vm.synced_folder ".", "/vagrant", disabled: true
        s.vm.synced_folder ".", "/vagrant"
        s.vm.provision "shell", inline: $ubuntu_script
        s.vm.provider "virtualbox" do |v|
            v.memory = 8192
            v.cpus = 4
        end
    end

end
