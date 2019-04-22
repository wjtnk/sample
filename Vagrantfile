Vagrant.configure("2") do |config|
  config.vm.box = "CentOS7"
  #ローカルでアクセスするときのIPアドレス。初期設定は192.168.33.10のはず。
  config.vm.network "private_network", ip: "192.168.33.10"
  #同期先を指定。「カレントディレクトリ（.）を/vagrant以下に同期」と、「syncディレクトリを/var/www/」以下に同期する。
  config.vm.synced_folder ".", "/vagrant"
  config.vm.synced_folder "sync", "/var/www/"
end
