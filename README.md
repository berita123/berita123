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
            gap: 80px;
            padding: 40px;
            background-color: #f8f9fa;
            border-radius: 10px;
            margin: 40px 0;
            position: relative;
        }
        .bar {
            width: 120px;
            background: linear-gradient(to top, #1a237e, #303f9f);
            display: flex;
            flex-direction: column;
            align-items: center;
            color: white;
            transition: all 0.3s ease;
            border-radius: 5px 5px 0 0;
            position: relative;
        }
        .bar span {
            color: #333;
            font-weight: bold;
        }
        .chart h3 {
            text-align: center;
            margin-bottom: 30px;
            color: #1a237e;
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
                gap: 40px;
                padding: 20px;
            }
            .bar {
                width: 80px;
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
                <h3>Data Penjualan Produk Aqua Desa Limau Manis</h3>
                <div class="bar-chart">
                    <div class="bar" style="height: 300px;">
                        <span style="position: absolute; bottom: -30px;">2021</span>
                        <span style="position: absolute; top: -25px;">18000</span>
                    </div>
                    <div class="bar" style="height: 316px;">
                        <span style="position: absolute; bottom: -30px;">2022</span>
                        <span style="position: absolute; top: -25px;">19000</span>
                    </div>
                    <div class="bar" style="height: 283px;">
                        <span style="position: absolute; bottom: -30px;">2023</span>
                        <span style="position: absolute; top: -25px;">17000</span>
                    </div>
                </div>
            </div>
            
            <!-- Data Table -->
            <table class="data-table">
                <thead>
                    <tr>
                        <th>Tahun</th>
                        <th>Jumlah Penjualan</th>
                        <th>Perubahan</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>2021</td>
                        <td>18,000 unit</td>
                        <td>Baseline</td>
                    </tr>
                    <tr>
                        <td>2022</td>
                        <td>19,000 unit</td>
                        <td>+5.56%</td>
                    </tr>
                    <tr>
                        <td>2023</td>
                        <td>17,000 unit</td>
                        <td>-10.53%</td>
                    </tr>
                </tbody>
            </table>

            <!-- Analisis Ringkas -->
            <div class="highlight-box" style="margin-top: 20px;">
                <h3>Analisis Trend Penjualan:</h3>
                <ul>
                    <li>Puncak penjualan tercatat pada tahun 2022 dengan 19,000 unit</li>
                    <li>Terjadi penurunan sebesar 10.53% pada tahun 2023</li>
                    <li>Rata-rata penjualan 3 tahun terakhir: 18,000 unit</li>
                </ul>
            </div>
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
