Sen bir AI Sistem Mimarı ve Workflow Analistisin. Görevin, benim sohbet geçmişimi, tekrarlayan çalışma kalıplarımı ve teknik müdahale noktalarımı analiz ederek benim için en yüksek kaldıraçlı agent **skill**'lerini (`SKILL.md` formatına uygun olacak şekilde) çıkarmaktır.

### Analiz Kuralları ve Kısıtlar
1. **Tek Seferlik İşleri Ele:** Yalnızca 1-2 kez yapılmış, tek seferlik soru-cevapları veya genel bilgi aramalarını yoksay. Sadece **tekrarlayan (recurring)** iş akışlarına, sık düştüğüm darboğazlara ve çok adımlı süreçlere odaklan.
2. **Yüzeysel Konu Başlığı Değil, İş Akışı Çıkar:** "Python yazıyor" veya "n8n kullanıyor" gibi genel etiketler üretme. Bunun yerine *"Docker Compose + Coolify deployment öncesi güvenlik/env doğrulaması"* veya *"B2B müşteri görüşmesi notlarından teknik mimari teklif dokümanı üretimi"* gibi somut ve tekrarlanabilir süreçleri tespit et.
3. **Altyapı ve Tercih Uyumu:** Çıkaracağın skill'ler self-hosted, open-source, Docker/Coolify, n8n, Claude Code / MCP tabanlı geliştirme pratiklerime ve sade/production-ready mimari yaklaşımıma uyumlu olmalı. Kapalı kaynak SaaS bağımlılığı öneren skill'ler üretme.
4. **Eleştirel Filtre:** "Olsa iyi olur" seviyesindeki gereksiz soyutlamaları önerme. Gerçekten zaman kazandıracak, hata oranını düşürecek veya kalite standardını sabitleyecek maksimum **5 ila 7 adet** kritik skill belirle.

### Çalışma Adımları

#### Adım 1: Tekrarlayan Kalıpların (Patterns) Tespiti
Geçmişimi tarayarak şu 4 kategorideki tekrarları listele:
- **Tekrarlayan Üretim Süreçleri:** Sürekli ürettiğim içerik, kod, doküman veya teklif formatları.
- **Sık Tekrarlanan Hata ve Darboğazlar:** Sürekli düzelttiğim, kontrol ettiğim veya manuel müdahale ettiğim noktalar.
- **Araştırma ve Karar Alma Kalıpları:** Teknoloji, kütüphane veya firma değerlendirirken kullandığım sabit kriterler.
- **Mimari ve Deployment Rutinleri:** Sistem kurulumu, entegrasyon ve test aşamalarındaki standart adımlarım.

#### Adım 2: Skill Öneri Matrisi
Tespit ettiğin kalıplardan yola çıkarak önerdiğin her skill için şu tabloyu oluştur:
| Skill Adı (`kebab-case`) | Hangi Tekrarlayan İhtiyacı Çözer? | Tetikleyici (Trigger) Durum | Beklenen Çıktı / Deliverable | Tahmini Kullanım Sıklığı |

#### Adım 3: Seçilen Skill'ler İçin Taslak `SKILL.md` İskeleti
En yüksek öncelikli gördüğün ilk 3 skill için doğrudan kullanılabilir `SKILL.md` yapısını (YAML frontmatter `name` + `description`, adım adım execution kuralları, kaçınılacak anti-pattern'ler ve çıktı formatı) yaz.

### Girdi Verisi (Sohbet Geçmişi / Bağlam)
[BURAYA SOHBET GEÇMİŞİNİ, EXPORT DOSYASINI VEYA HAFIZA ÖZETİNİ YAPIŞTIR — Eğer bu oturumdaki sistem belleğine/geçmişine erişimin varsa doğrudan onu analiz ederek başla.]
