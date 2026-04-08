# Contributing Guide

Bu proje, rastgele not toplama yerine **mühendislik kalitesinde dokümantasyon** üretmeyi hedefler. Katkı verirken aşağıdaki çerçeveyi izleyin.

## 1) Katkı Prensipleri

- İçerik teknik olarak doğru, ölçülebilir ve uygulanabilir olmalıdır.
- Kavram anlatımı ile operasyonel uygulama dengeli olmalıdır.
- Üretim ortamında yanlış yönlendirme riski taşıyan ifadelerden kaçınılmalıdır.
- Belirsiz genellemeler yerine bağlam verilmelidir (hangi ölçek, hangi sistem, hangi risk?).

## 2) Doküman Şablonu (Önerilen)

Her yeni teknik dokümanda mümkünse şu bölümler bulunsun:

1. **Problem tanımı**
2. **Kapsam / Kapsam dışı**
3. **Temel kavramlar**
4. **Mimari yaklaşım**
5. **Trade-off analizi**
6. **Operasyonel checklist**
7. **Sık yapılan hatalar (anti-patterns)**
8. **Kaynaklar**

## 3) Yazım Kuralları

- Markdown başlık hiyerarşisi bozulmamalıdır (`#`, `##`, `###`).
- Madde işaretleri mümkün olduğunca kısa ve eylem odaklı olmalıdır.
- Terimler tutarlı kullanılmalıdır (ör. “availability”, “reliability”).
- Türkçe anlatım tercih edilir; yaygın teknik terimler İngilizce bırakılabilir.
- Kopya içerik eklenmemelidir; kaynaklardan öğrenilip özgün ifade ile yazılmalıdır.

## 4) Kalite Kontrol Listesi (PR öncesi)

- [ ] Başlık yapısı tutarlı mı?
- [ ] Kırık bağlantı var mı?
- [ ] “Neden” ve “nasıl” birlikte anlatılıyor mu?
- [ ] En az bir gerçek kullanım senaryosu verildi mi?
- [ ] Operasyonel riskler belirtildi mi?

## 5) İnceleme Standardı (Reviewer için)

Reviewer aşağıdakileri doğrulamalıdır:

- Teknik doğruluk ve terminoloji kalitesi
- İçeriğin üretim gerçekliği (pratik uygulanabilirlik)
- Yanlış güven yaratabilecek ifadelerin temizliği
- Benzer dokümanlarla tekrar/çakışma kontrolü

## 6) Commit ve PR Notları

- Commit mesajları kısa, açıklayıcı ve tek amaca odaklı olmalıdır.
- Büyük değişikliklerde “neden bu değişim yapıldı?” sorusu PR açıklamasında cevaplanmalıdır.
- Eğer davranışsal/operasyonel bir değişim varsa, runbook etkisi mutlaka belirtilmelidir.
