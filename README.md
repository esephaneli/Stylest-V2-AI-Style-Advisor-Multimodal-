# Stylest-V2-AI-Style-Advisor-Multimodal-
# 👗 Stylest V2 – AI Style Advisor

Stylest V2, **kullanıcı fotoğrafı + ürün fotoğrafını** birlikte analiz ederek  
kişiselleştirilmiş **stil uyumu, kombin önerisi ve karar desteği** sunan  
multimodal bir AI stil danışmanıdır.

Bu proje, AI ile **sadece cevap üretmekten ziyade**  
*karar veren, gerekçelendiren ve yapılandırılmış çıktı üreten*  
sistemlerin nasıl tasarlanabileceğini göstermeyi amaçlar.

---

## 🚀 Neler Yapıyor?

- 📸 Kullanıcı fotoğrafından **stil eğilimlerini** analiz eder  
- 🧥 Ürün fotoğrafından **kesim, mevsim ve kombinlenebilirlik** çıkarır  
- 🤖 LLM tabanlı karar motoru ile:
  - Ürün **uygun mu?**
  - **Neden uygun / neden değil?**
  - **Hangi kombinlerle daha iyi olur?**
- 🧠 Sonuçları **JSON formatında** üretir (dataset / pipeline uyumlu)
- 🎨 Opsiyonel **AI concept preview** üretir  
  > (Gerçek virtual try-on değildir, stil mockup amaçlıdır)

---

## ⚠️ Önemli Not (Etik & Teknik)

- Bu proje **virtual try-on değildir**
- Kullanıcı fotoğrafı:
  - ❌ Kimlik kopyalama için kullanılmaz
  - ✅ Stil analizi ve kişiselleştirme içindir
- Üretilen görseller **konsept amaçlıdır**, birebir giydirme yapmaz

---

## 🧩 Teknik Mimari

- Multimodal input (Image + Text)
- LLM tabanlı stil değerlendirme
- Pydantic ile **schema doğrulama**
- JSON-first çıktı tasarımı
- Gradio tabanlı **ürün benzeri UI**
- Feature-flag yaklaşımı 

---

## 🧠 JSON Output Neden Var?

JSON çıktılar:
- Dataset üretimi
- Pipeline entegrasyonu
- Analitik ve loglama
- Model değerlendirme

gibi senaryolar için tasarlanmıştır.

> UI tarafında JSON **geliştirici modu** kapalıyken gizlenir.

---

