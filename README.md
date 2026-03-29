# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

Jaya Jaya Maju merupakan perusahaan multinasional dengan lebih dari 1000 karyawan. Seiring pertumbuhan perusahaan, muncul tantangan dalam pengelolaan SDM, khususnya terkait tingginya tingkat attrition (karyawan keluar) yang telah melebihi 10%.

Tingginya attrition dapat berdampak pada:
- Biaya rekrutmen dan pelatihan meningkat
- Penurunan produktivitas
- Hilangnya talent berpengalaman
- Gangguan operasional bisnis

Oleh karena itu, perusahaan membutuhkan pendekatan berbasis data untuk:
- Mengidentifikasi faktor penyebab attrition
- Memonitor kondisi karyawan secara berkelanjutan
- Mendukung pengambilan keputusan strategis HR

### Permasalahan Bisnis

- Faktor apa saja yang paling mempengaruhi attrition karyawan?
- Departemen atau job role mana yang memiliki tingkat attrition tertinggi?

### Cakupan Proyek

1. Analisis Data
- Eksplorasi data karyawan (EDA)
- Identifikasi pola dan hubungan dengan attrition
- Analisis berdasarkan:
    1. Demografi (Age, Gender, MaritalStatus)
    2. Pekerjaan (Department, JobRole, JobLevel)
    3. Kepuasan kerja
    4. Gaji dan pengalaman kerja

2. Data Preprocessing
- Handling missing values
- Encoding fitur kategorikal
- Feature selection (menghapus kolom tidak relevan seperti EmployeeId, EmployeeCount, Over18, dan StandardHours)

3. Visualisasi & Dashboard
- Membuat dashboard interaktif (Looker Studio)
- Menampilkan Attrition rate, Distribusi attrition, dan Faktor-faktor penyebab

### Persiapan

Sumber data: https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee

Setup environment:

### 1️ Clone the Repository

```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
```

---

### 2️ Create a Virtual Environment (Recommended)

```bash
python -m venv venv
```

Activate the virtual environment:

**Windows:**
```bash
venv\Scripts\activate
```

**Mac/Linux:**
```bash
source venv/bin/activate
```

---
### 3️ Install Dependencies

Make sure the `requirements.txt` file is available, then run:

```bash
pip install -r requirements.txt
```

---
### 4 Buat File requirements.txt
```bash
pip freeze > requirements.txt
```

## Business Dashboard

Business dashboard yang dibuat bertujuan untuk membantu tim HR di perusahaan Jaya Jaya Maju dalam memonitor dan menganalisis tingkat attrition karyawan secara interaktif dan berbasis data. Dashboard ini dirancang menggunakan Looker Studio sehingga dapat diakses dengan mudah, real-time, dan mendukung eksplorasi data oleh pengguna non-teknis.

🧩 Komponen Dashboard
- Attrition rate sebesar 16,92% tergolong cukup tinggi (>10%), sehingga perlu perhatian khusus dari HR.
- Karyawan laki-laki memiliki jumlah attrition lebih tinggi dibanding perempuan, dan MaritalStatus tidak mempengaruhi faktor attrition
- Departemen dengan attrition tertinggi adalah Research & Development (~59.8%) dan diikuti oleh Sales (~36.9%). Departemen teknis dan sales berkemungkinan memiliki tekanan kerja lebih tinggi yang berpotensi turnover lebih besar
- Attrition paling banyak terjadi pada karyawan berusia sekitar 25–35 tahun. Selain itu, pada usia 18–21 tahun, jumlah karyawan yang keluar lebih banyak dibandingkan yang tetap bekerja. Hal ini menunjukkan bahwa karyawan yang lebih muda cenderung lebih sering berpindah kerja karena mencari peluang karier yang lebih baik.
- Job role dengan attrition tinggi dimulai Laboratory Technician, Sales Executive, dan Research Scientist. Posisi operasional & teknis memiliki risiko attrition lebih tinggi dan job level rendah (level 1–2) lebih rentan keluar
- Jarak rumah karyawan tidak berpotensi attrition meningkat, memungkinkan karyawan sedang WFH atau transportasi sudah disediakan perusahaan

🌐 Akses Dashboard
https://lookerstudio.google.com/reporting/87da55b1-89e4-4a2a-963f-bb9aefeaff99

## Conclusion

Berdasarkan hasil analisis yang telah dilakukan, dapat disimpulkan bahwa tingkat attrition di perusahaan Jaya Jaya Maju yang mencapai 16,92% tergolong cukup tinggi dan memerlukan perhatian serius dari pihak HR. Faktor utama yang mempengaruhi attrition tidak hanya berasal dari satu aspek, melainkan kombinasi dari karakteristik karyawan dan kondisi pekerjaan. Karyawan dengan usia muda (25–35 tahun), terutama pada tahap awal karier, cenderung memiliki tingkat attrition lebih tinggi karena dorongan untuk mencari peluang yang lebih baik. Selain itu, posisi pekerjaan seperti Laboratory Technician, Sales Executive, dan Research Scientist, serta karyawan pada job level rendah (level 1–2), menunjukkan kecenderungan lebih besar untuk keluar dari perusahaan. Dari sisi organisasi, departemen Research & Development dan Sales memiliki tingkat attrition tertinggi, yang mengindikasikan adanya tekanan kerja atau tuntutan pekerjaan yang lebih tinggi dibandingkan departemen lain.

Di sisi lain, faktor seperti gender menunjukkan adanya perbedaan jumlah attrition (lebih tinggi pada laki-laki), namun tidak serta merta menjadi faktor utama penentu. Variabel seperti Marital Status dan Distance from Home tidak menunjukkan pengaruh signifikan terhadap attrition, yang mengindikasikan bahwa faktor-faktor tersebut bukan prioritas utama dalam strategi retensi karyawan. Secara keseluruhan, hasil proyek ini menegaskan bahwa pendekatan berbasis data mampu mengidentifikasi faktor-faktor kunci penyebab attrition dan memberikan insight yang dapat digunakan oleh HR untuk merancang strategi retensi yang lebih efektif, seperti peningkatan kesejahteraan karyawan, pengelolaan beban kerja, serta pengembangan karier khususnya bagi karyawan pada tahap awal. Dashboard yang dibangun juga berperan penting sebagai alat monitoring berkelanjutan untuk mendukung pengambilan keputusan yang lebih cepat dan tepat.

### Rekomendasi Action Items (Optional)

Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.

- Fokus Retensi pada Karyawan Usia Muda (25–35 tahun)
Perusahaan disarankan untuk membuat program retensi khusus bagi karyawan usia muda yang berada pada tahap awal karier. Hal ini dapat dilakukan melalui penyediaan jalur karier yang jelas (career path), program mentoring, serta pelatihan dan pengembangan kompetensi. Karyawan pada rentang usia ini cenderung memiliki motivasi tinggi untuk berkembang, sehingga jika perusahaan mampu memfasilitasi kebutuhan tersebut, potensi mereka untuk bertahan akan meningkat.
- Evaluasi Beban Kerja pada Departemen R&D dan Sales
Departemen Research & Development serta Sales memiliki tingkat attrition tertinggi, yang mengindikasikan adanya tekanan kerja yang lebih besar. Oleh karena itu, perusahaan perlu melakukan evaluasi terhadap beban kerja, target, serta sistem kerja di kedua departemen tersebut. Penyesuaian target yang lebih realistis, penambahan sumber daya, atau penerapan sistem kerja yang lebih fleksibel dapat membantu mengurangi tingkat kelelahan (burnout) karyawan.
- Penguatan Program untuk Job Role Berisiko Tinggi
Posisi seperti Laboratory Technician, Sales Executive, dan Research Scientist perlu mendapatkan perhatian khusus karena memiliki tingkat attrition yang tinggi. Perusahaan dapat memberikan insentif tambahan, penghargaan berbasis kinerja, serta peluang pengembangan karier yang lebih jelas untuk meningkatkan loyalitas karyawan pada posisi tersebut.
- Pengembangan Program untuk Karyawan Job Level Rendah
Karyawan pada level awal (level 1–2) memiliki kecenderungan lebih tinggi untuk keluar. Oleh karena itu, penting bagi perusahaan untuk menyediakan program onboarding yang lebih baik, pelatihan dasar, serta kesempatan promosi yang transparan. Dengan adanya kejelasan jenjang karier, karyawan akan lebih termotivasi untuk bertahan dan berkembang di dalam perusahaan.
- Optimalisasi Work-Life Balance
Meskipun tidak semua faktor dianalisis secara langsung, tekanan kerja yang tinggi berpotensi mempengaruhi kepuasan karyawan. Perusahaan dapat mempertimbangkan kebijakan seperti fleksibilitas jam kerja, sistem kerja hybrid (WFH), serta pengelolaan lembur yang lebih baik untuk meningkatkan keseimbangan antara pekerjaan dan kehidupan pribadi karyawan.