# Linux Teorik Sorular ve Cevaplar

## 1. Özgür Yazılım Felsefesi ve Açık Kaynak Kodlu Yazılım Kavramı
Özgür yazılım, kullanıcılara yazılımı çalıştırma, kopyalama, dağıtma, inceleme, değiştirme ve geliştirme özgürlüğü tanıyan yazılımdır. Açık kaynak kodlu yazılım ise bu özgürlükleri desteklerken, yazılımın kaynak kodunun da kamuya açık olmasını sağlar.

---

## 2. İşletim Sistemi Katmanları
1. **Donanım (Hardware)**
2. **Çekirdek (Kernel)**
3. **Sistem Çağrıları (System Calls)**
4. **Kabuk (Shell)**
5. **Kullanıcı Uygulamaları (User Applications)**

Bu yapı, işletim sisteminin donanım ve yazılım arasındaki etkileşimi sağlamasını kolaylaştırır.

---

## 3. CPU Zamanlama Algoritmaları
- **FCFS (First Come First Serve)**
- **SJF (Shortest Job First)**
- **Priority Scheduling**
- **Round Robin**
- **Multilevel Queue Scheduling**
- **Multilevel Feedback Queue Scheduling**

Her biri farklı sistem ihtiyaçlarına cevap verir; örneğin RR adil paylaşım sağlarken, SJF minimum ortalama bekleme süreci sunar.

---

## 4. CPU Planlama Algoritması: Round Robin (q=5)
Tablo:
```
İşlem   Süre   Öncelik
P1       10     1
P2       12     0
P3       7      3
P4       5      2
```
Quantum (zaman dilimi): 5ms

**Sıra ve zaman çizelgesi (Gantt Chart):**
```
P1 | P2 | P3 | P4 | P1 | P2 | P3 | P2
0   5   10  15  20  25  30  32  34
```

- P1: 10ms → 5 + 5
- P2: 12ms → 5 + 5 + 2
- P3: 7ms → 5 + 2
- P4: 5ms → tek seferde tamamlanır

---

## 5. Dosya: `dr-xrw-r-- 2 root root 4096 Kas 5 01:02 bin`
- `d`: bu bir dizindir
- `r-xrw-r--`: izinler (owner: read-execute, group: read-write, other: read)
- `2`: bağlantı sayısı
- `root root`: sahibi ve grubu
- `4096`: boyut (byte)
- `Kas 5 01:02`: değişitirme tarihi
- `bin`: dosya/dizin adı

---

## 6. Bulut Bilişim Hizmet Modelleri
1. **IaaS (Infrastructure as a Service)**: Sanal sunucular, depolama vb.
2. **PaaS (Platform as a Service)**: Uygulama geliştirme ortamı sunar.
3. **SaaS (Software as a Service)**: Son kullanıcıya uygulama hizmeti (Google Docs, Office 365).

---

## 7. Sanallaştırma Teknolojileri Grupları
1. **Donanım Sanallaştırma (Hypervisor-based)**
2. **İşletim Sistemi Seviyesinde Sanallaştırma (Container-based)**
3. **Paravirtualization**

---

## 8. Hypervizör, SELinux, Docker Containers ve Virtualization Kavramları
- **Hypervisor**: Sanal makineleri yöneten yazılım (VMware, KVM)
- **SELinux**: Güvenlik odaklı bir çekirdek modülü, erişim kontrolleri sağlar
- **Docker Containers**: Uygulamaları izole bir şekilde çalıştıran hafif yapılardır
- **Virtualization**: Fiziksel kaynağı mantıksal parçalara ayırarak verimli kullanım sağlar
