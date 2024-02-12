# Görev:
Ansible kullanarak Filebeat kurulumu ve yapılandırılması.

# Adımlar
- GCP veya AWS platformlarından birinde ücretsiz hesap açılması.
- Bulut platformunun arayüzü aracılığıyla bir CentOS sanal makinesi oluşturulması.
- Sanal makinenin boyutunun ve bölgesinin seçilmesi.
- Sanal makinen IP adresini ve erişim bilgilerinin not edilmesi, ör: Kullanıcı Adı, Şife, SSH anahtarı falan.
- Ansible ile Filebeat'in kurulumunu ve yapılandırmasını otomatikleştirecek bir playbook'un hazırlanması.
- Sanal makinenin IP adresi ve erişim bilgileri kullanılarak Ansible'ın bağlanmasının sağlanması.
- Filebeat'in doğru bir şekilde kurulup yapılanması.
- Log dosyalarının Elasticsearch'e gönderildiğinden emin olunması.


# Ansible 
Ansible, otomasyon yönetimi ve uygulama dağıtımı için kullanılan açık kaynaklı bir programdır. YAML dili kullanarak çalışır. Yapılandırma dosyalarında dinamik içerik oluşturmak için Jinja'yı kullanır. Ayrıca Ansible, yönetilen makinelerde çalışması için herhangi bir ajan gerektirmez.

# Filebeat
Filebeat, Elasticsearch'ün veri toplama ailesinin bir parçası olarak kullanılan hafif bir veri nakil aracıdır.

