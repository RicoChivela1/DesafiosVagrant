# Primeiro desafio
#Nome: João Chivela
#Nacionalidade: Angolana
#Aluno da Mentoria
#Data: 22-03-2023

Vagrant.configure("2") do |config|
 
  config.vm.box = "ubuntu/trusty64"
  config.vm.box_check_update
  #Faz a leitura do script de provisionamento
  config.vm.provision :shell, path: "bootstrap.sh"
  #Faz encaminhamento de porta
  config.vm.network :forwarded_port, guest: 80, host: 4567

    config.vm.provider "virtualbox" do |vb|
    
    vb.name = "SRV-CABINDA"
    vb.memory = "1024"
    vb.cpus = "01"

  end 
end
