# OpenAPI Tasarımı Ödevi Teslim Raporu

## 👤 Öğrenci Bilgileri
- **Ad Soyad**: [Hilmi Özbay]
- **Öğrenci Numarası**: [170422050]

---

## 📂 OpenAPI YAML Dosyası

- **openapi.yaml** dosyasını projenizin GitHub reposuna yükleyiniz.
- Swagger Editor ile test ettiğinizden emin olunuz.

### 🔗 GitHub Repo Linki
(https://github.com/hilmiozbay/openapi-homework)

---

## 📝 API Açıklaması

Varlıklar (Entities)
	•	Book: Kitap bilgileri (başlık, yazar, ISBN, stok vb.)
	•	Student: Öğrenci bilgileri (ad, numara, e-posta, aktiflik durumu)
	•	Loan: Kitap ödünç alma işlemleri (tarih, durum, iade tarihi vb.)

CRUD İşlemleri ve Endpointler

Tüm varlıklar için aşağıdaki işlemler gerçekleştirilmiştir:
	•	GET /books, POST /books, GET /books/{id}, PUT /books/{id}, DELETE /books/{id}
	•	GET /students, POST /students, GET /students/{id}, PUT /students/{id}, DELETE /students/{id}
	•	GET /loans, POST /loans, GET /loans/{id}, PATCH /loans/{id} (iade işlemi)

components/schemas
	•	Her varlık için detaylı type, format, enum, nullable, description alanlarıyla veri şemaları tanımlanmıştır.

Parameters
	•	path parametreleri (örn. id) ve query parametreleri (page, size) tanımlanmıştır.
	•	Özellikle GET /books için sayfalama desteklenmektedir (page, size).

responses
	•	Başarılı (200, 201, 204) ve hatalı (400, 404) durumlar için açıklayıcı yanıtlar belirtilmiştir.


