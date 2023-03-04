<h1 align="left">
Kali Linux
</h1>

<h1 align="left">
🚀🚀🚀
</h1>

<br>
<br>

- [[#Root Password Recovery Nasıl Yapılır?]]
- [[#File Operations Nasıl Yapılır?]]
- [[#File Archiving Nasıl Yapılır?]]
- [[#Directory Operations Nasıl Yapılır?]]
- [[#File and Directory Permission Management Nasıl Yapılır?]]
- [[#PAM Nedir?]]
- [[#PAM Nasıl Yapılır?]]
- [[#User Management Nasıl Yapılır?]]
- [[#Group Management Nasıl Yapılır?]]
- [[#Removing User From Group Nasıl Yapılır?]]
- [[#Delete Group Nasıl Yapılır?]]
- [[#Delete User Nasıl Yapılır?]]
- [[#Network Management Nedir?]]
- [[#Network Management Nasıl Yapılır?]]
- [[#Static IP Nedir?]]
- [[#Static IP Assignment Nasıl Yapılır?]]
- [[#Dynamic IP Nedir?]]
- [[#Dynamic IP Assignment Nasıl Yapılır?]]
- [[#Nginx Nedir?]]
- [[#Nginx Installation Nasıl Yapılır?]]
- [[#SSH Nedir?]]
- [[#Encrypted Connection with SSH Nasıl Yapılır?]]
- [[#SSH Copy ID Nedir?]]
- [[#Passwordless Connection with SSH Copy ID Nasıl Yapılır?]]
- [[#Cron Nedir?]]
- [[#Rsync Nedir?]]
- [[#Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?]]
- [[#LVM Nedir?]]
- [[#Commands Used in LVM and Their Tasks Nedir?]]
- [[#LV Nasıl Oluşturulur?]]
- [[#CIFS Protokolü Nedir?]]
- [[#NFS Protokolü Nedir?]]
- [[#File Sharing Between Kali Linux and Windows Nasıl Yapılır?]]
- [[#Process Management Nedir?]]
- [[#Process Management Nasıl Yapılır?]]
- [[#Environment Variables Nedir?]]
- [[#Environment Variables Nasıl Yapılır?]]

<br>
<br>

## Root Password Recovery Nasıl Yapılır?

<br>

Kali Linux oturum açma ekranı üzerinden e tuşuna basılır.

![Root Password Recovery Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/01.png)

<br>

Karşınıza GNU GRUB ekranın geldiğini göreceksiniz. Sayfanın aşağısındaki ro quit splash kod satırı silinir.

![Root Password Recovery Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/02.png)

<br>

Sildiğiniz kod satırı yerine rw quiet init=/bin/bash kodu yazılır. Yaptığınız değişikliği kaydetmek için ctrl + x tuş kombinasyonu kullanılır.

![Root Password Recovery Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/03.png)

<br>

Karşınıza gelen Shell ekranı üzerinden passwd komutunu yazdıktan sonra enter tuşuna basılır.

![Root Password Recovery Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/04.png)

<br>

Daha sonra yeni root kullanıcı şifresi belirlenir.

![Root Password Recovery Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/05.png)

<br>

Belirlemiş olduğunuz şifre ile Kali Linux üzerinden root kullanıcısı ile oturum açabilirsiniz.

![Root Password Recovery Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/06.png)

<br>
<br>

## File Operations Nasıl Yapılır?

<br>

Dosya oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo touch /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/01.png)

<br>

Dosya içeriğini okumak için aşağıdaki komut kullanılır.

```sh
sudo cat /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/02.png)

<br>

Dosya içeriğini tersten okumak için aşağıdaki komut kullanılır.

```sh
sudo tac /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/03.png)

<br>

Dosya içeriğini tersten görmek için aşağıdaki komut kullanılır.

```sh
sudo rev /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/04.png)

<br>

İstenilen bilgileri komut satırına yazdırmak için aşağıdaki komut kullanılır.

```sh
sudo echo "Hello World!"
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/05.png)

<br>

Dosya içeriğini okumak için aşağıdaki komut kullanılır. Sayfanın altındaki -- More -- (99%) yazan yazı bizlere sayfa içeriğinin devamı olduğunu belirtiyor. Sayfanın devamını okumak isterseniz enter tuşu ile adım adım alt satırları okuyabilirsiniz. Ayrıca space tuşu ile sayfa sayfa atlayarak sayfa içeriğini inceleyebilirsiniz. Bir önceki sayfaya geri dönmek isterseniz b tuşu, sayfadan çıkmak isterseniz q tuşuna basılır.

```sh
sudo more /etc/profile
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/06.png)

<br>

Dosya içeriğinin ilk 10 satırını komut satırı üzerinden görüntülemek isterseniz aşağıdaki komut kullanılır.

```sh
sudo head /etc/profile
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/07.png)

<br>

Dosya içeriğinin son 10 satırını komut satırı üzerinden görüntülemek isterseniz aşağıdaki komut kullanılır.

```sh
sudo tail /etc/profile
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/08.png)

<br>

Dosya içeriğindeki satırları komut satırı üzerinden numaralanmış olarak görmek isterseniz aşağıdaki komut kullanılır.

```sh
sudo nl /etc/profile
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/09.png)

<br>

Dosya içeriğinde bulunan satır sayısı, kelime sayısı ve karakter sayısını komut satırına yazdırmak için aşağıdaki komut kullanılır.

```sh
sudo wc Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/10.png)

<br>

Dosya içeriğini komut satırı üzerinden alfabetik sıraya göre görmek isterseniz aşağıdaki komut kullanılır.

```sh
sudo sort /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/11.png)

<br>

İki dosya içeriğini komut satırı üzerinden yan yana görmek isterseniz aşağıdaki komut kullanılır.

```sh
sudo paste /home/kali/Desktop/Linux /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/12.png)

<br>

İki dosya içeriğindeki verileri satır satır karşılaştırmak için aşağıdaki komut kullanılır.

```sh
sudo diff /home/kali/Documents/Linux /home/kali/Downloads/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/13.png)

<br>

İki dosya içeriğindeki verileri birleştirmek için aşağıdaki komut kullanılır.

```sh
sudo join /home/kali/Documents/Linux /home/kali/Downloads/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/14.png)

<br>

Yazmak istediğiniz ifadeleri hem komut satırına yansıtıp hem de bu ifadeleri bir dosya içeriğine kayıt etmek için aşağıdaki komut kullanılır. Daha sonra komut satırı üzerinden yazdığınız ifadeleri kaydetmek için ctrl + d tuş kombinasyonu kullanılır.

```sh
sudo tee /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/15.png)

<br>

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/16.png)

<br>

Dosyalar arasında karşılaştırma yapmak için aşağıdaki komut kullanılır.

```sh
sudo cmp /home/kali/Desktop/Linux /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/17.png)

<br>

Dosya içeriğindeki herhangi bir kelimeye sorgulamak için aşağıdaki komut kullanılır.

```sh
sudo grep Ubuntu /home/kali/Documents/Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/18.png)

<br>

Dizin adresini bilmediğiniz ama ismini hatırladığınız dosyayı bulmak için aşağıdaki komut kullanılır.

```sh
sudo find /etc -name local
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/19.png)

<br>

Resim dosyalarını listelemek için aşağıdaki komut kullanılır.

```sh
sudo find /home/kali -name *jpg
```

Listelenen dosyaların konum ve varlık bilgilerini xargs komutuna | argümanı ile aktarmış olursunuz. Daha sonra xargs komutu ise eline geçen bu bilgiler ile dosyaların konumunu bulup resim dosyalarını tek tek silme işlemini gerçekleştirmek için aşağıdaki komut kullanılır.

```sh
sudo find /home/kali -name *jpg | xargs rm
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/20.png)

<br>

Dosya içeriğindeki verilerin belirli sütununu filtrelemek için aşağıdaki komut kullanılır.

```sh
sudo awk '{print $1}' Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/21.png)

<br>

Dosya içeriğindeki Kali Linux satırını silmek için aşağıdaki komut kullanılır.

```sh
sudo sed '/Kali Linux/d' Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/22.png)

<br>

Dosya kopyalamak için aşağıdaki komut kullanılır.

```sh
sudo cp Linux /home/kali/Downloads/
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/23.png)

<br>

Dosya taşımak için aşağıdaki komut kullanılır.

```sh
sudo mv Linux /home/kali/Downloads/
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/24.png)

<br>

Dosya silmek için aşağıdaki komut kullanılır.

```sh
sudo rm Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/25.png)

<br>

Dosya içeriğine rastgele bitler yazarak dosyanın okunmaz hale gelmesi için aşağıdaki komut kullanılır.

```sh
sudo shred Linux
```

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/26.png)

<br>

![File Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/27.png)

<br>
<br>

## File Archiving Nasıl Yapılır?

<br>

Dosya arşivlemek için aşağıdaki komut kullanılır.

```sh
sudo tar -cf Linux.tar Linux
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/28.png)

<br>

Arşivlediğiniz dosyayı dışarı çıkarmak için aşağıdaki komut kullanılır.

```sh
sudo tar -xf Linux.tar
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/29.png)

<br>

Dosya sıkıştırma işlemi için aşağıdaki komut kullanılır.

```sh
sudo gzip Linux
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/30.png)

<br>

Dosya sıkıştırma işlemi için aşağıdaki komut kullanılır.

```sh
sudo bzip2 Linux
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/31.png)

<br>

Dosya arşivleme ve sıkıştırma işlemini birlikte kullanmak için aşağıdaki komutlar kullanılır.

```sh
sudo tar -czvf Linux.tar.gz Linux
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/32.png)

<br>

```sh
sudo tar -cjvf Linux.tar.bz2 Linux
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/33.png)

<br>

Arşivlediğiniz dosyayı dışarı çıkarmak için aşağıdaki komutlar kullanılır.

```sh
sudo tar -xzvf Linux.tar.gz
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/34.png)

<br>

```sh
sudo tar -xjvf Linux.tar.bz2
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/35.png)

<br>

Sıkıştırılmış dosya içeriğini okumak için aşağıdaki komut kullanılır.

```sh
sudo zcat Linux.gz
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/36.png)

<br>

Sıkıştırılmış dosya içeriğini okumak için aşağıdaki komut kullanılır.

```sh
sudo bzcat Linux.bz2
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/37.png)

<br>

Sıkıştırılmış dosya içeriğinde arama yapmak için aşağıdaki komut kullanılır.

```sh
sudo zgrep Ubuntu Linux.gz
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/38.png)

<br>

Sıkıştırılmış dosya içeriğinde arama yapmak için aşağıdaki komut kullanılır.

```sh
sudo bzgrep Ubuntu Linux.bz2
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/39.png)

<br>

Dosya sıkıştırma işlemi için aşağıdaki komut kullanılır.

```sh
sudo zip Linux.zip Linux
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/40.png)

<br>

Sıkıştırılmış dosyayı dışarı çıkarmak için aşağıdaki komut kullanılır.

```sh
sudo unzip Linux.zip
```

![File Archiving Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/41.png)

<br>
<br>

## Directory Operations Nasıl Yapılır?

<br>

Bulunduğunuz dizinin konumunu öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo pwd
```

![Directory Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/42.png)

<br>

Gitmek istediğiniz dizin adresine geçiş yapmak için aşağıdaki komut kullanılır.

```sh
cd /home/kali/Desktop/Linux/
```

![Directory Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/43.png)

<br>

Bulunduğunuz dizini listelemek için aşağıdaki komut kullanılır.

```sh
ls
```

![Directory Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/44.png)

<br>

Dizin oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo mkdir /home/kali/Documents/Linux
```

![Directory Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/45.png)

<br>

Dizin silmek için aşağıdaki komut kullanılır.

```sh
sudo rm -r /home/kali/Documents/Linux/
```

![Directory Operations Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/46.png)

<br>
<br>

## File and Directory Permission Management Nasıl Yapılır?

<br>

Bir dosyanın sahipliğini değiştirmek için aşağıdaki komut kullanılır.

```sh
sudo chown kali Linux
```

![File and Directory Permission Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/47.png)

<br>

Bir dosyanın grup sahipliğini değiştirmek için aşağıdaki komut kullanılır.

```sh
sudo chgrp kali Linux
```

![File and Directory Permission Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/48.png)

<br>

Linux dosyasına okuma, yazma ve çalıştırma yetkisini vermek için aşağıdaki komut kullanılır.

```sh
sudo chmod a+rwx Linux
```

![File and Directory Permission Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/49.png)

<br>

Ubuntu dosyasına okuma, yazma ve çalıştırma yetkisini vermek için aşağıdaki komut kullanılır.

```sh
sudo chmod 777 Ubuntu
```

![File and Directory Permission Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/50.png)

<br>

Dizinin özniteliklerini listelemek için aşağıdaki komut kullanılır.

```sh
lsattr
```

![File and Directory Permission Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/51.png)

<br>

Önemli gördüğünüz dosyanızın yanlışlıkla silinmesine engel olmak için chattr komutu kullanılır. Herhangi bir yanlış durumda dosyanın kaybolmasına engel olmak adına root kullanıcısının bile değişiklik yapmasına imkan tanımıyor. Sistemin bile ilgili dosyaya müdahale etmesini engellemek için dosyanızı koruma altına almış olursunuz. Dosyanızı koruma altına almak için aşağıdaki komut kullanılır.

```sh
sudo chattr +i Linux
```

![File and Directory Permission Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/52.png)

<br>

İşlem yaptığınız dosyanın korumasını kaldırmak için aşağıdaki komut kullanılır.

```sh
sudo chattr -i Linux
```

![File and Directory Permission Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/53.png)

<br>
<br>

## PAM Nedir?

<br>

Bir program kullanıcı kimlik kanıtlamasına ihtiyaç duyduğunda, PAM uygun kimlik kanıtlama şeması için gereken işlevleri içeren bir kütüphane sunar. Bu kütüphane dinamik olarak yüklendiği için kimlik kanıtlama şemasının yapılandırma dosyasını düzenlemek yeterli olur.

<br>

Esneklik PAM'ın en önemli güçlerinden birisidir. PAM belirli programların kullanıcı kimlik kanıtlaması yapamayacağı, sadece belirli kullanıcıların kimlik kanıtlaması yapabileceği, bazı programlar kimlik kanıtlaması yapmak istediğinde uyarı verecek şekilde ve hatta tüm kullanıcıları oturum açma ayrıcalıklarından mahrum bırakacak şekilde yapılandırılabilir. PAM'ın modüler tasarımı kimlik denetimi üzerindeki tüm kontrolü elinize almanıza izin verir.

<br>
<br>

## PAM Nasıl Yapılır?

<br>

PAM yapılandırma dosyalarını görmek için aşağıdaki komut kullanılır.

```sh
ls /etc/pam.d/
```

![PAM Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/01.png)

<br>

Eğer PAM yapılandırması /etc/pam.d/ dizini yerine /etc/pam.conf dosyasında saklanıyorsa PAM yapılandırma satırları biraz farklıdır. Her servisin kendi yapılandırma dosyası olması yerine tüm yapılandırmalar /etc/pam.conf dosyasında servisin adı ile başlayan satırlardan oluşur.

<br>

PAM yapılandırma dosyasını görmek için aşağıdaki komut kullanılır.

```sh
sudo nano /etc/pam.conf
```

![PAM Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/02.png)

<br>

Aşağıdaki dosya üzerinden değişiklik yapmak isterseniz ctrl + x tuş kombinasyonunu kullanarak y tuşuna basıp enter tuşu ile kaydet diyerek pencereyi kapatabilirsiniz.

![PAM Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/03.png)

<br>
<br>

## User Management Nasıl Yapılır?

<br>

Sisteminize yeni bir kullanıcı oluşturmak için kullanabileceğiniz iki farklı komut var. Bunlar adduser ve useradd komutlarıdır.

<br>

Yeni kullanıcı oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo adduser devops-temp
```

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/04.png)

<br>

Böylelikle /home/devops-temp dizini otomatik olarak oluşturuldu. Ayrıca devops-temp isimli kullanıcı devops-temp grubuna üye edildi.

<br>

Yeni oluşturduğunuz devops-temp isimli kullanıcı hesabını teyit etmek için sistemde kullanıcı hesapları ile ilgili bilgilerin tutulduğu /etc/passwd dosyasını incelemeniz gerekiyor.

<br>

Dosyayı incelemek için aşağıdaki komut kullanılır.

```sh
sudo cat /etc/passwd
```

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/05.png)

<br>

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/06.png)

<br>

Dosyanın en alt satırına baktığınız zaman yeni oluşturduğunuz devops-temp isimli kullanıcı hesabının eklenmiş olduğunu görmeniz gerekiyor.

<br>

Yeni kullanıcı oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo adduser -m devops-temp
```

Kullanıcıya ait parola oluşturma ve güncelleme işlemi için aşağıdaki komut kullanılır.

```sh
sudo passwd devops-temp
```

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/07.png)

<br>

Yeni oluşturduğunuz devops-temp isimli kullanıcı hesabını teyit etmek için sistemde kullanıcı hesapları ile ilgili bilgilerin tutulduğu /etc/passwd dosyasını incelemeniz gerekiyor.

<br>

Dosyayı incelemek için aşağıdaki komut kullanılır.

```sh
sudo cat /etc/passwd
```

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/08.png)

<br>

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/09.png)

<br>

Dosyanın en alt satırına baktığınız zaman yeni oluşturduğunuz devops-temp isimli kullanıcı hesabının eklenmiş olduğunu görmeniz gerekiyor.

<br>

Ayrıca parola bilgileri /etc/shadow isimli dosyada şifreli şekilde tutuluyor. Yeni oluşturduğunuz devops-temp isimli kullanıcı hesabının parola bilgilerini incelemek için aşağıdaki komut kullanılır.

```sh
sudo cat /etc/shadow
```

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/10.png)

<br>

![User Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/11.png)

<br>

Dosyanın en alt satırına baktığınız zaman yeni oluşturduğunuz devops-temp isimli kullanıcı hesabının parola bilgilerini görmeniz gerekiyor.

<br>
<br>

## Group Management Nasıl Yapılır?

<br>

Yeni bir grup oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo groupadd devops-grp
```

![Group Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/12.png)

<br>

Daha önce oluşturduğunuz devops-temp isimli kullanıcıyı devops-grp isimli gruba üye etmek için aşağıdaki komut kullanılır.

```sh
sudo gpasswd -a devops-temp devops-grp
```

![Group Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/13.png)

<br>

Kullanıcının hangi gruplara üye olduğunu görmek için aşağıdaki komut kullanılır.

```sh
sudo id devops-temp
```

![Group Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/14.png)

<br>

Bir grup oluşturulduğunda bu grubun bilgisi /etc/group isimli dosyada tutuluyor. Mevcut grupları görüntülemek için aşağıdaki komut kullanılır.

```sh
sudo nano /etc/group
```

![Group Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/15.png)

<br>

Aşağıdaki dosya üzerinden değişiklik yapmak isterseniz ctrl + x tuş kombinasyonunu kullanarak y tuşuna basıp enter tuşu ile kaydet diyerek pencereyi kapatabilirsiniz.

![Group Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/16.png)

<br>

Böylelikle sadece devops-temp ve devops-grp isimli gruplara üye olduğunuzu görmeniz gerekiyor.

<br>
<br>

## Removing User From Group Nasıl Yapılır?

<br>

En son oluşturduğunuz gruba üye olan bir kullanıcıyı gruptan çıkarmak için aşağıdaki komut kullanılır.

```sh
sudo gpasswd -d devops-temp devops-grp
```

![Removing User From Group Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/17.png)

<br>

Kullanıcının hangi gruplara üye olduğunu görmek için aşağıdaki komut kullanılır.

```sh
sudo id devops-temp
```

![Removing User From Group Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/18.png)

<br>
<br>

## Delete Group Nasıl Yapılır?

<br>

En son oluşturduğunuz grubu silmek için aşağıdaki komut kullanılır.

```sh
sudo groupdel devops-grp
```

![Delete Group Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/19.png)

<br>

Mevcut grupları görüntülemek için aşağıdaki komut kullanılır.

```sh
sudo nano /etc/group
```

![Delete Group Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/20.png)

<br>

Aşağıdaki dosya üzerinden değişiklik yapmak isterseniz ctrl + x tuş kombinasyonunu kullanarak y tuşuna basıp enter tuşu ile kaydet diyerek pencereyi kapatabilirsiniz.

![Delete Group Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/21.png)

<br>

Böylelikle sadece devops-temp isimli gruba üye olduğunuzu görmeniz gerekiyor.

<br>
<br>

## Delete User Nasıl Yapılır?

<br>

En son oluşturduğunuz kullanıcıyı /home dizini ile birlikte silmek için aşağıdaki komut kullanılır.

```sh
sudo deluser --remove-home devops-temp
```

![Delete User Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/pam-user-group-management/22.png)

<br>
<br>

## Network Management Nedir?

<br>

Bir sistemdeki yazılım, donanım, ürün yazılımı, dökümantasyon ve test özelliklerinde yapılan değişiklikleri kontrol ederek bir ağdaki güvenlik özelliklerinin yönetimini ifade eder. Bu alan, sistemi geliştikçe ve büyüdükçe kontrol altında tutar, kalite ve güvenliği korur.

<br>

## Network Management Nasıl Yapılır?

<br>

Ağ bağlantı kartlarını listelemek için aşağıdaki komut kullanılır.

```sh
sudo ifconfig
```

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/01.png)

<br>

Hedef sunucu adresi ile sisteminiz arasında iletişimin sağlanıp sağlanmadığını kontrol ederek hedef sunucunun çalışıp çalışmadığını veya aktarım hızının ne kadar olduğunu öğrenmek için aşağıdaki komut kullanılır. Ayrıca yaptığınız işlemi durdurmak için ctrl + c tuş kombinasyonu kullanılır.

```sh
sudo ping google.com
```

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/02.png)

<br>

IP yönlendirme tablosunun içeriğini incelemek için aşağıdaki komut kullanılır.

```sh
sudo route -n
```

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/03.png)

<br>

Belirli bir hedef sunucu adresine gönderilen paketin hangi host adreslerinden geçtiğini takip etmek için aşağıdaki komut kullanılır.

```sh
sudo traceroute google.com
```

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/04.png)

<br>

Domain ne zaman kurulmuş, ne zamana kadar geçerli, kimin üzerine kayıtlı ve bunun gibi diğer tüm bilgileri incelemek için aşağıdaki komut kullanılır.

```sh
sudo whois google.com
```

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/05.png)

<br>

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/06.png)

<br>

Hedef sunucu adresi hakkında bilgi almak için aşağıdaki komutlar kullanılır.

<br>

Domain adresinden IP adresine ulaşmak için aşağıdaki komut kullanılır.

```sh
sudo host google.com
```

IP adresinden Domain adresine ulaşmak için aşağıdaki komut kullanılır.

```sh
sudo host 142.250.187.142
```

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/07.png)

<br>

Hedef sunucunun DNS adresini sorgulamak için aşağıdaki komut kullanılır.

```sh
sudo dig google.com
```

![Network Management Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/network-management/08.png)

<br>
<br>

## Static IP Nedir?

<br>

İnternete bağlanan cihazların değişmeyen IP adreslerine, Statik IP denir. Sabit olmasının sebebi büyük sistemlerde kullanılır. Örneğin sunucu gibi cihazlar ve web siteleri kendilerine ait bir Statik IP kullanırlar. Bu tarz büyük cihazların ve kurumların Statik IP kullanmalarının sebebi bunun değişmemesidir. Kullanıcı ya da kurum değiştirmediği sürece Statik IP sabit kalır.

<br>

## Static IP Assignment Nasıl Yapılır?

<br>

Bilgisayarınızın IP adresini öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo ifconfig
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/01.png)

<br>

Vereceğiniz Statik IP adresinin kullanılmadığını teyit etmek için aşağıdaki komut kullanılır.

```sh
sudo netdiscover
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/02.png)

<br>

Gateway IP adresini öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo route -n
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/03.png)

<br>

Static IP ataması yapmak için aşağıdaki komut kullanılır.

```sh
sudo mousepad /etc/network/interfaces
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/04.png)

<br>

Dosyayı açtıktan sonra aşağıdaki değerlerin ilk satırına # işaretinin eklenmesi gerekiyor. İki değeri devre dışı bırakarak yorum satırına dönüştürmüş olursunuz.

```
#auto lo
#iface lo inet loopback
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/05.png)

<br>

Static IP adresi vermek için aşağıdaki değerleri yazdıktan sonra dosyayı kaydet diyerek pencereyi kapatabilirsiniz.

```
face eth0 inet static
               address 192.168.1.200
               netmask 255.255.255.0
               broadcast 192.168.1.255
               gateway 192.168.1.1
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/06.png)

<br>

Static IP adresinin aktif olması için aşağıdaki komut kullanılır.

```sh
sudo service networking restart
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/07.png)

<br>

Statik IP adresinin aktif olması için aşağıdaki komut kullanılır.

```sh
sudo reboot now
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/08.png)

<br>

Bilgisayar açıldığı zaman ağ bağlantısının olmadığını göreceksiniz.

<br>

Ağ bağlantısını aktif etmek için aşağıdaki komut kullanılır.

```sh
sudo ifup eth0
```

Bilgisayarınızın IP adresini öğrenmek için aşağıdaki komutlar kullanılır.

```sh
sudo ifconfig
```

![Static IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/09.png)

<br>

Böylelikle Static IP ataması gerçekleşmiş oldu.

<br>
<br>

## Dynamic IP Nedir?

<br>

İnternete bağlanabilen cihazların değiştirilebilir IP adresine Dynamic IP denir. İnternete her bağlandığınızda cihazınıza, DHCP tarafından farklı bir IP adresi tanımlanır. İnternet bağlantınız kesildiğinde Dynamic IP adresiniz kesilir ve bu adres farklı bir cihaza atanır. İnternet kullanımınız sırasında da Dynamic IP adresiniz değiştirilebilir. Statik IP dolaşım için yeterli gelmediği zamanlarda ve yerlerde Dynamic IP kullanılır.

<br>
<br>

## Dynamic IP Assignment Nasıl Yapılır?

<br>

Bilgisayarınızın IP adresini öğrenmek için ifconfig komutu kullanılır.

```sh
sudo ifconfig
```

![Dynamic IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/10.png)

<br>

Dynamic IP ataması yapmak için aşağıdaki komut kullanılır.

```sh
sudo mousepad /etc/network/interfaces
```

![Dynamic IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/11.png)

<br>

Dosyayı açtıktan sonra aşağıdaki değerlerin ilk satırına # işareti koymanız gerekiyor. İki değeri devre dışı bırakarak yorum satırına dönüştürmüş olursunuz.

```
#auto lo
#iface lo inet loopback
```

![Dynamic IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/12.png)

<br>

Dynamic IP adresi vermek için aşağıdaki değerleri yazdıktan sonra dosyayı kaydet diyerek pencereyi kapatabilirsiniz.

```
auto eth0
iface eth0 inet dhcp
```

![Dynamic IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/13.png)

<br>

Dynamic IP adresinin aktif olması için aşağıdaki komut kullanılır.

```sh
sudo service networking restart
```

![Dynamic IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/14.png)

<br>

Dynamic IP adresinin aktif olması için aşağıdaki komut kullanılır.

```sh
sudo reboot now
```

![Dynamic IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/15.png)

<br>

Bilgisayarınızın IP adresini öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo ifconfig
```

![Dynamic IP Assignment Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/static-dynamic-ip/16.png)

<br>

Böylelikle Dynamic IP ataması gerçekleşmiş oldu.

<br>
<br>

## Nginx Nedir?

<br>

Nginx, email vekil sunucu, ters vekil sunucu ve yük dengeleyici olarak da çalışan bir web sunucusudur. Yazılımın yapısı eşzamansız ve olay güdümlüdür, yani birçok isteğin aynı anda işlenebilmesini mümkün kılmaktadır. Ayrıca, Nginx son derecede ölçeklenebilirdir. Bu da sunduğu hizmetin müşterinin trafiğiyle birlikte büyüdüğü anlamına gelir. Nginx ve Apache kesinlikle piyasadaki en iyi sunuculardan ikisidir.

<br>
<br>

## Nginx Installation Nasıl Yapılır?

<br>

Sisteminizde kurulu olan paketlerin, paket deposundaki versiyonları ile farkları araştırılır ve liste güncellenir. Güncelleme işlemi için aşağıdaki komut kullanılır.

```sh
sudo apt update
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/01.png)

<br>

Nginx kurulumu için aşağıdaki komut kullanılır.

```sh
sudo apt install nginx
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/02.png)

<br>

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/03.png)

<br>

Nginx servisinin durumunu kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo service nginx status
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/04.png)

<br>

Nginx servisinin durumunu kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo systemctl status nginx
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/05.png)

<br>

Nginx servisini başlatmak için aşağıdaki komut kullanılır.

```sh
sudo service nginx start
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/06.png)

<br>

Nginx servisinin durumunu kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo systemctl status nginx
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/07.png)

<br>

Nginx’in sürümünü kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo nginx -v
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/08.png)

<br>

Sisteminizin IP adresini öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo ifconfig
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/09.png)

<br>

Nginx sunucusunun çalıştığını görmek için Firefox tarayıcısı üzerinden adres çubuğuna IP adresinizi yazarak kontrol edebilirsiniz.

```
192.168.1.76
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/10.png)

<br>

Sayfa içeriğinde değişiklik yapmak için aşağıdaki komut kullanılır.

```sh
sudo nano /var/www/html/index.nginx-debian.html
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/11.png)

<br>

Aşağıdaki dosya üzerinden istediğiniz değişikliği yaptıktan sonra ctrl + x tuş kombinasyonunu kullanarak y tuşuna basıp enter tuşu ile kaydet diyerek pencereyi kapatabilirsiniz.

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/12.png)

<br>

Nginx sunucusunun çalıştığını görmek için Firefox tarayıcısı üzerinden adres çubuğuna IP adresinizi yazarak kontrol edebilirsiniz.

```
192.168.1.76
```

![Nginx Installation Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/nginx/13.png)

<br>

Böylelikle istediğiniz şekilde sayfa içeriğini değiştirebilirsiniz.

<br>
<br>

## SSH Nedir?

<br>

Ağ hizmetlerinin güvenli olmayan bir ağ üzerinden güvenli bir şekilde çalıştırılması için kullanılan bir kriptografik ağ protokolüdür. En iyi bilinen uygulaması bilgisayar sistemlerine uzaktan oturum açmak için olanıdır. Güvensiz Telnet bağlantıları yerine, SSH sayesinde cihazlarınızı İnternet üzerinden güvenli bir şekilde yönetebilirsiniz.

<br>
<br>

## Encrypted Connection with SSH Nasıl Yapılır?

<br>

Aşağıdaki komut sisteminizde kurulu olan paketlerin, paket deposundaki versiyonları ile farkları araştırılır ve liste güncellenir. Güncelleme işlemi için aşağıdaki komut kullanılır.

```sh
sudo apt update
```

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/01.png)

<br>

SSH kurulumu için aşağıdaki komut kullanılır.

```sh
sudo apt install ssh
```

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/02.png)

<br>

Aşağıdaki komut sisteminizde kurulu olan paketlerin, paket deposundaki versiyonları ile farkları araştırılır ve liste güncellenir. Güncelleme işlemi için aşağıdaki komut kullanılır.

```sh
sudo apt update
```

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/03.png)

<br>

SSH kurulumu için aşağıdaki komut kullanılır.

```sh
sudo apt install ssh
```

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/04.png)

<br>

SSH servisini başlatmak için aşağıdaki komut kullanılır.

```sh
sudo service ssh start
```

SSH servisinin durumunu kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo service ssh status
```

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/05.png)

<br>

SSH servisini başlatmak için aşağıdaki komut kullanılır.

```sh
sudo service ssh start
```

SSH servisinin durumunu kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo service ssh status
```

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/06.png)

<br>

SSH ile bağlanacağınız linuxlpt bilgisayarının IP adresini öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo ifconfig
```

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/07.png)

<br>

SSH ile kalilpt üzerinden linuxlpt bilgisayarına bağlanmak için için aşağıdaki komut kullanılır.

```sh
ssh 192.168.1.45
```

Karşınıza gelen soruya yes dedikten sonra linuxlpt bilgisayarının kullanıcı şifresini girmeniz gerekiyor.

![Encrypted Connection with SSH Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/08.png)

<br>

Böylelikle SSH ile kalilpt bilgisayarı üzerinden linuxlpt bilgisayarına başarılı bir şekilde bağlanmanız gerekiyor.

<br>
<br>

## SSH Copy ID Nedir?

<br>

Şifresiz olarak iki bilgisayar arasında SSH bağlantısı yapmak sanılanın aksine oldukça basit bir iştir. Bu yazımızda bir bilgisayara şifre sormadan SSH bağlantısı yapmak için nelerin yapılması gerektiğini ve çalışma mekanizmalarını öğreneceğiz.

<br>
<br>

## Passwordless Connection with SSH Copy ID Nasıl Yapılır?

<br>

SSH ile bağlanacağınız bilgisayarın IP adresini öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo ifconfig
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/09.png)

<br>

İlk öncelikle kalilpt bilgisayarı üzerinden aşağıdaki komut kullanılır.

```sh
ssh-keygen
```

Aşağıdaki ilk kısmı dosya ismi vermeden enter tuşuna basarak ilerlerseniz oluşturulacak dosya ismi id_rsa.pub olacaktır. Bu dosyaları .ssh/ dizini altında görebilirsiniz.

```
Enter file in which to save the key (root/.ssh/id_rsa):
```

Aşağıdaki ikinci kısmı enter tuşuna basarak geçebilirsiniz.

```
Enter passphrase (empty for no passphrase):
```

Aşağıdaki üçüncü kısmı enter tuşuna basarak geçebilirsiniz.

```
Enter same passphrase again:
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/10.png)

<br>

Yukarıda çalıştırdığınız ssh-keygen komutunun oluşturulan şifre yöntemi RSA’dır. DSA oluşturmak için komutu ssh-keygen -t dsa olarak kullanmalısınız.

<br>

İlk öncelikle kalilpt bilgisayarı üzerinden aşağıdaki komut kullanılır.

```sh
ssh-keygen
```

Aşağıdaki ilk kısmı Puplic Key için dosya ismi verebilirsiniz. Daha sonra enter tuşuna basılır. Bu dosyaları /home dizini altında görebilirsiniz.

```
Enter file in which to save the key (root/.ssh/id_rsa):
```

Aşağıdaki ikinci kısmı enter tuşuna basarak geçebilirsiniz.

```
Enter passphrase (empty for no passphrase):
```

Aşağıdaki üçüncü kısmı enter tuşuna basarak geçebilirsiniz.

```
Enter same passphrase again:
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/11.png)

<br>

Yukarıda çalıştırdığınız ssh-keygen komutunun oluşturulan şifre yöntemi RSA’dır. DSA oluşturmak için komutu ssh-keygen -t dsa olarak kullanmalısınız.

<br>

İsim vermeden oluşturduğunuz dosyayı .ssh/ dizini altında olduğunu görmek için aşağıdaki komut kullanılır.

```sh
ls -la ./ssh
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/12.png)

<br>

İsim verdiğiniz dosyayı kullanıcının /home dizini altında olduğunu görmek için aşağıdaki komut kullanılır.

```sh
ls
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/13.png)

<br>

Hiyerarşiyi bozmamak adına nginx ve nginx.pub dosyalarını .ssh/ dizini altına taşımak için aşağıdaki komut kullanılır.

```sh
sudo mv nginx* .ssh/
```

Taşıdığınız dosyların son görünümünü görmek için aşağıdaki komut kullanılır.

```sh
ls -la .ssh/
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/14.png)

<br>

Oluşturduğunuz Puplic Key’i linuxlpt bilgisayarına kopyalamanız için ilk öncelikle linuxlpt bilgisayarı üzerinden /.ssh dizinini oluşturmanız gerekiyor. Dizini oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo mkdir /home/linux/.ssh
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/15.png)

<br>

Daha sonra Puplic Key’i aşağıdaki komut aracılığı ile linuxlpt bilgisayarına kopyalamanız gerekiyor. Kopyalama sırasında bir defaya mahsus linuxlpt bilgisayarının kullanıcı şifresini yazdıktan sonra başarılı bir şekilde Puplic Key’i kopyaladığınızı görmeniz gerekiyor.

```sh
ssh-copy-id -i /home/kali/.ssh/id_rsa.pub kali@192.168.1.45
```

Aşağıdaki komut ile linuxlpt bilgisayarına şifresiz olarak başarılı bir şekilde bağlanmanız gerekiyor.

```sh
ssh kali@192.168.1.45
```

Kopyaladığınız key dosyasını görmek için aşağıdaki komut kullanılır.

```sh
ls -la .ssh/
```

![Passwordless Connection with SSH Copy ID Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/ssh-ssh-copy-id/16.png)

<br>
<br>

## Cron Nedir?

<br>

Sistemde yapılması gereken rutin işlerin zamanı geldiğinde otomatik olarak yapılması işine Cron denir. Bu rutin işlere örnek vermek gerekirse; her pazartesi günü sistemi yedeklemeniz gerekiyor diyelim, her pazartesi günü elle yapmak yerine bu işi Cron’a ekleyerek otomatiğe bağlayabilirsiniz. İşte Cron bu ve bunun gibi durumlarda sıklıkla kullanılıyor.

<br>

<br>

## Rsync Nedir?

<br>

Linux tabanlı işletim sistemlerinde sıklıkla kullanılan dosya transfer uygulamasıdır. Sunucu içerisinde ya da sunucular arası yedekleme ve dosya senkronizasyon işlemlerinde kullanılan uygulama ayrıca değişen dosyaların kopyalanmasını sağlayarak transfer işlemlerini hızlandırmaktadır. Değişen dosyalar hakkında örnek vermek gerekirse; bir klasörün yedeğini farklı bir dizine ya da sunucuya Rsync kullanarak transfer ettiniz diyelim, transfer işlemini tekrar uyguladığınızda klasör içinde sadece değişen dosyaların transfer işlemini yapacaktır. Değişmeyen dosyaların transfer işlemini yapmayacağından dolayı zamandan büyük bir oranda tasarruf edeceksiniz.

<br>
<br>

## Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?

<br>

Aşağıdaki işlemlere başlamadan önce SSH servisinin kurulu olması ve SSH Copy ID işlemlerini gerçekleştirmeniz gerekiyor.

<br>

Yukarıdaki işlemleri gerçekleştirdikten sonra linuxlpt bilgisayarın IP adresini öğrenmek için aşağıdaki komut kullanılır.

```sh
sudo ifconfig
```

![Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cron-rsync/01.png)

<br>

Dosya kopyalama işlemini başlatacağınız kalilpt bilgisayarı üzerinden servisin çalışma durumunu kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo service cron status
```

![Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cron-rsync/02.png)

<br>

Cron servisinin yapılandırma dosyasını incelemek için aşağıdaki komut kullanılır.

```sh
sudo cat /etc/crontab
```

![Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cron-rsync/03.png)

<br>

Kopyalama işlemi yapacağınız dosyayı oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo touch /home/kali/nginx
```

![Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cron-rsync/04.png)

<br>

Dosya içerisinde düzenleme yapmak için aşağıdaki komut kullanılır.

```sh
crontab -e
```

Dosya içerisinde düzenleme yapmak için aşağıdaki araç kullanılır.

```sh
1. /bin/nano
```

![Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cron-rsync/05.png)

<br>

Her gün saat 3:25’de otomatik olarak linuxlpt bilgisayarına nginx dosyasının kopyalanması için aşağıdaki komut yazılır. Daha sonra ctrl + x tuş kombinasyonunu kullanarak y tuşuna basıp enter tuşu ile kaydet diyerek pencereyi kapatabilirsiniz.

```
25 3 * * * rsync -a /home/kali/nginx kali@192.168.1.45:/home/linux/
```

![Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cron-rsync/06.png)

<br>

Kopyaladığınız dosyayı linuxlpt bilgisayarı üzerinden kontrol etmek için aşağıdaki komut kullanılır.

```sh
ls -l /home/linux/
```

Kopyaladığınız dosyayı linuxlpt bilgisayarı üzerinden kontrol etmek için aşağıdaki komut kullanılır.

```sh
sudo stat /home/linux/nginx
```

![Passwordless Automatic File Copy with Cron-Rsync Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cron-rsync/07.png)

<br>

Böylelikle kalilpt bilgisayarı üzerinden linuxlpt bilgisayarına şifresiz otomatik dosya kopyalama işlemi başarılı bir şekilde tamamlanmış oldu.

<br>
<br>

## LVM Nedir?

<br>

LVM, modüler disk veri kümesi veya kümeleri oluşturulmasını, böylelikle de istenildiğinde mevcut disk alanı üzerinde istenilen boyutlandırmanın yeniden yapabilmesini sağlar. Disk alanının yetersiz kaldığı durumlarda LVM ile oluşturulan disk veri kümesine kolaylıkla yeni disk veya disk bölümleri ilave edilebilir, ihtiyaca göre disk alanı şekillendirilebilir.

<br>

Özellikle büyük disk alanı ihtiyacı olan sistemlerde LVM ile disk veri kümeleri oluşturularak ya da sisteme yeni bir disk daha eklenerek toplam disk boyutu arttırılabilir veya sistemde pasif durumda olan bir disk bölümü aktif disk kümesine dahil edilebilir. Aynı zamanda mevcut disk bölümlerinin boyutları değiştirilebilir. Yapılacak fiziksel veri alanı değişikliklerinden sistemin mevcut haritası hiçbir şekilde etkilenmez ve yeni tanımlar yapmaya gerek kalmaz.

<br>

**Hacim Grubu (VG)**

Fiziksel ve Mantıksal hacimleri içine alan üst düzey bir katmandır.

<br>

**Fiziksel Hacim (PV)**

Fiziksel disklerden veya disk bölümlerinden oluşan kısımdır.

<br>

**Mantıksal Hacim (LV)**

Disk bölümlerinin karşılığıdır. Dosya sistemi içerir.

<br>

**Fiziksel Birimler (PE)**

Fiziksel hacim her biri eşit uzunlukta varsayılan değeri 4 MB veri parçalarına bölünmüştür.

<br>

**Mantıksal Birimler (LE)**

Mantıksal hacimlerde aynı şekilde her biri eşit uzunlukta varsayılan değeri 4 MB veri parçalarına bölünmüştür. Fiziksel Birimler ve Mantıksal Birimler arasında da birebir ilişki vardır.

<br>
<br>

## Commands Used in LVM and Their Tasks Nedir?

<br>

- Sisteme diski veya bölümü fiziksel olarak tanıtmak için pvcreate komutu kullanılır.
- Fiziksel tanımlı diskleri ve bölümleri ekrana listelemek için pvdisplay komutu kullanılır.
- Fiziksel tanımlı diskin veya bölümün tanımını iptal etmek için pvremove komutu kullanılır.
- Hacim grubu oluşturmak için vgcreate komutu kullanılır.
- Hacim grubuna disk veya bölüm eklemek için vgextend komutu kullanılır.
- Hacim grubundan disk veya bölüm çıkartmak için vgreduce komutu kullanılır.
- Hacim grubunu kaldırmak için vgremove komutu kullanılır.
- Hacim grubunu listelemek için vgdisplay komutu kullanılır.
- Mevcut hacim grubunun ayarlarını bir dosyaya yedeklemek için vgcfgbackup komutu kullanılır. Ayrıca /etc/lvm/backup dizini altına yedeklenir.
- Mevcut hacim grubunun ayarlarını dosyadan düzenlemek için vgcfgrestore komutu kullanılır.
- Tanımlı mantıksal gruptan disk alanı oluşturmak için lvcreate komutu kullanılır.
- Mantıksal sürücüleri ekrana listelemek için lvdisplay komutu kullanılır.
- Mantıksal sürücüleri kaldırmak için lvremove komutu kullanılır.
- Tanımlı mantıksal sürücülerden blok silmek için lvreduce komutu kullanılır.
- Tanımlanmış mantıksal sürücüye blok eklemek için lvextend komutu kullanılır.
- LVM komutlarını ekrana açıklamasıyla beraber listelemek için lvm komutu kullanılır.
- Sistemdeki tüm diskleri listelemek için lvmdiskscan komutu kullanılır.

<br>
<br>

## LV Nasıl Oluşturulur?

<br>

Sisteminizde bulunan disk bölümlerini listelemek için aşağıdaki komut kullanılır.

```sh
sudo fdisk -l
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/01.png)

<br>

Aşağıdaki komut ile disk bölümlendirme işlemlerini gerçekleştirmek için GParted programı kullanılır.

```sh
sudo gparted
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/02.png)

<br>

Aşağıda belirtilen /dev/sdb (5.00 GiB) disk seçilir.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/03.png)

<br>

Boş disk’e bölüm ekleyebilmek için Create Partition Table’a tıklanır.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/04.png)

<br>

Karşınıza gelen pencere üzerinden Apply’e tıklanır.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/05.png)

<br>

Yeni bir disk bölümü oluşturmak için New’e tıklanır.


![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/06.png)

<br>

Karşınıza gelen bölüm oluşturma penceresi üzerinden Add’e tıklanır.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/07.png)

<br>

Yaptığınız işlemi gerçekleştirmek için Onay vermeniz gerekiyor.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/08.png)

<br>

Karşınıza gelen pencere üzerinden Apply’e tıklanır.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/09.png)

<br>

Aşağıdaki işlem detaylarını inceledikten sonra Close diyerek pencereyi kapatabilirsiniz.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/10.png)

<br>

Disk üzerine geldikten sonra sağ tıklayıp Manage Flags’a tıklanır.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/11.png)

<br>

Aşağıdaki lvm kutucuğununu işaretlemeniz gerekiyor. Daha sonra Close diyerek pencereyi kapatabilirsiniz.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/12.png)

<br>

Aşağıda yapacağınız bir işlem kalmadığı için GParted programını kapatabilirsiniz.

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/13.png)

<br>

Sisteminizde bulunan disk bölümlerini listelemek için aşağıdaki komut kullanılır.

```sh
sudo fdisk -l
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/14.png)

<br>

Physical Volume oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo pvcreate /dev/sdb1
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/15.png)

<br>

Yukarıdaki komutu çalıştırabilmeniz için ilk öncelikle lvm2 paketini yüklemeniz gerekiyor. Paketi yüklemek için aşağıdaki komut kullanılır.

```sh
sudo apt install lvm2
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/16.png)

<br>

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/17.png)

<br>

Physical Volume oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo pvcreate /dev/sdb1
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/18.png)

<br>

Volume Group oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo vgcreate vg0 /dev/sdb1
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/19.png)

<br>

Logical Volume oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo lvcreate -L 5G -n lv0 vg0
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/20.png)

<br>

Yukarıdaki komutu çalıştırabilmeniz için Volume Group’un PE boyutu 1279 olması gerektiği bilgisi verildi. Logical Volume oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo lvcreate --extents 1279 --name lv0 vg0
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/21.png)

<br>

PV’yi listelemek için aşağıdaki komut kullanılır.

```sh
sudo pvdisplay
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/22.png)

<br>

VG’yi listelemek için aşağıdaki komut kullanılır.

```sh
sudo vgdisplay
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/23.png)

<br>

LV’yi listelemek için aşağıdaki komut kullanılır.

```sh
sudo lvdisplay
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/24.png)

<br>

Her iki yeni bölümü bir dosya sistemiyle biçimlendirmek için aşağıdaki komut kullanılır.

```sh
sudo mkfs.ext4 /dev/vg0/lv0
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/25.png)

<br>

Disk kullanımı hakkında ayrıntılı bilgiye ulaşmak için aşağıdaki komut kullanılır.

```sh
sudo df -h
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/26.png)

<br>

Diski sistemden ayırmak için aşağıdaki komut kullanılır.

```sh
sudo umount /media/kali/788d4147-f1f8-4c7f-88f8-41f200089d1e
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/27.png)

<br>

Diski istediğiniz dizine mount etmeden önce yeni bir dizin oluşturmanız gerekiyor. Yeni bir dizin oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo mkdir /home/kali/Desktop/LVM
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/28.png)

<br>

Sisteminizi yeniden başlattığınız zamam otomatik bağlanmasını istediğiniz diskin UUID değerini kopyalamanız için aşağıdaki komut kullanılır.

```sh
sudo blkid /dev/vg0/lv0
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/29.png)

<br>

Sisteminizi yeniden başlattığınız zamam otomatik bağlanmasını istediğiniz diskinizi kalıcı olarak mount etmek için aşağıdaki komut kullanılır.

```sh
sudo nano /etc/fstab
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/30.png)

<br>

Aşağıdaki dosya üzerinden en alt satıra aşağıdaki kod satırı eklendikten sonra ctrl + x tuş kombinasyonunu kullanarak y tuşuna basıp enter tuşu ile kaydet diyerek pencereyi kapatabilirsiniz.

```
UUID=788d4147-f1f8-4c7f-88f8-41f200089d1e       /home/kali/Desktop/LVM  ext4    defaults 0 0
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/31.png)

<br>

Yukarıdaki fstab dosyasında bulunan satırlar sayesinde sistem yeniden başlatıldığı zaman belirtilen dosya sistemleri otomatik olarak sisteme eklenir. Sistem yeniden başlatıldığı zaman fstab dosyası içerisinde yer alan dosya sistemlerinin belirtilen şekilde bağlanması için aşağıdaki komut kullanılır.

```sh
sudo mount -a
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/32.png)

<br>

Sistem üzerindeki diskinizi aşağıdaki komutu kullanarak da bağlayabilirsiniz.

```sh
sudo mount /dev/mapper/vg0-lv0 /home/kali/Desktop/LVM
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/33.png)

<br>

Disk kullanımı hakkında ayrıntılı bilgiye ulaşmak için aşağıdaki komut kullanılır.

```sh
sudo df -h
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/34.png)

<br>

Sisteminizde bulunan disk bölümlerini listelemek için aşağıdaki komut kullanılır.

```sh
sudo fdisk -l
```

![LV Nasıl Oluşturulur?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/lvm/35.png)

<br>
<br>

## CIFS Protokolü Nedir?

<br>

Ağ sunucusu dosyalarını ve hizmetlerini istemek için açık ve platformlar arası bir mekanizma sağlayan bir dosya paylaşım protokolüdür. İnternet ve İntranet dosya paylaşımı için Microsoft'un Sunucu İleti Bloğu (SMB) protokolünün geliştirilmiş sürümünü temel alır.

<br>
<br>

## NFS Protokolü Nedir?

<br>

Unix/Linux işletim sistemlerinin ortak bir dosya sistemine, yerel diskleri kadar kolay ulaşmasını sağlayan, RPC temelli dağıtık dosya sistemi yapısıdır. NFS sayesinde bir makinede yer alan belirli bir disk bölümü, başka makineler tarafından okunabilir ve yazılabilir. NFS, istemci-sunucu mantığı ile ve birden fazla kullanıcıyla eş zamanlı olarak dosyalar üzerinde çalışmaktadır.

<br>
<br>

## File Sharing Between Kali Linux and Windows Nasıl Yapılır?

<br>

İlk öncelikle Windows üzerinden yeni bir klasör oluşturulur.

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/01.png)

<br>

Yeni oluşturduğunuz klasörü paylaşıma açmak için Sharing sekmesine tıklanır. Daha sonra Everyone grubu için Full Control izni verilir.

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/02.png)

<br>

Yeni oluşturduğunuz klasörün izinleri için Security sekmesine tıklanır. Daha sonra Everyone grubu için Full Control izni verilir.

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/03.png)

<br>

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/04.png)

<br>

Windows üzerindeki arama kutucuğuna cmd yazarak Command Prompt penceresi açılır. Paylaşıma açtığınız yeni klasörü kontrol etmek için aşağıdaki komut kullanılır.

```
net share
```

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/05.png)

<br>

Windows bilgisayarınızın IP adresini öğrenmek için aşağıdaki komut kullanılır.

```
ipconfig
```

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/06.png)

<br>

Kali Linux üzerinden CIFS yardımcı programın paketini yüklemek için aşağıdaki komut kullanılır.

```sh
sudo apt install cifs-utils
```

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/07.png)

<br>

Windows paylaşımı için bağlantı noktası olarak kullanılacak bir dizin oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo mkdir /mnt/shared
```

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/08.png)

<br>

Paylaşımı bağlamak için aşağıdaki komut kullanılır. Daha sonra Windows bilgisayarınızdaki kullanıcı hesabınızın şifresi yazılır.

```sh
sudo mount -t cifs -o username=cloud //192.168.1.136/Shared /mnt/shared
```

<br>

> -o username=cloud - Windows bilgisayarınızın kullanıcı hesap adı yazılır.
> //192.168.1.136 - Windows bilgisayarınızın IP adresi yazılır.
> /Shared - Windows bilgisayarı üzerinden paylaşıma açtığınız klasör adı yazılır.
> /mnt/shared - Kali Linux bilgisayarı üzerinden paylaşıma açtığınız klasör adı yazılır.

<br>

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/09.png)

<br>

Kali Linux ile Windows arasındaki dosya paylaşımını kontrol etmek için paylaşıma açtığınız klasör içerisine dosya oluşturulur. Dosya oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo touch linux /mnt/shared/
```

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/10.png)

<br>

Böylelikle Kali Linux ile Windows arasındaki dosya paylaşımı başarılı bir şekilde tamamlanmış oldu.

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/11.png)

<br>

![File Sharing Between Kali Linux and Windows Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/cifs-nfs-protocol/12.png)

<br>
<br>

## Process Management Nedir?

<br>

Sistemde çalışan her program en az bir Process'den oluşur. Bir Process ön planda veya arka planda çalışarak sistemin kaynaklarını kullanabilir.

<br>

**PID**

Her Process diğerlerinden farklı Unique bir PID değerine sahiptir. Bazı komutlar sayesinde PID değerini bulduğunuz Process'leri sonlandırarak, arka planda gereksiz çalışan Process'lerin önüne geçmiş olursunuz.

<br>
<br>

## Process Management Nasıl Yapılır?

<br>

Aşağıdaki komut tek başına kullanıldığında mevcut konsol üzerinden çalıştırılmış Process’leri verir.

```sh
ps
```

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/01.png)

<br>

Process’leri hiyerarşik bir biçimde görüntülemek için aşağıdaki komut kullanılır.

```sh
pstree
```

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/02.png)

<br>

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/03.png)

<br>

Process’ler hakkında 3 saniyede bir yenilenecek şekilde anlık değişimleri görmek için aşağıdaki komut kullanılır.

```sh
top
```

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/04.png)

<br>

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/05.png)

<br>

Process numarasını ve ismini görmek için aşağıdaki komut kullanılır.

```sh
sudo pgrep -l mousepad
```

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/06.png)

<br>

Process’leri PID numarasına göre sonlandırmak için aşağıdaki komut kullanılır.

```sh
sudo kill 102637
```

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/07.png)

<br>

Process’leri isme göre sonlandırmak için aşağıdaki komut kullanılır.

```sh
sudo killall mousepad
```

![Process Management Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/process-management/08.png)

<br>
<br>

## Environment Variables Nedir?

<br>

Shell üzerinden herhangi bir komutu çalıştırmak için sırasıyla PATH Environment Variables dizinleri kontrol edilir. Komutun çalıştırılabilir dosyası PATH Environment Variables dizinlerinde varsa çalıştırabilirsiniz. PATH Environment Variables dizinlerinde yoksa çalıştıramazsınız.

<br>
<br>

## Environment Variables Nasıl Yapılır?

<br>

PATH Environment Variables dizinlerini incelemek için aşağıdaki komut kullanılır.

```sh
sudo echo $PATH
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/01.png)

<br>

PATH Environment Variables üzerinden yeni bir program eklemek için aşağıdaki adımlar uygulanır.

<br>

Dizin oluşturmak için aşağıdaki komutlar kullanılır.

```sh
sudo mkdir Linux
```

```sh
sudo mkdir Ubuntu
```

```sh
sudo mkdir Debian
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/02.png)

<br>

Oluşturduğunuz dizinin en alt klasörü üzerinden mousepad programı çalıştırılır.

```sh
sudo mousepad
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/03.png)

<br>

Belge içeriğine aşağıdaki komut yazılır.

```
echo "Welcome!"
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/04.png)

<br>

Belgeyi farklı kaydet diyerek Robot.sh ismi ile kaydetmeniz gerekiyor.

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/05.png)

<br>

Karşınıza gelen pencereyi kapatabilirsiniz.

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/06.png)

<br>

Oluşturduğunuz Robot.sh dosyası bir betik dosyasıdır. Bu betik dosyası program yerine geçen bir formattır.

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/07.png)

<br>

PATH Environment Variables üzerinden ekleyeceğiniz dizini her oturum başlangıcında sistem tarafından otomatik olarak okunan bir dosya içeriğinde olmasını ve yaptığınız değişikliği siz silene kadar geçerli olması için aşağıdaki komut kullanılır.

```sh
sudo nano /etc/bash.bashrc
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/08.png)

<br>

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/09.png)

<br>

Robot.sh programınızın tam dizin adresini aşağıdaki dosyanın en alt satırına ekledikten sonra ctrl + x tuş kombinasyonunu kullanarak y tuşuna basıp enter tuşu ile kaydet diyerek pencereyi kapatabilirsiniz.

```
PATH="/home/kali/Documents/Linux/Ubuntu/Debian":$PATH
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/10.png)

<br>

Yukarıdaki adımları tamamladıktan sonra PATH Environment Variables üzerinden dizin adresinin eklendiğini görmek için aşağıdaki komut kullanılır. Yaptığınız değişikliğin geçerli olabilmesi için bilgisayarınızı yeniden başlatmanız gerekiyor.

```sh
sudo echo $PATH
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/11.png)

<br>

Programı çalıştırmak için aşağıdaki komut kullanılır.

```sh
Robot.sh
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/12.png)

<br>

Yukarıdaki programı çalıştırabilmeniz için ilk öncelikle Robot.sh dosyasına çalıştırma yetkisi vermeniz gerekiyor. Programı çalıştırmak için aşağıdaki komut kullanılır.

```sh
sudo chmod +x Robot.sh
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/13.png)

<br>

Programı çalıştırmak için aşağıdaki komut kullanılır.

```sh
Robot.sh
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/14.png)

<br>

Böylelikle Robot.sh programını başarılı bir şekilde çalıştığını görmeniz gerekiyor.

<br>

Ayrıca sistemde bulunan tüm Environment Variables listeleme işlemi için aşağıdaki komut kullanılır.

```sh
printenv
```

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/15.png)

<br>

![Environment Variables Nasıl Yapılır?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/environment-variables/16.png)
