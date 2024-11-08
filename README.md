

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
