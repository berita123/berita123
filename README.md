<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Penjualan Aqua Desa Limau Manis</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
        }
        .header {
            text-align: center;
            padding: 20px 0;
            background-color: #f5f5f5;
            margin-bottom: 20px;
        }
        .chart {
            margin: 30px 0;
            text-align: center;
        }
        .bar-chart {
            display: flex;
            justify-content: center;
            align-items: flex-end;
            height: 300px;
            gap: 20px;
            padding: 20px;
        }
        .bar {
            width: 80px;
            background-color: #4a90e2;
            display: flex;
            flex-direction: column;
            align-items: center;
            color: white;
            transition: height 0.3s ease;
        }
        .bar-value {
            margin-top: -25px;
            color: black;
        }
        .bar-label {
            margin-top: 10px;
            color: black;
        }
        .analysis {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 5px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Data Penjualan Produk Aqua Desa Limau Manis</h1>
            <p>Analisis Trend Penjualan 2021-2023</p>
        </div>

        <article>
            <h2>Trend Penjualan Aqua Mengalami Fluktuasi</h2>
            
            <p>Berdasarkan data yang dihimpun dari Desa Limau Manis, penjualan produk Aqua menunjukkan pola yang menarik selama tiga tahun terakhir. Berikut adalah gambaran lengkap dari data penjualan tersebut.</p>

            <div class="chart">
                <div class="bar-chart">
                    <div class="bar" style="height: 240px;">
                        <div class="bar-value">18000</div>
                        <div class="bar-label">2021</div>
                    </div>
                    <div class="bar" style="height: 253px;">
                        <div class="bar-value">19000</div>
                        <div class="bar-label">2022</div>
                    </div>
                    <div class="bar" style="height: 227px;">
                        <div class="bar-value">17000</div>
                        <div class="bar-label">2023</div>
                    </div>
                </div>
            </div>

            <div class="analysis">
                <h3>Analisis Data:</h3>
                <ul>
                    <li>Tahun 2021: Penjualan mencapai 18.000 unit</li>
                    <li>Tahun 2022: Terjadi peningkatan menjadi 19.000 unit (kenaikan 5.5%)</li>
                    <li>Tahun 2023: Mengalami penurunan menjadi 17.000 unit (penurunan 10.5%)</li>
                </ul>
            </div>

            <h3>Faktor-faktor yang Mempengaruhi:</h3>
            <p>Beberapa faktor yang mempengaruhi fluktuasi penjualan antara lain:</p>
            <ul>
                <li>Perubahan pola konsumsi masyarakat</li>
                <li>Kondisi ekonomi lokal</li>
                <li>Persaingan dengan produk sejenis</li>
                <li>Strategi pemasaran yang diterapkan</li>
            </ul>

            <h3>Kesimpulan</h3>
            <p>Meski mengalami penurunan di tahun 2023, data historis menunjukkan bahwa penjualan Aqua di Desa Limau Manis tetap menunjukkan angka yang cukup stabil dengan rata-rata penjualan 18.000 unit per tahun. Diperlukan strategi baru untuk meningkatkan penjualan di tahun-tahun mendatang.</p>
        </article>
    </div>
</body>
</html>
