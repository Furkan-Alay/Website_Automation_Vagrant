# Buradaki otomasyonu kullanabilmek için aşağıdaki komutları uygulamanız gerekmektedir.
* Kendi bilgisayarınızın "C" veya "F" klasörüne kaynak kodumu clone edin.
* Sanal Makinelerin takibi için Oracle VM makinenize indirebilirsiniz.
* Gitbash terminalini kurmanız tavsiye edilir.
* Burada "finance" ve "ubuntu" klasörleri içerisindeki Vagrantfile dosyaları ile sanal makineler kurabilirsiniz.
* Vagrantfile dosyalarını açarak sanal makinelerinizin konfigürasyon ayarlarını yapabilirsiniz.
* Burada "centos" ve "ubuntu" adında iki klasör ve Vagrantfile dosyaları bulunmakta.Buradaki Vagrantfile dosyasını vagrant kodlarıyla direkt olarak kontrol edebilirsiniz
* vagrant up = Vagrantfile özelliklerine göre sanal makine başlatır.
* vagrant halt = Sanal makineyi durdurur.
* vagrant destroy= Sanal makineyi siler.
* vagrant status = Sanal makinenin durumunu ekrana getirir.
* vagrant global status= Tüm sanal makinelerin durumunu ekrana getirir.
* vagrant ssh= SSH bağlantısıyla Sanal makinenize bağlanır.
## finance
* Buradaki klasörümüzün Vagrantfile dosyasında provizyon işlemi bulunmaktadır yani ön yükleme kısmı bulunuyor.
* Vagrantfile dosyamızın içerisinde "private network" yorum satırını kaldırıp statik IP adresi vermiş olduk
* Provizyon kısmında apache web servisini indirecektir.
* Statik IP adresimizle oluşturmuş olduğumuz apache web servisine tarayıcıdan bağlanabilirsiniz.
## financeIAC
* Burada ise Provizyon kısmında belirtilen komutlar uygulanmış olacaktır.
* Buradaki Sanal makinemiz içerisine Provizyon kısmında belirtilen yerden hazır template çekilip httpd web servisimizin template kısmına aktarılmış olacaktır.
* Statik IP adresiyle bağlanabileceğimiz ve hazır template kullanan bir httpd web sitemiz olacaktır.
* Dilerseniz Provizyon kısmını özelleştirip kendizine ait web sitenizi Otomatik olarak oluşturabilirsiniz. 

## wordpressIAC
* Burada ise wordpress kurulumunu manuel kurmak yerine bizim için VM yapmaktadır.
* Statik IP adresi ile wordpress sitemize erişebiliriz.
## multiVM
* Burada birden fazla Sanal makineyi tek bir Vagrantfile ile oluşturabiliriz
* Dilersek dosyamızı ve kaynaklarını özelleştirebiliriz.
