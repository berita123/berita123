.
<html lang="id">
<!-- [Header dan Style CSS sebelumnya tetap sama] -->

<style>
    /* [Style CSS sebelumnya tetap sama] */
    
    /* Tambahan style untuk berita */
    .news-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 20px;
        margin: 30px 0;
    }
    .news-card {
        background: white;
        border-radius: 8px;
        overflow: hidden;
        box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        transition: transform 0.3s ease;
    }
    .news-card:hover {
        transform: translateY(-5px);
    }
    .news-image {
        width: 100%;
        height: 200px;
        background-color: #e0e0e0;
        display: flex;
        align-items: center;
        justify-content: center;
        color: #666;
    }
    .news-content {
        padding: 20px;
    }
    .news-date {
        color: #666;
        font-size: 0.9em;
    }
    .tag {
        display: inline-block;
        padding: 3px 8px;
        background-color: #1a237e;
        color: white;
        border-radius: 3px;
        font-size: 0.8em;
        margin-right: 5px;
    }
    .breaking-news {
        background: linear-gradient(45deg, #ff4081, #ff6e40);
        color: white;
        padding: 15px;
        margin: 20px 0;
        border-radius: 8px;
        animation: pulse 2s infinite;
    }
    @keyframes pulse {
        0% { box-shadow: 0 0 0 0 rgba(255, 64, 129, 0.4); }
        70% { box-shadow: 0 0 0 10px rgba(255, 64, 129, 0); }
        100% { box-shadow: 0 0 0 0 rgba(255, 64, 129, 0); }
    }
    .related-news {
        background: #f5f5f5;
        padding: 20px;
        border-radius: 8px;
        margin-top: 30px;
    }
    .news-list {
        list-style: none;
        padding: 0;
    }
    .news-list li {
        padding: 10px 0;
        border-bottom: 1px solid #ddd;
    }
</style>

<body>
    <div class="container">
        <!-- [Konten sebelumnya tetap sama sampai sebelum footer] -->

        <!-- Tambahan Section Berita Terbaru -->
        <section class="content-section">
            <h2>Berita Terkini</h2>

            <div class="breaking-news">
                <h3>🔴 Breaking News!</h3>
                <p>Aqua Meluncurkan Program "Peduli Air Bersih" di Desa Limau Manis dengan Investasi 5 Miliar Rupiah</p>
                <small>2 jam yang lalu</small>
            </div>

            <div class="news-grid">
                <article class="news-card">
                    <div class="news-image">Inovasi Produk</div>
                    <div class="news-content">
                        <span class="tag">Produk Baru</span>
                        <span class="tag">Inovasi</span>
                        <h3>Aqua Perkenalkan Kemasan Ramah Lingkungan di Limau Manis</h3>
                        <p class="news-date">5 November 2024</p>
                        <p>Program baru ini menggunakan bahan daur ulang 100% untuk kemasan produk...</p>
                    </div>
                </article>

                <article class="news-card">
                    <div class="news-image">CSR Program</div>
                    <div class="news-content">
                        <span class="tag">Komunitas</span>
                        <span class="tag">CSR</span>
                        <h3>Program Pemberdayaan UMKM Desa Limau Manis</h3>
                        <p class="news-date">3 November 2024</p>
                        <p>Kerjasama dengan pelaku UMKM lokal untuk meningkatkan distribusi produk...</p>
                    </div>
                </article>

                <article class="news-card">
                    <div class="news-image">Market Update</div>
                    <div class="news-content">
                        <span class="tag">Bisnis</span>
                        <span class="tag">Pasar</span>
                        <h3>Analisis Pasar: Tren Konsumsi Air Mineral 2024</h3>
                        <p class="news-date">1 November 2024</p>
                        <p>Studi terbaru menunjukkan perubahan pola konsumsi masyarakat...</p>
                    </div>
                </article>
            </div>

            <div class="related-news">
                <h3>Berita Terkait</h3>
                <ul class="news-list">
                    <li>
                        <strong>Ekonomi:</strong> Pertumbuhan Ekonomi Desa Limau Manis Meningkat 15% 
                        <span class="news-date">31 Oktober 2024</span>
                    </li>
                    <li>
                        <strong>Teknologi:</strong> Implementasi Sistem Digital untuk Tracking Distribusi
                        <span class="news-date">29 Oktober 2024</span>
                    </li>
                    <li>
                        <strong>Sosial:</strong> Program Beasiswa untuk Siswa Berprestasi di Limau Manis
                        <span class="news-date">27 Oktober 2024</span>
                    </li>
                    <li>
                        <strong>Lingkungan:</strong> Inisiatif Penghijauan di Sekitar Pabrik
                        <span class="news-date">25 Oktober 2024</span>
                    </li>
                </ul>
            </div>

            <div class="highlight-box">
                <h3>Agenda Mendatang</h3>
                <ul>
                    <li>15 November 2024 - Pembukaan Pusat Pelatihan UMKM</li>
                    <li>20 November 2024 - Festival Air Bersih Limau Manis</li>
                    <li>25 November 2024 - Seminar Ekonomi Kreatif</li>
                    <li>1 Desember 2024 - Peluncuran Program Daur Ulang Kemasan</li>
                </ul>
            </div>
        </section>

        <!-- Tambahan Section Update Sosial Media -->
        <section class="content-section">
            <h2>Media Sosial Update</h2>
            <div class="news-grid">
                <div class="news-card">
                    <div class="news-content">
                        <span class="tag">Instagram</span>
                        <h3>📸 Dokumentasi Kegiatan CSR</h3>
                        <p>Kunjungi Instagram kami untuk melihat kegiatan terbaru di Desa Limau Manis #AquaPeduli</p>
                    </div>
                </div>

                <div class="news-card">
                    <div class="news-content">
                        <span class="tag">Twitter</span>
                        <h3>🐦 Trending Topic</h3>
                        <p>#AquaLimauManis menjadi trending topic regional dengan 10k+ tweets</p>
                    </div>
                </div>

                <div class="news-card">
                    <div class="news-content">
                        <span class="tag">YouTube</span>
                        <h3>🎥 Video Dokumenter</h3>
                        <p>Tonton dokumenter terbaru tentang perjalanan Aqua di Desa Limau Manis</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- [Footer tetap sama] -->
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portal Analisis & Berita Aqua Desa Limau Manis</title>
    <style>
        /* Style dasar */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header dan Navigasi */
        .header {
            text-align: center;
            padding: 40px 0;
            background: linear-gradient(135deg, #1a237e, #303f9f);
            color: white;
            margin-bottom: 30px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            border-radius: 10px;
            position: relative;
            overflow: hidden;
        }
        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, rgba(255,255,255,0.1) 25%, transparent 25%),
                        linear-gradient(-45deg, rgba(255,255,255,0.1) 25%, transparent 25%);
            background-size: 60px 60px;
            animation: moveBackground 20s linear infinite;
        }
        @keyframes moveBackground {
            0% { background-position: 0 0; }
            100% { background-position: 60px 60px; }
        }
        .header h1, .header h2, .header p {
            position: relative;
            z-index: 1;
        }
        .navigation {
            background-color: #1a237e;
            padding: 15px 0;
            margin-bottom: 30px;
            border-radius: 5px;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        .navigation ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        .navigation ul li {
            margin: 0 15px;
        }
        .navigation ul li a {
            color: white;
            text-decoration: none;
            padding: 5px 10px;
            transition: all 0.3s ease;
        }
        .navigation ul li a:hover {
            background-color: #303f9f;
            border-radius: 3px;
            transform: translateY(-2px);
        }

        /* Konten Sections */
        .content-section {
            background-color: white;
            padding: 30px;
            margin-bottom: 30px;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }
        .content-section:hover {
            transform: translateY(-5px);
        }

        /* Charts dan Visualisasi */
        .chart {
            margin: 40px 0;
            text-align: center;
        }
        .bar-chart {
            display: flex;
            justify-content: center;
            align-items: flex-end;
            height: 400px;
            gap: 40px;
            padding: 20px;
            background-color: #f8f9fa;
            border-radius: 10px;
            position: relative;
        }
        .bar-chart::before {
            content: '';
            position: absolute;
            left: 40px;
            right: 40px;
            bottom: 0;
            height: 2px;
            background-color: #1a237e;
        }
        .bar {
            width: 100px;
            background: linear-gradient(to top, #1a237e, #303f9f);
            display: flex;
            flex-direction: column;
            align-items: center;
            color: white;
            transition: all 0.3s ease;
            border-radius: 5px 5px 0 0;
            position: relative;
            cursor: pointer;
        }
        .bar:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        /* Berita Styles */
        .news-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        .news-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            position: relative;
        }
        .news-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        .news-image {
            width: 100%;
            height: 200px;
            background: linear-gradient(45deg, #1a237e, #303f9f);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2em;
            position: relative;
            overflow: hidden;
        }
        .news-image::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, rgba(255,255,255,0.1), transparent);
        }
        .news-content {
            padding: 20px;
        }
        .news-date {
            color: #666;
            font-size: 0.9em;
            margin-top: 10px;
        }
        .tag {
            display: inline-block;
            padding: 3px 8px;
            background-color: #1a237e;
            color: white;
            border-radius: 3px;
            font-size: 0.8em;
            margin-right: 5px;
            margin-bottom: 5px;
            transition: all 0.3s ease;
        }
        .tag:hover {
            background-color: #303f9f;
            transform: translateY(-2px);
        }

        /* Breaking News Animation */
        .breaking-news {
            background: linear-gradient(45deg, #ff4081, #ff6e40);
            color: white;
            padding: 20px;
            margin: 20px 0;
            border-radius: 8px;
            position: relative;
            overflow: hidden;
            animation: pulse 2s infinite;
        }
        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(255, 64, 129, 0.4); }
            70% { box-shadow: 0 0 0 10px rgba(255, 64, 129, 0); }
            100% { box-shadow: 0 0 0 0 rgba(255, 64, 129, 0); }
        }

        /* Tabel Data */
        .data-table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background: white;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            border-radius: 8px;
            overflow: hidden;
        }
        .data-table th, .data-table td {
            padding: 15px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        .data-table th {
            background-color: #1a237e;
            color: white;
        }
        .data-table tr:hover {
            background-color: #f5f5f5;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .navigation ul {
                flex-direction: column;
                align-items: center;
            }
            .navigation ul li {
                margin: 5px 0;
            }
            .bar-chart {
                height: 300px;
                gap: 20px;
            }
            .bar {
                width: 60px;
            }
            .news-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 30px;
            background: linear-gradient(135deg, #1a237e, #303f9f);
            color: white;
            border-radius: 10px;
            margin-top: 30px;
            position: relative;
            overflow: hidden;
        }
        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, rgba(255,255,255,0.1) 25%, transparent 25%);
            background-size: 30px 30px;
            animation: moveBackground 15s linear infinite;
        }
        footer p {
            position: relative;
            z-index: 1;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Section -->
        <div class="header">
            <h1>Portal Analisis & Berita Aqua</h1>
            <h2>Desa Limau Manis 2021-2024</h2>
            <p>Pusat Informasi dan Analisis Terpadu</p>
        </div>

        <!-- Navigation -->
        <nav class="navigation">
            <ul>
                <li><a href="#ringkasan">Ringkasan</a></li>
                <li><a href="#data">Data</a></li>
                <li><a href="#analisis">Analisis</a></li>
                <li><a href="#berita">Berita</a></li>
                <li><a href="#media">Media</a></li>
            </ul>
        </nav>

        <!-- Breaking News -->
        <div class="breaking-news">
            <h3>🔴 BREAKING NEWS</h3>
            <p>Aqua Meluncurkan Program "Peduli Air Bersih" di Desa Limau Manis dengan Investasi 5 Miliar Rupiah</p>
            <small>Baru saja</small>
        </div>

        <!-- Main Content -->
        <section id="ringkasan" class="content-section">
            <h2>Ringkasan Eksekutif</h2>
            <p>Analisis komprehensif perkembangan dan distribusi Aqua di Desa Limau Manis menunjukkan pertumbuhan yang signifikan...</p>
            
            <!-- Highlight Box -->
            <div class="highlight-box">
                <h3>Pencapaian Utama 2024:</h3>
                <ul>
                    <li>Peningkatan penjualan 25% dari tahun sebelumnya</li>
                    <li>Pembukaan 10 titik distribusi baru</li>
                    <li>Peluncuran program sustainability</li>
                </ul>
            </div>
        </section>

        <!-- Data Visualization -->
        <section id="data" class="content-section">
            <h2>Visualisasi Data</h2>
            <div class="chart">
                <div class="bar-chart">
                    <!-- Bars will be added here -->
                </div>
            </div>
            
            <!-- Data Table -->
            <table class="data-table">
                <!-- Table content -->
            </table>
        </section>

        <!-- News Section -->
        <section id="berita" class="content-section">
            <h2>Berita Terkini</h2>
            <div class="news-grid">
                <!-- News cards will be added here -->
            </div>
        </section>

        <!-- Social Media Updates -->
        <section id="media" class="content-section">
            <h2>Media Sosial Update</h2>
            <div class="news-grid">
                <!-- Social media updates will be added here -->
            </div>
        </section>

        <!-- Footer -->
        <footer>
            <p>Portal Analisis & Berita Aqua Desa Limau Manis</p>
            <p>© 2024 All Rights Reserved</p>
        </footer>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Analisis Komprehensif Penjualan Aqua Desa Limau Manis</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .header {
            text-align: center;
            padding: 40px 0;
            background-color: #ffffff;
            margin-bottom: 30px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            border-radius: 10px;
        }
        .header h1 {
            color: #1a237e;
            margin-bottom: 10px;
        }
        .navigation {
            background-color: #1a237e;
            padding: 15px 0;
            margin-bottom: 30px;
            border-radius: 5px;
        }
        .navigation ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
        }
        .navigation ul li {
            margin: 0 15px;
        }
        .navigation ul li a {
            color: white;
            text-decoration: none;
            padding: 5px 10px;
        }
        .navigation ul li a:hover {
            background-color: #303f9f;
            border-radius: 3px;
        }
        .content-section {
            background-color: white;
            padding: 30px;
            margin-bottom: 30px;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .chart {
            margin: 40px 0;
            text-align: center;
        }
        .bar-chart {
            display: flex;
            justify-content: center;
            align-items: flex-end;
            height: 400px;
            gap: 40px;
            padding: 20px;
            background-color: #f8f9fa;
            border-radius: 10px;
        }
        .bar {
            width: 100px;
            background: linear-gradient(to top, #1a237e, #303f9f);
            display: flex;
            flex-direction: column;
            align-items: center;
            color: white;
            transition: all 0.3s ease;
            border-radius: 5px 5px 0 0;
            position: relative;
        }
        .bar:hover {
            transform: scale(1.05);
        }
        .bar-value {
            margin-top: -25px;
            color: #1a237e;
            font-weight: bold;
        }
        .bar-label {
            margin-top: 10px;
            color: #1a237e;
            font-weight: bold;
        }
        .analysis {
            background-color: #f8f9fa;
            padding: 25px;
            border-radius: 8px;
            margin-top: 30px;
            border-left: 5px solid #1a237e;
        }
        .highlight-box {
            background-color: #e3f2fd;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
        }
        .data-table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        .data-table th, .data-table td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        .data-table th {
            background-color: #1a237e;
            color: white;
        }
        .data-table tr:nth-child(even) {
            background-color: #f8f9fa;
        }
        .recommendations {
            background-color: #e8eaf6;
            padding: 20px;
            border-radius: 8px;
            margin-top: 30px;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #1a237e;
            color: white;
            border-radius: 10px;
            margin-top: 30px;
        }
        @media (max-width: 768px) {
            .bar-chart {
                height: 300px;
                gap: 20px;
            }
            .bar {
                width: 60px;
            }
            .navigation ul {
                flex-direction: column;
                align-items: center;
            }
            .navigation ul li {
                margin: 5px 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Analisis Komprehensif Penjualan Produk Aqua</h1>
            <h2>Desa Limau Manis 2021-2023</h2>
            <p>Laporan Lengkap dan Analisis Trend Penjualan</p>
        </div>

        <nav class="navigation">
            <ul>
                <li><a href="#ringkasan">Ringkasan Eksekutif</a></li>
                <li><a href="#data">Data Penjualan</a></li>
                <li><a href="#analisis">Analisis</a></li>
                <li><a href="#rekomendasi">Rekomendasi</a></li>
            </ul>
        </nav>

        <article>
            <section id="ringkasan" class="content-section">
                <h2>Ringkasan Eksekutif</h2>
                <p>Laporan ini menyajikan analisis komprehensif tentang penjualan produk Aqua di Desa Limau Manis selama periode 2021-2023. Data menunjukkan fluktuasi yang signifikan dengan tren yang menarik untuk dikaji lebih dalam.</p>
                
                <div class="highlight-box">
                    <h3>Poin-poin Utama:</h3>
                    <ul>
                        <li>Puncak penjualan tercapai pada tahun 2022</li>
                        <li>Terjadi penurunan signifikan di tahun 2023</li>
                        <li>Rata-rata penjualan 18.000 unit per tahun</li>
                    </ul>
                </div>
            </section>

            <section id="data" class="content-section">
                <h2>Data Penjualan Tahunan</h2>
                
                <div class="chart">
                    <div class="bar-chart">
                        <div class="bar" style="height: 280px;">
                            <div class="bar-value">18000</div>
                            <div class="bar-label">2021</div>
                        </div>
                        <div class="bar" style="height: 295px;">
                            <div class="bar-value">19000</div>
                            <div class="bar-label">2022</div>
                        </div>
                        <div class="bar" style="height: 265px;">
                            <div class="bar-value">17000</div>
                            <div class="bar-label">2023</div>
                        </div>
                    </div>
                </div>

                <table class="data-table">
                    <thead>
                        <tr>
                            <th>Tahun</th>
                            <th>Volume Penjualan</th>
                            <th>Persentase Perubahan</th>
                            <th>Keterangan</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>2021</td>
                            <td>18.000 unit</td>
                            <td>-</td>
                            <td>Tahun dasar</td>
                        </tr>
                        <tr>
                            <td>2022</td>
                            <td>19.000 unit</td>
                            <td>+5.5%</td>
                            <td>Puncak penjualan</td>
                        </tr>
                        <tr>
                            <td>2023</td>
                            <td>17.000 unit</td>
                            <td>-10.5%</td>
                            <td>Penurunan signifikan</td>
                        </tr>
                    </tbody>
                </table>
            </section>

            <section id="analisis" class="content-section">
                <h2>Analisis Mendalam</h2>
                
                <div class="analysis">
                    <h3>Faktor-faktor yang Mempengaruhi Penjualan:</h3>
                    <h4>1. Faktor Internal</h4>
                    <ul>
                        <li>Strategi distribusi dan pemasaran</li>
                        <li>Manajemen stok dan inventori</li>
                        <li>Hubungan dengan reseller dan distributor</li>
                        <li>Program promosi dan diskon</li>
                    </ul>

                    <h4>2. Faktor Eksternal</h4>
                    <ul>
                        <li>Perubahan perilaku konsumen</li>
                        <li>Kondisi ekonomi makro</li>
                        <li>Persaingan pasar</li>
                        <li>Faktor cuaca dan musim</li>
                    </ul>
                </div>

                <div class="highlight-box">
                    <h3>Temuan Utama:</h3>
                    <ol>
                        <li>Terjadi peningkatan signifikan pada tahun 2022 karena strategi pemasaran yang efektif</li>
                        <li>Penurunan tahun 2023 dipengaruhi oleh masuknya kompetitor baru</li>
                        <li>Pola konsumsi masyarakat berubah seiring dengan tren gaya hidup</li>
                    </ol>
                </div>
            </section>

            <section id="rekomendasi" class="content-section">
                <h2>Rekomendasi Strategis</h2>
                
                <div class="recommendations">
                    <h3>Langkah-langkah Perbaikan:</h3>
                    <ol>
                        <li>Pengembangan Program Loyalitas
                            <ul>
                                <li>Membuat sistem poin reward</li>
                                <li>Program membership khusus</li>
                                <li>Diskon berdasarkan volume pembelian</li>
                            </ul>
                        </li>
                        <li>Optimalisasi Distribusi
                            <ul>
                                <li>Pemetaan ulang jalur distribusi</li>
                                <li>Kerjasama dengan distributor baru</li>
                                <li>Penggunaan teknologi tracking pengiriman</li>
                            </ul>
                        </li>
                        <li>Strategi Pemasaran Digital
                            <ul>
                                <li>Pemanfaatan media sosial</li>
                                <li>Kampanye digital awareness</li>
                                <li>Kolaborasi dengan influencer lokal</li>
                            </ul>
                        </li>
                    </ol>
                </div>
            </section>
        </article>

        <footer>
            <p>Laporan Analisis Penjualan Aqua Desa Limau Manis</p>
            <p>Diperbarui: November 2024</p>
        </footer>
    </div>
</body>
</html>
