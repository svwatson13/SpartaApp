Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.10.100"
  config.hostsupdater.aliases = ["development.local"]
  # Syncing a folder
  config.vm.synced_folder "app", "/app" #{To sync folder}, {to sync on vm}
  # Provisioning
  config.vm.provision "shell", path: "environment/spec-tests/provision.sh"

end
