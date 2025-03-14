
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Page</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Section 1 - Menu */
        .nav-menu {
            background-color: #333;
            padding: 1rem;
        }
        
        .nav-menu ul {
            display: flex;
            justify-content: center;
            gap: 2rem;
            list-style: none;
        }
        
        .nav-menu a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
        }

        /* Section 2 - Judul dan Gambar */
        .section-2 {
            display: flex;
            align-items: center;
            padding: 3rem;
            gap: 2rem;
        }
        
        .judul {
            flex: 1;
        }
        
        .gambar {
            flex: 1;
        }
        
        .gambar img {
            max-width: 100%;
            height: auto;
        }

        /* Section 3 - Biodata */
        .section-3 {
            padding: 2rem;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 1rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .box {
            background-color: #f0f0f0;
            padding: 1.5rem;
            border-radius: 8px;
            text-align: center;
        }

        /* Section 4 - Portofolio */
        .section-4 {
            padding: 3rem;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1rem;
        }
        
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        
        th {
            background-color: #333;
            color: white;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .section-3 {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .section-2 {
                flex-direction: column;
            }
        }

        @media (max-width: 480px) {
            .section-3 {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Section 1 - Menu -->
    <nav class="nav-menu">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Section 2 - Judul dan Gambar -->
    <section class="section-2">
        <div class="judul">
            <h1>Portfolio Saya</h1>
            <p>Selamat datang di halaman portfolio saya</p>
        </div>
        <div class="gambar">
            <img src="profil.jpg" alt="Gambar Profil">
        </div>
    </section>

    <!-- Section 3 - Biodata -->
    <section class="section-3">
        <div class="box">Nama Lengkap</div>
        <div class="box">Tanggal Lahir</div>
        <div class="box">Pendidikan</div>
        <div class="box">Pengalaman</div>
        <div class="box">Skill</div>
        <div class="box">Kontak</div>
    </section>

    <!-- Section 4 - Portofolio -->
    <section class="section-4">
        <h2>Portfolio Projek</h2>
        <table>
            <thead>
                <tr>
                    <th>Nama Projek</th>
                    <th>Tahun</th>
                    <th>Deskripsi</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Website Perusahaan</td>
                    <td>2023</td>
                    <td>Pembuatan website perusahaan XYZ</td>
                </tr>
                <tr>
                    <td>Aplikasi Mobile</td>
                    <td>2022</td>
                    <td>Pengembangan aplikasi Android</td>
                </tr>
                <tr>
                    <td>Sistem Inventory</td>
                    <td>2021</td>
                    <td>Sistem manajemen inventory</td>
                </tr>
            </tbody>
        </table>
    </section>
</body>
</html>
