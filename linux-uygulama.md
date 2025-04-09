# Linux Uygulama Soruları ve Cevapları

## 1. "Okul.txt" Dosyasını Oluşturma
```bash
cd Masaüstü
touch okul.txt
echo "Ad Soyad - Bölüm" > okul.txt
cat okul.txt
```
Bu komutlar, "okul.txt" dosyasını oluşturur ve içerisine ad, soyad ve bölüm bilgilerini ekler.

---

## 2. Dosyaların Birleştirilmesi
**Amaç**: "ben.txt" ve "program.txt" dosyalarını oluşturmak, içerik eklemek ve bu dosyaları birleştirerek "birleştirme.txt" dosyasını elde etmek.
```bash
cd Masaüstü
touch ben.txt
echo "Ad Soyad - Şehir" > ben.txt
touch program.txt
echo "Python C++ HTML" > program.txt
paste ben.txt program.txt > birleştirme.txt
cat birleştirme.txt
```

---

## 3. Yetkilendirme
**Amaç**: "yetki" adında bir dizin oluşturmak ve "yetkilendirme.txt" dosyasına grup ve diğer kullanıcılar için yazma yetkisi vermek.
```bash
cd Masaüstü
mkdir yetki
cd yetki
touch yetkilendirme.txt
chmod 662 yetkilendirme.txt
ls -l yetkilendirme.txt
```

---

## 4. `cat -n /etc/passwd` Komutunun İşlemi
Bu komut, sistemdeki kullanıcı bilgilerini tutan `/etc/passwd` dosyasını satır numaraları ile birlikte gösterir.

---

## 5. Komut Bloğu ve Çıktısı
**Komut Bloğu:**
```bash
echo Açık Kaynak > ders1.txt
echo İşletim Sistemi > ders2.txt
cat ders1.txt ders2.txt
```
**Beklenen Çıktı:**
```
Açık Kaynak
İşletim Sistemi
```

---

## 6. "Deneme.txt" Dökümanındaki İlk İki Satırı Okuma
```bash
head -n 2 Deneme.txt
```
Bu komut, "Deneme.txt" dosyasının ilk iki satırını gösterir.

---

## 7. "passwd" Dökümanının İlk ve Son Beş Satırı
**İlk 5 Satır:**
```bash
head -n 5 /etc/passwd
```
**Son 5 Satır:**
```bash
tail -n 5 /etc/passwd
```
Bu komutlar, `/etc/passwd` dosyasının başından ve sonundan beşer satır görüntülemek için kullanılır.

