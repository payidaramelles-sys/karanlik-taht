# Sürüm notları

## v1.0.0 — 28 Ekim 2026

İlk genel sürüm. Oyun canlı: **https://taht.mehmetacar.org**

### Dünyalar
- **Valdris** başkenti: güvenli bölge, PvP kapalı, beş NPC (demirci, simyacı, arena ustası, zindan kâtibi, ırk eğitmeni).
- **Kül Ovaları** (Sv 1–8), **Kararmış Orman** (8–18), **Kırık Tapınak** (18–28), **Cehennem Yarığı** (28–40) av alanları.
- Yarık'ın sonunda boss: **Kemik Ejderha** (9000 can).
- Haritalar panelinden bölgeler arası seyahat; her bölgenin kendi ışık/pus atmosferi.

### Karakter
- **6 ırk**: İnsan, İskelet, Şeytan, Balçık, Canavar Adam, Orman Elfi — her biri kendi pasifi, başlangıç statları ve silah yatkınlığıyla.
- **5 silah yolu**: Kılıç, Mızrak, Yay, Kalkan, Asa — her biri üç yetenek.
- **4 basamaklı ırk ağacı**: iki stat/direnç düğümü + iki gerçek yetenek; düşen **ırk özü** ile sırayla açılır.
- Kalıcı ilerleme: seviye, statlar, altın, ırk özü ve ağaç durumu sunucuda saklanır.
- Seviye sınırı 50; seviye arttıkça statlar, can ve mana büyür.

### Dövüş
- Sunucu otoriteli hasar, menzil, kaçınma, kritik ve zırh hesabı.
- Elementler: fiziksel, ateş, zehir, karanlık, kutsal — dirençler ve bağışıklıklar ırka göre değişir.
- Statü etkileri: kanama, zehir, yavaşlatma, sersemletme, kalkan, zırh aşınması.
- Alan etkili yetenekler, ileri atılma (dash), yansıtma ve kökleme.
- **PvP**: güvenli bölge dışında oyuncular birbirine saldırabilir; PvP için ayrı hasar dengesi.
- Yeni oyuncu affı: 5. seviyeye kadar alınan hasar %30 azalır.

### Sosyal
- Canlı sohbet (Enter), oyuncu listesi, bölge başına çevrimiçi sayaç.
- Aynı haritada diğer oyuncuların gerçek zamanlı konumu ve yetenek efektleri.

### Arayüz
- Pixel-art HUD: can/mana çubukları, altın ve ırk özü sayacı, yetenek çubuğu (kısayol tuşlarıyla eşleşen).
- Minimap ve bölge bilgisi, ırk ağacı paneli, haritalar paneli.
- Türkçe arayüz, açılıp kapanan ses efektleri.

### Altyapı
- Tek Node.js süreci: HTTP + WebSocket + derlenmiş istemci; ayrı web sunucusu/CDN gerekmez.
- SQLite ile kalıcı veri; sunucu kapanırken açık oyuncular kaydedilir.
- HTTPS, güvenli oturum çerezi, hız sınırları ve CSRF koruması.
- Günlük otomatik veritabanı yedeği.
- Sürüm öncesi kapsamlı hata/güvenlik/performans denetimi: oturum yönetimi, yetki kontrolleri,
  kayıt tutarlılığı ve ağ katmanı sertleştirildi.

### Bilinen sınırlamalar
- Oyun klavye + fare odaklı; dokunmatik için özel bir arayüz yok.
- E-posta doğrulaması ve parola sıfırlama akışı bulunmuyor.
- v1 kapsamı dışında bırakılanlar: envanter/eşya, zindan, lonca, meslek ve binek sistemleri.
