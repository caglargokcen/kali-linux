# Kali Linux

<br>

- Root Password Recovery Nedir?
- File Operations Nedir?
- File Archiving Nedir?
- Directory Operations Nedir?
- File and Directory Permission Management Nedir?
- Nginx Nedir?
- SSH Nedir?
- SSH Copy ID Nedir?
- Cron Nedir?
- Rsync Nedir?
- Static IP Nedir?
- Dynamic IP Nedir?
- CIFS Protokolü Nedir?
- NFS Protokolü Nedir?
- PAM Nedir?
- LVM Nedir?
- Network Management Nedir?
- Environment Variables Nedir?
- Process Management Nedir?

<br>

# Root Password Recovery Nedir?

<br>

Kali Linux oturum açma ekranı üzerinden e tuşuna basılır.

![Root Password Recovery Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/01.png)

<br>

Karşınıza GNU GRUB ekranın geldiğini göreceksiniz. Sayfanın aşağısındaki ro quit splash kod satırı silinir.

![Root Password Recovery Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/02.png)

<br>

Sildiğiniz kod satırı yerine rw quiet init=/bin/bash kodu yazılır. Yaptığınız değişikliği kaydetmek için ctrl + x kombinasyonu kullanılır.

![Root Password Recovery Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/03.png)

<br>

Karşınıza gelen Shell ekranı üzerinden passwd komutunu yazdıktan sonra enter tuşuna basılır.

![Root Password Recovery Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/04.png)

<br>

Daha sonra yeni root kullanıcı şifresi belirlenir.

![Root Password Recovery Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/05.png)

<br>

Belirlemiş olduğunuz şifre ile Kali Linux üzerinden root kullanıcısı ile oturum açabilirsiniz.

![Root Password Recovery Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/root-password-recovery/06.png)

<br>
<br>

# File Operations Nedir?

<br>

Dosya oluşturmak için aşağıdaki komut kullanılır.

```sh
sudo touch /home/kali/Documents/Linux
```

![File Operations Nedir?](https://raw.githubusercontent.com/caglargokcen/kali-linux/master/images/file-archiving-directory-permissions-operations/01.png)
























