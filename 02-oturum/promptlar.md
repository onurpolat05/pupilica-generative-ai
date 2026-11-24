# 2. ders · promptlar

Ders sırasında kullanılan bütün mesajlar. Her kutunun sağ üstündeki düğmeyle kopyalayabilirsin.

Kulüp, etkinlikler, Elif ve ders notu kurgusal; kendi bilginle değiştirip dene.

## 1. İleri görev tanımı · kulüp takvimi

Hepsi AI Studio'da (aistudio.google.com), varsayılan ayarlarla.

### Teknik 1 · Örnekle göster

Önce örneksiz, yeni bir sohbette:

```text
Rol: Bir üniversite kulübünün sosyal medyasını yöneten deneyimli bir içerik editörüsün.
Görev: Kampüs Girişimcilik Kulübü'nün 3 Aralık etkinliği için bir Instagram postu yaz.
Bağlam: Kulübün Aralık etkinlikleri:
- 3 Aralık Perşembe 18.00 · Girişimci Sohbetleri: "İlk müşterimi nasıl buldum". Konuk: bir kahve dükkânının kurucusu. Yer: İİBF Konferans Salonu.
- 8 Aralık Salı 17.30 · Excel'le Bütçe Atölyesi. Anlatan: kulüp üyesi Elif. Yer: Bilgisayar Lab 2. Kontenjan 30 kişi, kayıt formuyla.
- 11 Aralık Cuma 20.00 · Dönem Sonu Buluşması. Yer: Kampüs kafe. Kayıt yok, herkes gelebilir.
Kısıt: Listede olmayan bir bilgi ekleme (konuğun adı, ücret, ikram gibi). En fazla 3 cümle.
Format: Yalnız post metni, başka açıklama yazma.
```

Sonra yeni bir sohbette aynı mesajın altına şunu ekle:

```text
Kulübün sesi şöyle: “Kahve bahane, fikir şahane ☕ Perşembe akşamı ilk işini kuran üç mezunumuz anlatıyor… Soru getir, kahve bizden. 📍 İİBF Konferans Salonu · 18.00” Yeni postları bu tonda yaz: kısa, esprili ama abartısız, her postta yer ve saat.
```

### Teknik 2 · Parçala, ara çıktı iste

Yeni bir sohbette:

```text
Rol: Bir üniversite kulübünün sosyal medyasını yöneten deneyimli bir içerik editörüsün.
Görev: Kampüs Girişimcilik Kulübü'nün 1–11 Aralık arası Instagram ve LinkedIn paylaşım takvimini hazırla.
Bağlam: Kulübün Aralık etkinlikleri:
- 3 Aralık Perşembe 18.00 · Girişimci Sohbetleri: "İlk müşterimi nasıl buldum". Konuk: bir kahve dükkânının kurucusu. Yer: İİBF Konferans Salonu.
- 8 Aralık Salı 17.30 · Excel'le Bütçe Atölyesi. Anlatan: kulüp üyesi Elif. Yer: Bilgisayar Lab 2. Kontenjan 30 kişi, kayıt formuyla.
- 11 Aralık Cuma 20.00 · Dönem Sonu Buluşması. Yer: Kampüs kafe. Kayıt yok, herkes gelebilir.
Kısıt: Listede olmayan bir bilgi ekleme (konuğun adı, ücret, ikram gibi).

Henüz post yazma. Önce takvimin iskeletini çıkar: hangi gün, hangi platform, hangi etkinlik, postun amacı. Bitince dur, onayımı bekle.
```

### Teknik 3 · Formatı sabitle

Aynı sohbette, ikinci mesaj:

```text
İki düzeltme: Excel atölyesinin ilk duyurusunu 1 Aralık’a çek, kayıt formu ve 30 kişilik kontenjan var. Toplam paylaşımı 8’e indir, bunu tek kişi yönetiyor.

Şimdi metinleri yaz. Cevabı yalnız şu tabloyla ver, tablonun dışında hiçbir şey yazma:

Tarih | Platform | Etkinlik | Post metni | Görsel fikri

Post metni Instagram’da en fazla 3 cümle, LinkedIn’de en fazla 5 cümle.
```

### Teknik 4 · Kendi çıktısını kontrol ettir

Aynı sohbette, üçüncü mesaj:

```text
Şimdi tablodaki her satırı sana verdiğim etkinlik listesiyle karşılaştır. Tarih, saat, yer ya da kontenjan listede yazandan farklıysa, ya da listede olmayan bir bilgi eklediysen, o satırı göster ve neyin farklı olduğunu yaz.
```

## 2. Kalıcı talimat

### Elif'in sistem talimatı

AI Studio'da sağ üstteki ayar simgesi → sağ panelin en üstündeki **System instructions** kutusu. Kendi bilginle değiştir; kimlik numarası, telefon, okul numarası yazma.

```text
KİM
Ben Elif, İşletme 3. sınıf öğrencisiyim. Bu dönem Tüketici Davranışı dersini alıyorum ve pazarlamada staj arıyorum.

NASIL ANLAT
Bir kavramı anlatırken önce tek cümlelik tanım ver, sonra pazarlamadan bir örnek. Bilmediğim terimi açıkla. Türkçe yaz.

NE YAPMA
Kaynak, sayı ya da tarih uydurma; emin değilsen “emin değilim” de. Ödevimi benim yerime yazma; taslak istersem iskelet ver.
```

Talimat yalnız kullandığın tarayıcıda saklanıyor. Metni burada ya da kendi notlarında da tut. Yeni sohbette kutu boş açılır, kaydettiğin talimatı kutunun üstündeki listeden seç.

Karşılaştırma için aynı soruyu önce talimatsız, sonra talimatla sor:

```text
Tuzak seçenek etkisi nedir?
```

### Talimatı yazmayı bilmiyorsan

```text
Benim için bir sistem talimatı yazmak istiyorum. Bunu iyi yazabilmen için bana önce en fazla 6 soru sor. Yalnız soruları yaz, talimatı yazma.
```

Mesajın başına kim olduğunu ve neden kullanacağını yazarsan sorular sana göre gelir (örneğin: "Ben üniversite öğrencisiyim, ders çalışmak için kullanacağım.").

### Gemini'de

- Kişisel talimat: Ayarlar → Kişisel Zeka → "Gemini için talimatlarınız" → Ekle
- Sohbetlerin model eğitiminde kullanılmasını kapatmak: Ayarlar → Etkinlik → "Metin ve ekler dahil sohbet içeriği" kutusunun işaretini kaldır

## 3. Kendi ders notunla çalışmak · Gemini Notebook

Ders notu bu klasörde: `tuketici-davranisi-7-hafta.pdf`. notebook.google.com → Yeni not defteri → Kaynak ekle → Dosya yükle.

```text
Bu haftanın dört kısayolunu birer cümleyle özetle. Her biri için ders notundaki pazarlama örneğini de yaz.
```

```text
Tuzak seçenek etkisi bana vize sınavında nasıl sorulur? Bir örnek soru yaz ve tam puan alacak bir cevabın iskeletini çıkar.
```

Yalnız iskelet istiyorsan sonuna "cevabı yazma, yalnız başlıkları ver" ekle.

Ders notunda olmayan bir konu:

```text
Sosyal kanıt etkisi bu haftanın konusu mu? Ders notuna göre nasıl açıklanır?
```

Kendini sınamak için: Studio → Test.

## Ders arası uygulama

1. AI Studio'da kendi sistem talimatını yaz (Elif'inkini kopyalayıp değiştir).
2. Aynı soruyu önce talimatsız, sonra talimatla sor; karşılaştır.
3. Bu dönemin bir ders notunu Gemini Notebook'a yükle, üç soru sor; biri "bu bana sınavda nasıl sorulur" olsun. Ders notun yoksa ya da paylaşılmaması gerekiyorsa bu klasördeki notu kullan.

Pazartesi şu soruyla açacağız: kalıcı talimatı yazdıktan sonra aynı soruya gelen cevap nasıl değişti?
