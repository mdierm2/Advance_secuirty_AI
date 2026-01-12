# Ketahanan Infrastruktur Digital di Tengah Kompleksitas Layanan Perbankan

*(Catatan Risiko Infrastruktur & Cyber Resilience – Internal Board)*

Sepanjang **tahun 2025**, Bank BNI mengelola ekosistem teknologi informasi dengan skala dan kompleksitas yang terus meningkat, mencakup **263 aplikasi aktif** yang menopang operasional perbankan secara menyeluruh. Dari jumlah tersebut, **72 aplikasi dikategorikan sebagai aplikasi kritikal**, karena berkaitan langsung dengan transaksi nasabah, sistem inti perbankan, dan keberlangsungan layanan bisnis BNI.

Untuk mendukung kebutuhan tersebut, Bank BNI mengoperasikan **dua data center aktif dan satu disaster recovery center** sebagai fondasi infrastruktur digital. Arsitektur ini dirancang untuk menjaga ketersediaan layanan serta memitigasi risiko apabila salah satu data center mengalami gangguan operasional.

Namun demikian, realitas operasional sepanjang tahun 2025 menunjukkan bahwa **ketahanan layanan digital tidak semata-mata ditentukan oleh keberadaan infrastruktur cadangan**. Fakta operasional mencatat bahwa **sembilan (9) kejadian gangguan aplikasi berskala signifikan terjadi sepanjang tahun 2025**, yang terutama berdampak pada aspek **ketersediaan layanan (availability)**, tanpa indikasi pelanggaran terhadap **kerahasiaan (confidentiality)** maupun **integritas (integrity)** data.

---

## Prinsip Arsitektur Aktif–Aktif dan Kesenjangan Implementasi

Secara prinsip, arsitektur **data center aktif–aktif** dirancang untuk memberikan **ketersediaan layanan yang tinggi dan ketahanan operasional**, dengan memastikan bahwa **masing-masing data center memiliki kapabilitas yang setara** dan mampu **saling mengambil alih seluruh beban layanan secara penuh** apabila terjadi gangguan pada salah satu data center.

Namun, berdasarkan evaluasi kondisi terkini, implementasi arsitektur aktif–aktif yang berjalan **belum sepenuhnya memenuhi prinsip dasar tersebut**. Dua data center yang saat ini beroperasi secara aktif **belum memiliki kapabilitas untuk mengakomodasi 100% trafik secara mandiri**, serta menerapkan **pembagian beban layanan yang tidak seimbang**.

Dalam kondisi operasional normal, skema ini masih dapat mendukung kebutuhan layanan. Akan tetapi, **dalam skenario gangguan pada salah satu data center atau lonjakan beban signifikan**, keterbatasan kapasitas pada data center lainnya **meningkatkan risiko terhadap keberlangsungan layanan**, khususnya pada layanan yang bersifat kritikal.

> **Pembagian beban layanan antar dua data center saat ini belum dirancang untuk memungkinkan salah satu data center menopang keseluruhan layanan kritikal secara berkelanjutan.**
> Dalam skenario gangguan atau lonjakan beban signifikan, kondisi eksisting menunjukkan bahwa **data center yang tersisa belum dirancang untuk mengambil alih seluruh beban layanan secara penuh**, sehingga berpotensi menimbulkan degradasi performa maupun gangguan layanan.

Kondisi tersebut **belum sepenuhnya selaras dengan praktik terbaik industri perbankan digital**, di mana arsitektur dua data center aktif diarahkan agar **setiap data center memiliki kapabilitas operasional penuh** sebagai bagian dari penguatan ketahanan layanan dan mitigasi risiko operasional.

---

## Perencanaan Kapasitas dan Pertumbuhan Beban Layanan

Selain aspek kapasitas fisik, evaluasi juga menunjukkan bahwa perencanaan infrastruktur belum sepenuhnya didukung oleh pendekatan capacity planning berbasis trafik aktual. Perhitungan kebutuhan kapasitas, baik berdasarkan volume transaksi aktual maupun skenario lonjakan beban, belum tersedia secara konsisten sebagai baseline perencanaan.

Ketiadaan baseline kapasitas yang terukur ini meningkatkan risiko terjadinya kelebihan beban sumber daya tanpa terdeteksi sejak dini, sehingga memperbesar potensi gangguan layanan ketika terjadi perubahan kondisi operasional.

---

## Monitoring dan Pengendalian Dini

Dari sisi pengendalian operasional, saat ini **belum tersedia mekanisme peringatan dini (Early Warning System) yang terstandarisasi** untuk memberikan sinyal ketika utilisasi kapasitas infrastruktur mendekati ambang batas kritis.

Kondisi ini **berpotensi membatasi waktu respons organisasi** dalam melakukan langkah mitigasi atau penyesuaian kapasitas secara proaktif sebelum gangguan layanan terjadi.

---

## Kompleksitas Arsitektur dan Ketergantungan Sistem

Kompleksitas infrastruktur tidak hanya tercermin dari kapasitas fisik, tetapi juga dari **ketergantungan antar sistem dan platform pendukung layanan digital**. Pengelolaan middleware, integrasi aplikasi, serta konfigurasi lintas data center menambah lapisan risiko yang meningkatkan sensitivitas sistem terhadap **kegagalan parsial dan perubahan kondisi operasional**.

Dari perspektif **IT risk**, temuan ini menegaskan bahwa tantangan utama Bank saat ini **tidak berada pada aspek serangan siber yang berorientasi pada pelanggaran data**, melainkan pada **ketahanan layanan digital (cyber resilience)**, khususnya dalam domain *availability*.

---

## Arah Penguatan Arsitektur Aktif–Aktif

Sebagai pembelajaran strategis dari kejadian sepanjang tahun 2025, penguatan arsitektur aktif–aktif diarahkan pada:

* **Penyelarasan kapasitas antar data center** agar masing-masing memiliki kapabilitas operasional yang memadai.
* **Penguatan perencanaan kapasitas berbasis trafik aktual**, termasuk skenario lonjakan beban.
* **Penerapan mekanisme monitoring dan peringatan dini yang lebih proaktif** untuk mendukung respons yang tepat waktu.

Langkah-langkah tersebut diharapkan dapat memastikan bahwa arsitektur aktif–aktif **tidak hanya berjalan secara operasional**, tetapi juga memberikan **ketahanan layanan yang memadai** terhadap skenario gangguan dan peningkatan pertumbuhan bisnis di era digital, 
