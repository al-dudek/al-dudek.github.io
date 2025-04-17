<!DOCTYPE html>
<html lang="pl" class="no-js">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wyjazd na Svalbard - Jesień 2025 | Arktyczna Przygoda</title>

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">

    <!-- AOS (Animate On Scroll) CSS -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">

    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />

    <!-- Custom CSS -->
    <style>
        :root {
            --primary-dark-blue: #0a2e5c;
            --accent-light-blue: #5cb8e6;
            --light-gray-bg: #f8f9fa;
            --white: #ffffff;
            --light-blue-bg: #eef3f9;
            --text-dark: #333;
            --text-muted-light: #f0f0f0;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            color: var(--text-dark);
            background-color: var(--light-gray-bg);
            overflow-x: hidden; /* Prevent horizontal scroll */
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            color: var(--primary-dark-blue);
        }

        .hero {
            position: relative;
            height: 100vh;
            color: var(--white);
            text-align: center;
            display: flex;
            align-items: center;
            justify-content: center;
            background: url('https://images.unsplash.com/photo-1549667742-e1f860d64f4e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80') no-repeat center center; /* Specific Svalbard Landscape */
            background-size: cover;
            overflow: hidden;
        }

        .hero::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(rgba(0, 20, 50, 0.6), rgba(0, 20, 50, 0.8)); /* Slightly darker gradient overlay */
            z-index: 1;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 800px;
            padding: 30px;
        }

        .hero h1 {
             font-size: clamp(2.5rem, 6vw, 4rem); /* Responsive font size */
             margin-bottom: 1.5rem;
             color: var(--white);
             text-shadow: 2px 2px 6px rgba(0,0,0,0.6);
        }

        .hero p.lead {
            font-size: clamp(1rem, 2.5vw, 1.25rem);
            margin-bottom: 2.5rem;
            color: rgba(255, 255, 255, 0.9);
            text-shadow: 1px 1px 4px rgba(0,0,0,0.5);
        }

        .btn-outline-light {
            border-width: 2px;
            padding: 12px 30px;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        .btn-outline-light:hover {
            background-color: var(--white);
            color: var(--primary-dark-blue);
        }


        .navbar {
            transition: background-color 0.4s ease-in-out, box-shadow 0.4s ease-in-out;
            background-color: rgba(10, 46, 92, 0.85); /* Semi-transparent dark blue */
            padding-top: 1rem;
            padding-bottom: 1rem;
        }

        .navbar-brand {
             font-family: 'Montserrat', sans-serif;
             font-weight: 700;
             color: var(--white) !important;
             font-size: 1.5rem;
        }
         .navbar-nav .nav-link {
            color: var(--text-muted-light) !important;
            margin: 0 0.75rem;
            transition: color 0.3s ease;
            font-weight: 600;
            position: relative;
            padding-bottom: 0.5rem;
        }
        .navbar-nav .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 2px;
            background-color: var(--accent-light-blue);
            transition: width 0.3s ease;
        }
        .navbar-nav .nav-link:hover::after,
        .navbar-nav .nav-link.active::after {
             width: 60%;
        }
        .navbar-nav .nav-link:hover,
        .navbar-nav .nav-link.active {
            color: var(--white) !important;
        }

        .navbar.scrolled {
            background-color: var(--primary-dark-blue); /* Solid dark blue when scrolled */
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
            padding-top: 0.75rem;
            padding-bottom: 0.75rem;
        }

        section {
            padding: 100px 0;
            overflow: hidden; /* Prevent AOS elements sliding out */
        }

        section:nth-of-type(odd) {
             background-color: var(--white);
        }
        section:nth-of-type(even) {
             background-color: var(--light-blue-bg);
        }
        #intro { background-color: var(--white); } /* Ensure intro is white */

        .section-title {
            text-align: center;
            margin-bottom: 60px;
            color: var(--primary-dark-blue);
        }

        .section-title h2 {
            font-size: clamp(2rem, 5vw, 2.8rem);
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
            padding-bottom: 10px;
        }
         .section-title .underline {
            width: 100px;
            height: 4px;
            background-color: var(--accent-light-blue);
            margin: 5px auto 20px auto;
            border-radius: 2px;
        }
        .section-title p {
            font-size: 1.1rem;
            color: #555;
        }

        .icon {
            font-size: 3rem;
            color: var(--accent-light-blue);
            margin-bottom: 20px;
            display: block; /* Center icon above title */
            text-align: center;
        }
        .section-title .icon { /* Icon specifically within section title */
             margin-bottom: 10px;
        }


        .card {
            border: none;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            transition: transform 0.35s ease, box-shadow 0.35s ease;
            height: 100%;
            overflow: hidden; /* Ensure rounded corners clip image */
        }
        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.12);
        }

        .card-img-top {
            height: 220px;
            object-fit: cover;
            border-top-left-radius: 10px; /* Match card radius */
            border-top-right-radius: 10px;
        }
        .card-body {
            padding: 25px;
        }
        .card-title {
            margin-bottom: 15px;
            font-size: 1.3rem;
        }

        .list-group-item {
            border: none;
            padding-left: 0;
            background-color: transparent; /* Ensure list items inherit card bg */
            margin-bottom: 5px;
        }
        .list-group-item i.fa-fw { /* Specific styling for fixed-width icons */
             color: var(--accent-light-blue);
             margin-right: 12px;
             width: 22px;
             text-align: center;
        }
        .list-unstyled i { /* General styling for list icons */
             color: var(--accent-light-blue);
             margin-right: 10px;
             width: 20px;
             text-align: center;
        }


        .map-container {
            position: relative;
            overflow: hidden;
            padding-top: 56.25%; /* 16:9 Aspect Ratio */
            margin-top: 25px;
            border-radius: 10px;
            box-shadow: 0 6px 18px rgba(0,0,0,0.1);
        }
        .map-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: 0;
        }

        .polar-bear-warning {
            background-color: #fff8e1; /* Lighter yellow */
            border-left: 6px solid #ffc107; /* Amber */
            padding: 25px;
            margin-top: 25px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(133, 100, 4, 0.1);
        }
        .polar-bear-warning h4 {
             color: #b38600; /* Darker yellow/brown */
             font-weight: 700;
        }
        .polar-bear-warning i {
             color: #ffc107;
             margin-right: 10px;
        }


        .insurance-info {
             background-color: #e0f7fa; /* Lighter cyan */
             border-left: 6px solid #00bcd4; /* Cyan */
             padding: 25px;
             margin-top: 25px;
             border-radius: 8px;
             box-shadow: 0 4px 10px rgba(12, 84, 96, 0.1);
        }
         .insurance-info h4 {
              color: #007a8a; /* Darker cyan */
              font-weight: 700;
         }
        .insurance-info i {
             color: #00bcd4;
             margin-right: 10px;
        }

        .budget-table {
            margin-top: 40px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            border-radius: 10px;
            overflow: hidden; /* Clip shadow */
        }
         .budget-table th {
             background-color: var(--primary-dark-blue);
             color: var(--white);
             padding: 15px;
             text-align: center;
         }
        .budget-table td {
             vertical-align: middle;
             padding: 15px;
             text-align: center;
        }
        .budget-table tbody tr:nth-child(odd) {
            background-color: var(--white);
        }
        .budget-table tbody tr:nth-child(even) {
             background-color: var(--light-blue-bg);
        }
        .budget-table tfoot {
            font-weight: bold;
        }
        .budget-table tfoot tr.table-dark td {
            background-color: #343a40; /* Dark gray for total */
            color: var(--white);
        }
         .budget-table tfoot tr.table-secondary td {
            background-color: #e2e3e5; /* Light gray for per person */
            color: var(--text-dark);
         }


        .checklist li {
            margin-bottom: 12px;
            display: flex;
            align-items: center;
        }
         .checklist li i {
             color: #28a745; /* Green check */
             margin-right: 12px;
             font-size: 1.2rem;
         }

        footer {
            background-color: var(--primary-dark-blue);
            color: var(--text-muted-light);
            padding: 30px 0;
            text-align: center;
        }
        footer p {
            margin-bottom: 0;
            font-size: 0.9rem;
        }

        /* Accordion Styling */
        .accordion-button {
            background-color: var(--light-blue-bg);
            color: var(--primary-dark-blue);
            font-weight: 600;
        }
        .accordion-button:not(.collapsed) {
             background-color: var(--accent-light-blue);
             color: var(--white);
             box-shadow: inset 0 -1px 0 rgba(0,0,0,.125);
        }
         .accordion-button:focus {
            box-shadow: 0 0 0 0.25rem rgba(92, 184, 230, 0.5); /* Light blue focus */
         }
         .accordion-body {
             background-color: var(--white);
             padding: 20px;
         }
        .accordion-item {
            border: 1px solid #dee2e6;
            border-radius: 5px;
            margin-bottom: 10px;
            overflow: hidden; /* For rounded corners */
        }
        .accordion-item:first-of-type {
            border-top-left-radius: 5px;
            border-top-right-radius: 5px;
        }
        .accordion-item:last-of-type {
             border-bottom-left-radius: 5px;
            border-bottom-right-radius: 5px;
        }
        .accordion-button i {
            margin-right: 10px;
            transition: transform 0.3s ease;
        }
        .accordion-button:not(.collapsed) i {
             transform: rotate(90deg);
        }

        /* Info items styling */
         .info-item {
            display: flex;
            align-items: flex-start; /* Align icon top */
            margin-bottom: 1.5rem;
         }
        .info-item i.fa-fw {
            font-size: 1.5rem;
            color: var(--accent-light-blue);
            margin-right: 15px;
            margin-top: 5px; /* Align icon slightly lower */
             width: 30px;
             flex-shrink: 0; /* Prevent icon shrinking */
        }
         .info-item p {
            margin-bottom: 0;
         }

        /* Lead paragraph styling */
        #intro .lead {
            font-size: 1.2rem;
            font-weight: 400;
            color: #555;
            line-height: 1.7;
        }
        .text-danger-emphasis { /* Bootstrap class for stronger danger text */
            font-weight: bold;
        }

        /* AOS Customization */
        [data-aos="fade-up"] {
          transform: translateY(30px);
        }
        [data-aos="fade-in"] {
            opacity: 0;
        }

    </style>
</head>
<body>

    <!-- Hero Section -->
    <header class="hero" id="page-top">
        <div class="hero-content" data-aos="fade-in" data-aos-duration="1200" data-aos-delay="200">
            <h1>Arktyczna Przygoda</h1>
            <p class="lead">Twoja niezapomniana 7-dniowa wyprawa na Svalbard z Warszawy<br>Jesień 2025</p>
            <a href="#intro" class="btn btn-outline-light btn-lg scroll-link">Odkryj Plan</a>
        </div>
    </header>

    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-dark fixed-top" id="mainNav">
        <div class="container px-4">
            <a class="navbar-brand scroll-link" href="#page-top">Svalbard 2025</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
                <i class="fas fa-bars"></i>
            </button>
            <div class="collapse navbar-collapse" id="navbarResponsive">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link scroll-link" href="#intro">Wstęp</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#logistyka">Loty</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#zakwaterowanie">Noclegi</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#pogoda">Pogoda</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#atrakcje">Atrakcje</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#operatorzy">Operatorzy</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#praktyczne">Info</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#plan">Plan</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#budzet">Budżet</a></li>
                    <li class="nav-item"><a class="nav-link scroll-link" href="#przygotowania">Start!</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Main Content -->
    <main>

        <!-- Intro Section -->
        <section id="intro">
            <div class="container" data-aos="fade-up">
                <div class="section-title">
                    <i class="fas fa-door-open icon"></i>
                    <h2>Wrota do Arktyki Czekają</h2>
                    <div class="underline"></div>
                </div>
                <div class="row justify-content-center">
                    <div class="col-lg-9">
                         <p class="lead text-center mb-4">Svalbard, archipelag na północ od Norwegii kontynentalnej, kusi surowym pięknem, dziką przyrodą i niepowtarzalną atmosferą Arktyki.</p>
                         <p class="text-center">Jesień to czas niezwykłej transformacji – dni stają się krótsze, krajobraz szykuje się do zimy, a na niebie rośnie szansa ujrzenia magicznej zorzy polarnej. Ten przewodnik pomoże zaplanować niezapomnianą, 7-dniową wyprawę dla dwóch osób z Warszawy na Svalbard jesienią 2025 (wrzesień-listopad), prezentując kluczowe informacje i wskazówki.</p>
                         <p class="text-center fst-italic mt-4"><small>Uwaga: Informacje opierają się na danych dostępnych w momencie tworzenia. Ceny, rozkłady i dostępność mogą ulec zmianie. Zawsze weryfikuj aktualne dane przed rezerwacją.</small></p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Logistyka Section -->
        <section id="logistyka">
            <div class="container" data-aos="fade-up">
                <div class="section-title">
                     <i class="fas fa-plane-departure icon"></i>
                    <h2>Logistyka Podróży</h2>
                    <div class="underline"></div>
                    <p>Z Warszawy (WAW) do Longyearbyen (LYR)</p>
                </div>
                <div class="row justify-content-center">
                    <div class="col-lg-9">
                        <p class="text-center mb-5">Podróż lotnicza na Svalbard wymaga co najmniej jednej przesiadki, najczęściej w Oslo (OSL). Bezpośrednie połączenia nie istnieją.</p>
                        <div class="info-item mb-4">
                            <i class="fas fa-route fa-fw"></i>
                            <p><strong>Linie Lotnicze i Połączenia:</strong> Główni przewoźnicy przez Norwegię to <strong class="text-primary">Scandinavian Airlines (SAS)</strong> i <strong class="text-primary">Norwegian</strong>. Oferują regularne loty do Longyearbyen (LYR) z Oslo. SAS lata też przez Kopenhagę/Sztokholm. Loty WAW-OSL obsługują m.in. SAS, Norwegian, LOT.</p>
                        </div>
                         <div class="info-item mb-4">
                             <i class="far fa-clock fa-fw"></i>
                             <p><strong>Czas Podróży:</strong> Najkrótszy szacowany czas lotu z przesiadką to ok. <strong class="text-primary">6 godz. 15 min</strong>, ale całkowity czas (z oczekiwaniem) może być znacznie dłuższy (nawet >20h). Sprawdź dokładnie czas przesiadki!</p>
                         </div>
                         <div class="info-item mb-4">
                             <i class="fas fa-tags fa-fw"></i>
                            <p><strong>Koszty Orientacyjne (Jesień 2025, 1 os. w obie strony):</strong> Ceny mocno zmienne. Najtańsze oferty (szczególnie we wrześniu, rezerwowane wcześnie) mogą startować od ok. <strong class="text-primary">1300 PLN</strong>. Średnio należy liczyć się z wydatkiem rzędu <strong class="text-primary">1900 - 4200 PLN</strong>. Używaj wyszukiwarek i alertów cenowych.</p>
                         </div>
                         <p class="text-center mt-5">
                            <a href="https://www.google.com/travel/flights/flights-from-warsaw-to-longyearbyen.html" target="_blank" class="btn btn-primary me-2 mb-2"><i class="fab fa-google me-2"></i>Sprawdź w Google Flights</a>
                            <a href="https://www.skyscanner.pl/trasy/waw/lyr/warszawa-chopina-do-longyearbyen.html" target="_blank" class="btn btn-info text-white mb-2"><i class="fab fa-fly me-2"></i>Sprawdź w Skyscanner</a>
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Zakwaterowanie Section -->
        <section id="zakwaterowanie">
            <div class="container" data-aos="fade-up">
                 <div class="section-title">
                     <i class="fas fa-bed icon"></i>
                    <h2>Zakwaterowanie w Longyearbyen</h2>
                    <div class="underline"></div>
                    <p>Gdzie spać w sercu Arktyki?</p>
                </div>
                <p class="text-center mb-5 col-lg-8 mx-auto">Longyearbyen oferuje różnorodne opcje, od hoteli premium po przytulne pensjonaty i apartamenty. Ceny są generalnie wysokie, a rezerwacja z dużym wyprzedzeniem jest kluczowa!</p>

                <div class="row gy-4 justify-content-center">
                    <!-- Hotele Wyższego Standardu -->
                    <div class="col-lg-4 col-md-6">
                        <div class="card h-100">
                             <img src="https://images.unsplash.com/photo-1618773928121-c32242e63f39?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" class="card-img-top" alt="Luksusowy pokój hotelowy">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title">Hotele Wyższego Standardu (4*)</h5>
                                <p class="card-text">Pełen komfort, restauracje, piękne widoki. Idealne dla ceniących wygodę.</p>
                                <ul class="list-unstyled mt-auto">
                                    <li><i class="fas fa-star fa-fw"></i> Przykłady: Radisson Blu Polar, Funken Lodge, Svalbard Hotell | Polfareren</li>
                                    <li><i class="fas fa-map-marker-alt fa-fw"></i> Lokalizacja: Zazwyczaj w centrum lub z dobrym widokiem.</li>
                                    <li><i class="fas fa-tag fa-fw"></i> Cena (2os./noc): od 940 - 1500+ PLN</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                     <!-- Hotele Średniego Standardu -->
                     <div class="col-lg-4 col-md-6">
                        <div class="card h-100">
                            <img src="https://images.unsplash.com/photo-1568495248636-6432b97bd949?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80" class="card-img-top" alt="Przytulny pokój hotelowy">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title">Hotele Średniego Standardu (3-3.5*)</h5>
                                <p class="card-text">Komfortowe pokoje, dobra lokalizacja, często unikalny wystrój (np. Basecamp w stylu traperskim).</p>
                                <ul class="list-unstyled mt-auto">
                                    <li><i class="fas fa-star-half-alt fa-fw"></i> Przykłady: Svalbard Hotell | The Vault, Basecamp Hotel</li>
                                    <li><i class="fas fa-map-marker-alt fa-fw"></i> Lokalizacja: Zazwyczaj w centrum.</li>
                                    <li><i class="fas fa-tag fa-fw"></i> Cena (2os./noc): od 640 - 900 PLN</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <!-- Hostele / Pensjonaty -->
                    <div class="col-lg-4 col-md-6">
                        <div class="card h-100">
                             <img src="https://images.unsplash.com/photo-1584132967334-10e028bd69f7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" class="card-img-top" alt="Wspólna przestrzeń w hostelu">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title">Hostele / Pensjonaty</h5>
                                <p class="card-text">Opcje ekonomiczne, często ze wspólnymi łazienkami/kuchnią. Świetna atmosfera i możliwość poznania innych podróżników.</p>
                                <ul class="list-unstyled mt-auto">
                                    <li><i class="fas fa-users fa-fw"></i> Przykłady: Mary-Ann's Polarrigg, Coal Miners' Cabins, Gjestehuset 102, Haugen Pensjonat</li>
                                     <li><i class="fas fa-map-marker-alt fa-fw"></i> Lokalizacja: Centrum lub nieco oddalone (sprawdź!).</li>
                                     <li><i class="fas fa-tag fa-fw"></i> Cena (2os./noc): od 400 - 600 PLN</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                     <!-- Apartamenty -->
                     <div class="col-lg-4 col-md-6">
                        <div class="card h-100">
                             <img src="https://images.unsplash.com/photo-1616594039964-ae9021a400a0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80" class="card-img-top" alt="Nowoczesny apartament">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title">Apartamenty</h5>
                                <p class="card-text">Więcej przestrzeni, prywatność, aneks kuchenny umożliwiający samodzielne gotowanie (oszczędność!).</p>
                                <ul class="list-unstyled mt-auto">
                                     <li><i class="fas fa-home fa-fw"></i> Przykłady: Svalbard Hotell | Lodge, wynajem przez Airbnb/Booking.</li>
                                     <li><i class="fas fa-map-marker-alt fa-fw"></i> Lokalizacja: Różna, często w centrum.</li>
                                     <li><i class="fas fa-tag fa-fw"></i> Cena (2os./noc): od ~1000 PLN (Airbnb) / ~1800 PLN (Lodge)</li>
                                </ul>
                             </div>
                        </div>
                     </div>
                 </div>

                <!-- Mapa Lokalizacji -->
                <div class="row mt-5 justify-content-center">
                    <div class="col-lg-10">
                         <h4 class="text-center mb-4">Orientacyjna Lokalizacja Zakwaterowania w Longyearbyen</h4>
                        <div class="map-container">
                             <iframe
                                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d12678.442682794687!2d15.597089888800988!3d78.2231962033141!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x459cb7b7f9b8e7b1%3A0x4ef9c23c506f017e!2sLongyearbyen%2C%20Svalbard%20i%20Jan%20Mayen!5e0!3m2!1spl!2spl!4v1718656556636!5m2!1spl!2spl"
                                width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"
                                referrerpolicy="no-referrer-when-downgrade"></iframe>
                        </div>
                        <p class="text-muted text-center mt-3"><small>Mapa pokazuje centrum Longyearbyen. Hotele jak Radisson, Polfareren, The Vault są w ścisłym centrum. Coal Miners' Cabins i Gjestehuset 102 są ok. 2-2.5 km na południowy-wschód. Funken Lodge jest na wzgórzu.</small></p>
                         <p class="text-center mt-4">
                             <a href="https://www.booking.com/accommodation/city/no/longyearbyen.pl.html" target="_blank" class="btn btn-primary"><i class="fas fa-search-location me-2"></i>Sprawdź dostępność na Booking.com</a>
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Pogoda i Ekwipunek Section -->
        <section id="pogoda">
             <div class="container" data-aos="fade-up">
                 <div class="section-title">
                     <i class="fas fa-temperature-three-quarters icon"></i>
                     <h2>Pogoda i Ekwipunek</h2>
                     <div class="underline"></div>
                     <p>Jak ubrać się na spotkanie z Arktyką?</p>
                 </div>
                 <div class="row gy-5 align-items-center">
                     <div class="col-lg-6">
                         <h3 class="mb-4"><i class="fas fa-cloud-sun-rain me-2 text-primary"></i>Warunki Pogodowe (IX - XI)</h3>
                         <p>Jesień to okres przejściowy z dynamicznie zmieniającą się pogodą i szybko skracającym się dniem.</p>
                         <ul class="list-group list-group-flush">
                             <li class="list-group-item"><i class="fas fa-thermometer-half fa-fw"></i><strong>Temperatury:</strong> Od +1/-1°C (IX), przez -3/-5°C (X), do -6/-11°C (XI). Wiatr znacząco obniża odczuwalną!</li>
                             <li class="list-group-item"><i class="fas fa-cloud-showers-heavy fa-fw"></i><strong>Opady:</strong> Deszcz/śnieg (IX), głównie śnieg (X, XI). Stosunkowo wilgotno.</li>
                            <li class="list-group-item"><i class="fas fa-wind fa-fw"></i><strong>Wiatr:</strong> Może być silny i porywisty, potęgując uczucie zimna.</li>
                             <li class="list-group-item"><i class="far fa-lightbulb fa-fw"></i><strong>Światło Dzienne:</strong> Drastycznie maleje: >18h (pocz. IX) → ~6h (pocz. X) → <strong class="text-primary">0h (noc polarna od końca X)</strong>.</li>
                         </ul>
                     </div>
                     <div class="col-lg-6">
                         <h3 class="mb-4"><i class="fas fa-user-astronaut me-2 text-primary"></i>Niezbędny Ekwipunek</h3>
                         <p>Kluczem jest ubieranie się <strong class="text-primary">"na cebulkę" (warstwowo)</strong>. Komfort = bezpieczeństwo.</p>
                         <ul class="list-group list-group-flush">
                             <li class="list-group-item"><i class="fas fa-layer-group fa-fw"></i><strong>Warstwy:</strong> Termoaktywna (baza), Izolująca (polar/puch), Ochronna (wiatro/wodoodporna).</li>
                             <li class="list-group-item"><i class="fas fa-hat-winter fa-fw"></i><strong>Głowa:</strong> Ciepła czapka, kominiarka/komin.</li>
                             <li class="list-group-item"><i class="fas fa-mitten fa-fw"></i><strong>Ręce:</strong> Cienkie + grube, nieprzemakalne łapawice.</li>
                             <li class="list-group-item"><i class="fas fa-shoe-prints fa-fw"></i><strong>Stopy:</strong> Ciepłe, wodoodporne buty zimowe (dobry bieżnik!), grube skarpety (wełna!).</li>
                             <li class="list-group-item"><i class="fas fa-headlamp fa-fw text-danger"></i><strong class="text-danger-emphasis">Absolutnie Konieczne:</strong> Latarka czołowa (od X), okulary UV (IX), krem UV, termos, mały plecak, aparat (+baterie), ogrzewacze.</li>
                         </ul>
                     </div>
                 </div>
             </div>
        </section>

         <!-- Atrakcje Section -->
        <section id="atrakcje">
            <div class="container" data-aos="fade-up">
                <div class="section-title">
                    <i class="fas fa-binoculars icon"></i>
                    <h2>Atrakcje i Aktywności</h2>
                    <div class="underline"></div>
                    <p>Co czeka na Ciebie na Svalbardzie jesienią?</p>
                </div>

                <div class="row gy-4">
                    <!-- Zorza Polarna -->
                    <div class="col-lg-4 col-md-6 d-flex align-items-stretch">
                        <div class="card h-100">
                            <img src="https://images.unsplash.com/photo-1531366936337-7c912a4589a7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" class="card-img-top" alt="Zorza Polarna nad górami">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-meteor text-success me-2"></i>Polowanie na Zorzę Polarną</h5>
                                <p class="card-text">Najlepsze szanse od października (ciemne noce). Listopad (noc polarna) oferuje 24h możliwości (teoretycznie). Wymaga ucieczki od świateł miasta – idealne są zorganizowane wycieczki.</p>
                            </div>
                        </div>
                    </div>
                    <!-- Psie Zaprzęgi -->
                     <div class="col-lg-4 col-md-6 d-flex align-items-stretch">
                        <div class="card h-100">
                             <img src="https://images.unsplash.com/photo-1559723940-4e204601c342?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" class="card-img-top" alt="Psy husky ciągnące zaprzęg">
                             <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-dog text-info me-2"></i>Przejażdżka Psim Zaprzęgiem</h5>
                                <p class="card-text">Jesienią (IX-X) na specjalnych wózkach na kołach. Gdy spadnie śnieg (zwykle od XI/XII), możliwe są wycieczki na saniach. Niezapomniane spotkanie z arktycznymi psami i dziką przyrodą.</p>
                            </div>
                        </div>
                    </div>
                    <!-- Skutery Śnieżne -->
                     <div class="col-lg-4 col-md-6 d-flex align-items-stretch">
                        <div class="card h-100">
                             <img src="https://images.unsplash.com/photo-1604537586132-14a8f814b38a?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2069&q=80" class="card-img-top" alt="Skuter śnieżny na tle arktycznego krajobrazu">
                             <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-snowflake text-primary me-2"></i>Wyprawy Skuterami Śnieżnymi</h5>
                                <p class="card-text">Dostępność jesienią BARDZO ograniczona (zależna od śniegu). Sezon zwykle startuje zimą (XII-II). W listopadzie szansa rośnie, ale bez gwarancji. Wymagane prawo jazdy.</p>
                            </div>
                         </div>
                     </div>
                    <!-- Jaskinie Lodowe -->
                    <div class="col-lg-4 col-md-6 d-flex align-items-stretch">
                        <div class="card h-100">
                             <img src="https://images.unsplash.com/photo-1551522434-7511a350d5a3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" class="card-img-top" alt="Wnętrze błękitnej jaskini lodowej">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-icicles text-info me-2"></i>Eksploracja Jaskiń Lodowych</h5>
                                <p class="card-text">Zazwyczaj dostępne zimą (od XI/XII). Jesienią dostępność ograniczona. Możliwe piesze wycieczki lub łączone (z psami/skuterem, jeśli warunki pozwolą). Magiczny, błękitny świat lodu.</p>
                            </div>
                        </div>
                    </div>
                    <!-- Rejsy -->
                    <div class="col-lg-4 col-md-6 d-flex align-items-stretch">
                         <div class="card h-100">
                            <img src="https://images.unsplash.com/photo-1588628040786-c59575388a8f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80" class="card-img-top" alt="Statek wycieczkowy przy lodowcu na Svalbardzie">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-ship text-warning me-2"></i>Rejsy Statkiem po Fiordach</h5>
                                <p class="card-text">Sezon na większość rejsów kończy się jesienią. Krótsze wycieczki po Isfjordzie mogą być dostępne do IX/X (zależnie od pogody i lodu). W listopadzie raczej niedostępne.</p>
                            </div>
                        </div>
                     </div>
                    <!-- Muzea i Lokalne Atrakcje -->
                    <div class="col-lg-4 col-md-6 d-flex align-items-stretch">
                        <div class="card h-100">
                             <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/55/Svalbard_Museum_interior_01.jpg/640px-Svalbard_Museum_interior_01.jpg" class="card-img-top" alt="Wnętrze Muzeum Svalbardu">
                             <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-landmark text-secondary me-2"></i>Muzea i Lokalne Atrakcje</h5>
                                 <p class="card-text">Idealne na poznanie historii i kultury: Muzeum Svalbardu, Muzeum Ekspedycji Polarnych, Kopalnia Gruve 3 (zwiedzanie!), Kościół Svalbardu, Browar Svalbard (degustacje!). Zobacz wejście do Globalnego Banku Nasion.</p>
                             </div>
                         </div>
                    </div>
                    <!-- Piesze Wycieczki -->
                    <div class="col-lg-4 col-md-6 d-flex align-items-stretch">
                        <div class="card h-100">
                            <img src="https://images.unsplash.com/photo-1617845913801-a3f8c69335b7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1974&q=80" class="card-img-top" alt="Grupa turystów podczas wędrówki na Svalbardzie">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-hiking text-success me-2"></i>Wędrówki z Przewodnikiem</h5>
                                <p class="card-text"><strong class="text-danger-emphasis">Zawsze z uzbrojonym przewodnikiem</strong> (niedźwiedzie!). Dostępne jesienią, dopóki pozwalają warunki. Trasy o różnym stopniu trudności oferują wspaniałe widoki i kontakt z naturą.</p>
                            </div>
                        </div>
                    </div>
                     <!-- Mapa Atrakcji -->
                    <div class="col-lg-8 col-md-6 d-flex align-items-stretch">
                         <div class="card h-100">
                            <div class="card-body d-flex flex-column">
                                <h5 class="card-title"><i class="fas fa-map-marked-alt text-primary me-2"></i>Mapa Atrakcji i Obszarów Aktywności</h5>
                                <p class="card-text">Mapa pokazuje centrum Longyearbyen (muzea, kościół, browar) oraz przybliżone obszary/kierunki niektórych aktywności.</p>
                                <div class="map-container mt-auto">
                                    <iframe src="https://www.google.com/maps/embed?pb=!1m16!1m12!1m3!1d25355.559862797135!2d15.565508774716274!3d78.22725109099665!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!2m1!1sLongyearbyen%20attractions!5e0!3m2!1spl!2spl!4v1718657274787!5m2!1spl!2spl" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                                </div>
                                <p class="text-muted mt-3 mb-0"><small><strong>Centrum:</strong> Muzeum Svalbardu, galerie, sklepy. <strong>Kierunek SE:</strong> Globalny Bank Nasion (na zboczu), doliny Adventdalen/Bolterdalen (psie zaprzęgi, wędrówki).</small></p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Operatorzy Section -->
        <section id="operatorzy">
            <div class="container" data-aos="fade-up">
                <div class="section-title">
                     <i class="fas fa-concierge-bell icon"></i>
                     <h2>Lokalni Operatorzy Turystyczni</h2>
                     <div class="underline"></div>
                     <p>Zaufaj ekspertom od arktycznych przygód</p>
                 </div>
                 <div class="row justify-content-center">
                     <div class="col-lg-9">
                        <p class="text-center mb-5">W Longyearbyen działa wielu sprawdzonych operatorów. Rezerwacja wycieczek online z wyprzedzeniem to najlepszy sposób na zapewnienie sobie miejsca na wymarzone aktywności.</p>
                        <h4 class="mb-4 text-center">Polecani Operatorzy (Przykłady):</h4>
                         <div class="row text-center gy-3">
                            <div class="col-md-4"><i class="fas fa-anchor me-2 text-primary"></i>Hurtigruten Svalbard</div>
                            <div class="col-md-4"><i class="fas fa-mountain me-2 text-primary"></i>Svalbard Adventures</div>
                            <div class="col-md-4"><i class="fas fa-camera-retro me-2 text-primary"></i>Better Moments</div>
                            <div class="col-md-4"><i class="fas fa-dog me-2 text-primary"></i>Green Dog Svalbard</div>
                            <div class="col-md-4"><i class="fas fa-paw me-2 text-primary"></i>Arctic Husky Travellers</div>
                            <div class="col-md-4"><i class="fas fa-campground me-2 text-primary"></i>Basecamp Explorer</div>
                            <div class="col-md-4"><i class="fas fa-hiking me-2 text-primary"></i>Svalbard Wildlife Expeditions</div>
                            <div class="col-md-4"><i class="fas fa-compass me-2 text-primary"></i>Spitzbergen Adventures</div>
                             <div class="col-md-4"><i class="fas fa-binoculars me-2 text-primary"></i>...i inni!</div>
                         </div>
                         <p class="mt-5 text-center"><strong>Wskazówka:</strong> Sprawdź aktualne oferty i harmonogramy jesienne bezpośrednio na stronach operatorów. Dostępność niektórych aktywności (szczególnie zimowych jak skutery) zależy od warunków pogodowych i śniegowych.</p>
                          <p class="text-center mt-4">
                            <a href="https://en.visitsvalbard.com/things-to-do/activities" target="_blank" class="btn btn-primary"><i class="fas fa-search me-2"></i>Przeglądaj aktywności na VisitSvalbard.com</a>
                         </p>
                     </div>
                 </div>
             </div>
        </section>

        <!-- Praktyczne Section -->
        <section id="praktyczne">
             <div class="container" data-aos="fade-up">
                <div class="section-title">
                    <i class="fas fa-info-circle icon"></i>
                    <h2>Informacje Praktyczne</h2>
                    <div class="underline"></div>
                    <p>Kluczowe zasady i wskazówki dla podróżujących</p>
                </div>
                 <div class="row gy-5">
                     <!-- Lewa Kolumna: Wjazd, Waluta -->
                     <div class="col-lg-6">
                         <h3 class="mb-4"><i class="fas fa-passport me-2 text-primary"></i>Wjazd i Dokumenty (Obywatele PL)</h3>
                         <ul class="list-unstyled">
                             <li class="info-item"><i class="fas fa-flag fa-fw"></i><p><strong>Status Svalbardu:</strong> Część Norwegii, ale <strong class="text-danger">poza Strefą Schengen</strong>/EOG.</p></li>
                             <li class="info-item"><i class="fas fa-plane fa-fw"></i><p><strong>Tranzyt:</strong> Loty zawsze przez Norwegię (Schengen).</p></li>
                             <li class="info-item"><i class="fas fa-id-card fa-fw"></i><p><strong>Dokumenty:</strong> Ważny dowód osobisty lub paszport. Kontrola na trasie Norwegia-Svalbard-Norwegia. <strong class="text-primary">Zalecany paszport</strong>.</p></li>
                             <li class="info-item"><i class="fas fa-times-circle fa-fw"></i><p><strong>Wiza:</strong> Nie jest wymagana dla obywateli UE.</p></li>
                             <li class="info-item"><i class="fas fa-money-bill-wave fa-fw"></i><p><strong>Środki:</strong> Należy posiadać środki na utrzymanie (formalny wymóg).</p></li>
                         </ul>

                         <h3 class="mt-5 mb-4"><i class="fas fa-coins me-2 text-primary"></i>Waluta, Płatności i Koszty</h3>
                         <ul class="list-unstyled">
                             <li class="info-item"><i class="fas fa-money-bill-alt fa-fw"></i><p><strong>Waluta:</strong> Korona norweska (NOK).</p></li>
                             <li class="info-item"><i class="far fa-credit-card fa-fw"></i><p><strong>Płatności:</strong> Karty płatnicze są <strong class="text-primary">powszechnie akceptowane</strong>. Gotówka rzadko potrzebna.</p></li>
                             <li class="info-item"><i class="fas fa-shopping-cart fa-fw"></i><p><strong>Koszty:</strong> <strong class="text-danger">Wysokie.</strong> Norwegia jest droga, Svalbard generalnie jeszcze droższy. Orientacyjnie: piwo 100-140 NOK, posiłek 200+ NOK (tani) / 500+ NOK (średni/os.).</p></li>
                             <li class="info-item"><i class="fas fa-taxi fa-fw"></i><p><strong>Transport Lokalny:</strong> Centrum Longyearbyen małe (spacer). Działa autobus lotniskowy. Taksówki są drogie.</p></li>
                         </ul>
                     </div>
                     <!-- Prawa Kolumna: Niedźwiedzie, Ubezpieczenie -->
                     <div class="col-lg-6">
                        <div class="polar-bear-warning">
                            <h4><i class="fas fa-exclamation-triangle"></i>Bezpieczeństwo – Niedźwiedzie Polarne</h4>
                            <p class="mb-2"><strong>NAJWYŻSZA OSTROŻNOŚĆ!</strong> Niedźwiedzie są realnym zagrożeniem na całym archipelagu, także blisko osiedli.</p>
                            <ul class="list-unstyled small">
                                <li class="mb-1"><i class="fas fa-ban text-danger me-1"></i><strong class="text-danger-emphasis">ABSOLUTNY ZAKAZ</strong> opuszczania Longyearbyen bez uzbrojonego przewodnika!</li>
                                <li class="mb-1"><i class="fas fa-shield-alt me-1"></i>Poruszanie się poza miastem <strong class="text-danger-emphasis">WYŁĄCZNIE</strong> w ramach zorganizowanych wycieczek.</li>
                                <li class="mb-1"><i class="fas fa-eye me-1"></i>Bądź czujny, obserwuj otoczenie.</li>
                                <li class="mb-1"><i class="fas fa-paw me-1"></i>Nigdy nie zbliżaj się, nie karm, nie prowokuj.</li>
                                <li class="mb-1"><i class="fas fa-leaf me-1"></i>Niedźwiedzie są chronione prawem.</li>
                             </ul>
                         </div>

                         <div class="insurance-info mt-4">
                            <h4><i class="fas fa-file-medical-alt"></i>Ubezpieczenie Podróżne</h4>
                            <p class="mb-2"><strong>KRYTYCZNIE WAŻNE!</strong> Standardowa polisa jest niewystarczająca.</p>
                            <ul class="list-unstyled small">
                                 <li class="mb-1"><i class="fas fa-globe-americas me-1"></i>Musi obejmować <strong class="text-primary">warunki arktyczne</strong>.</li>
                                 <li class="mb-1"><i class="fas fa-ambulance text-danger me-1"></i>Kluczowe: pokrycie kosztów <strong class="text-danger-emphasis">ewakuacji medycznej i repatriacji</strong> (bardzo wysokie sumy, min. 50-100 tys. EUR/USD).</li>
                                 <li class="mb-1"><i class="fas fa-snowboarding me-1"></i>Musi obejmować planowane aktywności (skutery, psy itp.).</li>
                                <li class="mb-1"><i class="fas fa-check-circle text-success me-1"></i>Wykup <strong class="text-primary">kompleksową polisę</strong> od renomowanego ubezpieczyciela przed wyjazdem.</li>
                            </ul>
                        </div>
                     </div>
                 </div>
            </div>
        </section>

        <!-- Plan Pobytu Section -->
        <section id="plan">
            <div class="container" data-aos="fade-up">
                <div class="section-title">
                    <i class="far fa-calendar-check icon"></i>
                    <h2>Przykładowy Plan Pobytu</h2>
                    <div class="underline"></div>
                     <p>7 Dni Jesienią (Propozycja - dostosuj do pory i zainteresowań!)</p>
                 </div>
                 <div class="row justify-content-center">
                     <div class="col-lg-9">
                        <div class="accordion" id="itineraryAccordion">
                            <!-- Dzień 1 -->
                            <div class="accordion-item">
                                <h2 class="accordion-header" id="headingOne">
                                    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
                                        <i class="fas fa-plane-arrival fa-fw"></i><strong>Dzień 1: Przylot i Aklimatyzacja</strong>
                                    </button>
                                </h2>
                                <div id="collapseOne" class="accordion-collapse collapse" aria-labelledby="headingOne" data-bs-parent="#itineraryAccordion">
                                    <div class="accordion-body">
                                        <ul class="list-unstyled">
                                            <li><i class="fas fa-plane-departure text-primary me-2"></i>Lot WAW-OSL-LYR.</li>
                                            <li><i class="fas fa-bus text-primary me-2"></i>Transfer do zakwaterowania (Flybussen).</li>
                                            <li><i class="fas fa-bed text-primary me-2"></i>Check-in, krótki odpoczynek.</li>
                                            <li><i class="fas fa-walking text-primary me-2"></i>Spacer orientacyjny po Longyearbyen.</li>
                                            <li><i class="fas fa-utensils text-primary me-2"></i>Kolacja, pierwsze wrażenia arktyczne.</li>
                                        </ul>
                                    </div>
                                 </div>
                            </div>
                            <!-- Dzień 2 -->
                            <div class="accordion-item">
                                <h2 class="accordion-header" id="headingTwo">
                                    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                                        <i class="fas fa-landmark fa-fw"></i><strong>Dzień 2: Historia i Pierwsze Widoki</strong>
                                    </button>
                                </h2>
                                <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#itineraryAccordion">
                                    <div class="accordion-body">
                                        <ul class="list-unstyled">
                                             <li><i class="fas fa-university text-success me-2"></i>Rano: Zwiedzanie <strong class="text-primary">Muzeum Svalbardu</strong> (świetne wprowadzenie!).</li>
                                             <li><i class="fas fa-hiking text-success me-2"></i>Popołudnie: Wycieczka piesza z przewodnikiem (np. na Plateau Mountain dla widoków lub spacer w kierunku Globalnego Banku Nasion).</li>
                                             <li><i class="fas fa-utensils text-success me-2"></i>Wieczór: Kolacja.</li>
                                             <li><i class="fas fa-meteor text-success me-2"></i>(X/XI): Jeśli pogoda pozwoli, wieczorne wyjście na polowanie na zorzę (blisko miasta lub zorganizowana wycieczka).</li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                            <!-- Dzień 3 -->
                             <div class="accordion-item">
                                <h2 class="accordion-header" id="headingThree">
                                     <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                                        <i class="fas fa-dog fa-fw"></i><strong>Dzień 3: Przygoda z Psim Zaprzęgiem</strong>
                                     </button>
                                </h2>
                                <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#itineraryAccordion">
                                     <div class="accordion-body">
                                        <ul class="list-unstyled">
                                             <li><i class="fas fa-paw text-info me-2"></i>Wycieczka psim zaprzęgiem (ok. 4-5 godzin).</li>
                                            <li><i class="fas fa-asterisk text-info me-2"></i>IX/X: Najprawdopodobniej na wózkach na kołach.</li>
                                             <li><i class="fas fa-asterisk text-info me-2"></i>XI (jeśli jest śnieg): Może już na saniach!</li>
                                             <li><i class="fas fa-info-circle text-info me-2"></i>Wizyta w hodowli, instruktaż, przejażdżka przez dolinę (np. Adventdalen), ciepły napój/posiłek.</li>
                                             <li><i class="fas fa-camera text-info me-2"></i>Mnóstwo okazji do zdjęć!</li>
                                             <li><i class="fas fa-utensils text-info me-2"></i>Wieczór: Odpoczynek, kolacja.</li>
                                         </ul>
                                    </div>
                                </div>
                             </div>
                            <!-- Dzień 4 -->
                             <div class="accordion-item">
                                 <h2 class="accordion-header" id="headingFour">
                                     <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="false" aria-controls="collapseFour">
                                        <i class="fas fa-industry fa-fw"></i><strong>Dzień 4: Górnictwo, Kultura i Smaki</strong>
                                     </button>
                                </h2>
                                 <div id="collapseFour" class="accordion-collapse collapse" aria-labelledby="headingFour" data-bs-parent="#itineraryAccordion">
                                    <div class="accordion-body">
                                         <ul class="list-unstyled">
                                             <li><i class="fas fa-pickaxe text-secondary me-2"></i>Rano: Zwiedzanie nieczynnej <strong class="text-primary">Kopalni Węgla nr 3</strong> (fascynujące!).</li>
                                            <li><i class="fas fa-beer text-secondary me-2"></i>Popołudnie: Czas wolny - np. wizyta i degustacja w <strong class="text-primary">Svalbard Bryggeri</strong> (najbardziej na północ wysunięty browar) lub inne muzea/galerie.</li>
                                             <li><i class="fas fa-shopping-bag text-secondary me-2"></i>Okazja na zakup pamiątek.</li>
                                             <li><i class="fas fa-star text-secondary me-2"></i>Wieczór (X/XI): Kolejna szansa na zorzę lub wieczór tematyczny (np. "Wilderness Evening" - sprawdź dostępność).</li>
                                         </ul>
                                    </div>
                                </div>
                             </div>
                             <!-- Dzień 5 -->
                            <div class="accordion-item">
                                <h2 class="accordion-header" id="headingFive">
                                    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFive" aria-expanded="false" aria-controls="collapseFive">
                                        <i class="fas fa-compass fa-fw"></i><strong>Dzień 5: Aktywność Sezonowa</strong>
                                     </button>
                                 </h2>
                                <div id="collapseFive" class="accordion-collapse collapse" aria-labelledby="headingFive" data-bs-parent="#itineraryAccordion">
                                     <div class="accordion-body">
                                         <p>Wybierz aktywność dostosowaną do miesiąca, warunków i zainteresowań:</p>
                                         <ul class="list-unstyled">
                                             <li><i class="fas fa-ship text-warning me-2"></i><strong>IX / Wczesny X:</strong> Rejs statkiem po Isfjordzie (jeśli dostępny i pogoda sprzyja).</li>
                                             <li><i class="fas fa-snowflake text-primary me-2"></i><strong>Późny X / XI:</strong> Wycieczka skuterem śnieżnym (TYLKO jeśli jest wystarczająco śniegu i oferta jest dostępna!).</li>
                                             <li><i class="fas fa-icicles text-info me-2"></i><strong>Późny X / XI:</strong> Eksploracja jaskini lodowej (pieszo lub w połączeniu z inną aktywnością, jeśli dostępne).</li>
                                             <li><i class="fas fa-hiking text-success me-2"></i><strong>Alternatywy (cała jesień):</strong> Dłuższa piesza wędrówka (np. do doliny Bjørndalen), wycieczka fotograficzna.</li>
                                         </ul>
                                    </div>
                                </div>
                            </div>
                             <!-- Dzień 6 -->
                            <div class="accordion-item">
                                <h2 class="accordion-header" id="headingSix">
                                    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSix" aria-expanded="false" aria-controls="collapseSix">
                                        <i class="fas fa-redo-alt fa-fw"></i><strong>Dzień 6: Dzień Elastyczny / Pożegnanie</strong>
                                     </button>
                                 </h2>
                                 <div id="collapseSix" class="accordion-collapse collapse" aria-labelledby="headingSix" data-bs-parent="#itineraryAccordion">
                                     <div class="accordion-body">
                                        <ul class="list-unstyled">
                                            <li><i class="fas fa-question-circle text-warning me-2"></i>Dzień na dodatkowe, ulubione aktywności, relaks lub nadrobienie czegoś, co uniemożliwiła pogoda.</li>
                                            <li><i class="fas fa-camera-retro text-warning me-2"></i>Może krótka wycieczka fotograficzna lub obserwacja ptaków w okolicy?</li>
                                            <li><i class="fas fa-shopping-cart text-warning me-2"></i>Ostatnie zakupy pamiątek.</li>
                                            <li><i class="fas fa-glass-cheers text-warning me-2"></i>Pożegnalna kolacja w jednej z polecanych restauracji (np. Funktionærmessen, Huset, Kroa).</li>
                                        </ul>
                                     </div>
                                 </div>
                            </div>
                            <!-- Dzień 7 -->
                            <div class="accordion-item">
                                <h2 class="accordion-header" id="headingSeven">
                                    <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSeven" aria-expanded="false" aria-controls="collapseSeven">
                                        <i class="fas fa-plane-departure fa-fw"></i><strong>Dzień 7: Powrót do Domu</strong>
                                    </button>
                                </h2>
                                <div id="collapseSeven" class="accordion-collapse collapse" aria-labelledby="headingSeven" data-bs-parent="#itineraryAccordion">
                                    <div class="accordion-body">
                                        <ul class="list-unstyled">
                                            <li><i class="fas fa-briefcase text-danger me-2"></i>Ostatnie pakowanie, ewentualnie szybkie śniadanie.</li>
                                            <li><i class="fas fa-sign-out-alt text-danger me-2"></i>Wykwaterowanie (check-out).</li>
                                            <li><i class="fas fa-bus text-danger me-2"></i>Transfer na lotnisko LYR.</li>
                                            <li><i class="fas fa-home text-danger me-2"></i>Wylot do Warszawy przez Oslo. Koniec arktycznej przygody!</li>
                                        </ul>
                                    </div>
                                </div>
                             </div>
                         </div>
                        <p class="mt-4 text-muted text-center"><small><strong>Pamiętaj:</strong> Dni przylotu i wylotu są mocno ograniczone czasowo. Realnie masz 5 pełnych dni na miejscu. Elastyczność to klucz – pogoda i światło dzienne (lub jego brak) dyktują warunki!</small></p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Budżet Section -->
        <section id="budzet">
            <div class="container" data-aos="fade-up">
                 <div class="section-title">
                    <i class="fas fa-calculator icon"></i>
                    <h2>Budżet Wyprawy</h2>
                    <div class="underline"></div>
                     <p>Szacunkowe Koszty (2 Osoby, 7 Dni, Jesień 2025)</p>
                 </div>
                 <div class="row justify-content-center">
                     <div class="col-lg-10">
                        <p class="text-center mb-4">Svalbard to inwestycja w niezapomniane przeżycia, ale wymaga świadomego planowania finansowego. Poniższe szacunki są orientacyjne (kursy: 1 EUR ≈ 4.3 PLN, 1 NOK ≈ 0.38 PLN).</p>
                         <div class="table-responsive budget-table">
                             <table class="table table-striped table-hover">
                                <thead>
                                    <tr>
                                         <th>Kategoria Wydatków</th>
                                         <th>Niski Budżet (PLN)</th>
                                         <th>Średni Budżet (PLN)</th>
                                        <th>Niski Budżet (EUR)</th>
                                        <th>Średni Budżet (EUR)</th>
                                    </tr>
                                </thead>
                                <tbody>
                                     <tr>
                                         <td><i class="fas fa-plane me-2"></i>Loty (2 os.)</td>
                                        <td>3000 - 4600</td>
                                        <td>4600 - 7000</td>
                                         <td>~700 - 1070</td>
                                         <td>~1070 - 1630</td>
                                    </tr>
                                    <tr>
                                        <td><i class="fas fa-bed me-2"></i>Zakwaterowanie (7 nocy)</td>
                                        <td>2800 - 4200</td>
                                         <td>6600 - 9800</td>
                                        <td>~650 - 980</td>
                                        <td>~1535 - 2280</td>
                                     </tr>
                                    <tr>
                                        <td><i class="fas fa-binoculars me-2"></i>Aktywności (3-4 wycieczki)</td>
                                        <td>3900 - 5200</td>
                                        <td>5850 - 7800</td>
                                         <td>~905 - 1210</td>
                                        <td>~1360 - 1815</td>
                                    </tr>
                                     <tr>
                                        <td><i class="fas fa-utensils me-2"></i>Wyżywienie</td>
                                        <td>1800 - 2800</td>
                                         <td>3600 - 5500</td>
                                         <td>~420 - 650</td>
                                        <td>~840 - 1280</td>
                                    </tr>
                                    <tr>
                                         <td><i class="fas fa-file-medical-alt me-2 text-danger"></i>Ubezpieczenie (arktyczne!)</td>
                                        <td>400 - 700</td>
                                        <td>700 - 1000</td>
                                         <td>~95 - 165</td>
                                        <td>~165 - 235</td>
                                     </tr>
                                     <tr>
                                        <td><i class="fas fa-random me-2"></i>Transport Lokalny / Inne</td>
                                         <td>600 - 1000</td>
                                        <td>1000 - 1500</td>
                                        <td>~140 - 235</td>
                                         <td>~235 - 350</td>
                                     </tr>
                                </tbody>
                                <tfoot>
                                     <tr class="table-dark">
                                        <td><strong>SUMA (2 osoby)</strong></td>
                                         <td><strong>12500 - 18500</strong></td>
                                         <td><strong>22350 - 32600</strong></td>
                                        <td><strong>~2910 - 4310</strong></td>
                                        <td><strong>~5195 - 7590</strong></td>
                                    </tr>
                                    <tr class="table-secondary">
                                        <td><strong>SUMA (na osobę)</strong></td>
                                        <td><strong>6250 - 9250</strong></td>
                                        <td><strong>11175 - 16300</strong></td>
                                         <td><strong>~1455 - 2155</strong></td>
                                         <td><strong>~2598 - 3795</strong></td>
                                     </tr>
                                </tfoot>
                            </table>
                        </div>
                         <p class="mt-4 text-center"><strong>Co wpływa na koszt?</strong> Standard noclegu, liczba i rodzaj aktywności, styl jedzenia (gotowanie vs. restauracje), termin rezerwacji (im wcześniej, tym lepiej!).</p>
                     </div>
                </div>
            </div>
        </section>

        <!-- Przygotowania Section -->
        <section id="przygotowania">
            <div class="container" data-aos="fade-up">
                <div class="section-title">
                     <i class="fas fa-clipboard-check icon"></i>
                     <h2>Przygotowania Końcowe</h2>
                     <div class="underline"></div>
                     <p>Ostatnia prosta przed arktyczną przygodą!</p>
                 </div>
                <div class="row gy-5">
                     <!-- Lewa kolumna: Rezerwacje, Nastawienie -->
                     <div class="col-lg-6">
                         <h3 class="mb-4"><i class="far fa-calendar-alt me-2 text-primary"></i>Harmonogram Rezerwacji</h3>
                        <ul class="list-group list-group-flush bg-transparent">
                            <li class="list-group-item"><i class="fas fa-plane fa-fw"></i><strong>Loty i Noclegi:</strong> Rezerwuj <strong class="text-primary">6-9 miesięcy przed</strong> wyjazdem! To klucz do dobrych cen i dostępności.</li>
                            <li class="list-group-item"><i class="fas fa-ticket-alt fa-fw"></i><strong>Wycieczki:</strong> Najpopularniejsze (psy, skutery - jeśli planujesz i będą dostępne) rezerwuj <strong class="text-primary">2-4 miesiące przed</strong>, zwłaszcza w popularnych terminach.</li>
                        </ul>

                         <h3 class="mt-5 mb-4"><i class="fas fa-snowflake me-2 text-primary"></i>Przyjmij Arktykę Taką, Jaka Jest</h3>
                        <ul class="list-group list-group-flush bg-transparent">
                             <li class="list-group-item"><i class="fas fa-cloud-sun-rain fa-fw"></i>Bądź <strong class="text-primary">elastyczny</strong> – pogoda może pokrzyżować plany. Miej plan B.</li>
                            <li class="list-group-item"><i class="fas fa-paw fa-fw"></i><strong class="text-primary">Szanuj</strong> surową przyrodę, lokalne zasady i ograniczenia.</li>
                            <li class="list-group-item"><i class="far fa-lightbulb fa-fw"></i><strong class="text-primary">Doceniaj</strong> ciszę, przestrzeń i unikalne światło – od złotej jesieni po tajemniczą noc polarną.</li>
                            <li class="list-group-item"><i class="fas fa-user-shield fa-fw"></i>Zaufaj <strong class="text-primary">lokalnym przewodnikom</strong> – ich wiedza i doświadczenie są bezcenne.</li>
                        </ul>
                    </div>
                     <!-- Prawa kolumna: Checklist -->
                     <div class="col-lg-6">
                        <h3 class="mb-4"><i class="fas fa-list-check me-2 text-primary"></i>Lista Kontrolna Przed Wyjazdem</h3>
                        <ul class="list-unstyled checklist">
                             <li><i class="fas fa-check-circle"></i> Zarezerwowane loty WAW-LYR-WAW?</li>
                             <li><i class="fas fa-check-circle"></i> Zarezerwowane zakwaterowanie (7 nocy)?</li>
                            <li><i class="fas fa-check-circle text-danger"></i> Wykupione <strong class="text-danger-emphasis">specjalistyczne ubezpieczenie</strong> (Arktyka + ewakuacja!)?</li>
                             <li><i class="fas fa-check-circle"></i> Przygotowana <strong class="text-primary">odzież warstwowa</strong> i niezbędny ekwipunek (czołówka!)?</li>
                            <li><i class="fas fa-check-circle text-danger"></i> Zapoznane zasady bezpieczeństwa dot. <strong class="text-danger-emphasis">niedźwiedzi polarnych</strong>?</li>
                             <li><i class="fas fa-check-circle"></i> Zarezerwowane 2-4 kluczowe wycieczki?</li>
                             <li><i class="fas fa-check-circle"></i> Przygotowana karta płatnicza (+ew. trochę NOK)?</li>
                             <li><i class="fas fa-check-circle"></i> Sprawdzona ważność paszportu/dowodu?</li>
                        </ul>
                         <div class="alert alert-success mt-5" role="alert">
                             <h4 class="alert-heading"><i class="fas fa-rocket me-2"></i>Gotowi na Start!</h4>
                             <p class="mb-0">Podróż na Svalbard jesienią to wyjątkowe doświadczenie. Staranne planowanie to klucz do bezpiecznej i satysfakcjonującej przygody na krańcu świata. <strong class="text-success">Udanej wyprawy!</strong></p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="mt-auto">
        <div class="container px-4">
            <p>© 2025 Plan Wyprawy na Svalbard by FRN.</p>
        </div>
    </footer>

    <!-- Bootstrap JS Bundle with Popper -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>

    <!-- AOS (Animate On Scroll) JS -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>

    <!-- Custom JS -->
    <script>
        // Initialize AOS
        AOS.init({
            duration: 800, // Animation duration
            easing: 'ease-in-out', // Animation timing function
            once: true, // Animate only once
            offset: 100 // Offset (in px) from the original trigger point
        });

        // Navbar scroll effect
        const navbar = document.getElementById('mainNav');
        const navbarHeight = navbar ? navbar.offsetHeight : 70; // Get navbar height or fallback

        function handleScroll() {
             if (window.scrollY > 50) {
                 navbar.classList.add('scrolled');
            } else {
                 navbar.classList.remove('scrolled');
            }
             // Active link highlighting on scroll
             let scrollPosition = window.scrollY;
             document.querySelectorAll('section[id]').forEach(section => {
                 const sectionTop = section.offsetTop - navbarHeight - 50; // Adjusted for navbar and offset
                 const sectionHeight = section.offsetHeight;
                 const sectionId = section.getAttribute('id');
                 const navLink = document.querySelector(`.navbar-nav .nav-link[href="#${sectionId}"]`);

                 if (scrollPosition >= sectionTop && scrollPosition < sectionTop + sectionHeight) {
                     document.querySelectorAll('.navbar-nav .nav-link').forEach(link => link.classList.remove('active'));
                     if(navLink) navLink.classList.add('active');
                 } else {
                      if(navLink) navLink.classList.remove('active');
                 }
             });
             // Ensure top link is active when at top
             const topLink = document.querySelector('.navbar-nav .nav-link[href="#page-top"]');
              if (scrollPosition < document.querySelector('#intro').offsetTop - navbarHeight - 50) {
                 document.querySelectorAll('.navbar-nav .nav-link').forEach(link => link.classList.remove('active'));
                 // No active link when above intro
             }
        }

        window.addEventListener('scroll', handleScroll);
        document.addEventListener('DOMContentLoaded', handleScroll); // Initial check


        // Smooth scrolling for internal links with class "scroll-link"
         document.querySelectorAll('a.scroll-link[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);

                if (targetElement) {
                    const elementPosition = targetElement.getBoundingClientRect().top;
                    // Use the dynamically calculated navbarHeight
                    const offsetPosition = elementPosition + window.pageYOffset - (navbar.classList.contains('scrolled') ? navbar.offsetHeight : navbarHeight); // Adjust offset based on scrolled state

                    window.scrollTo({
                         top: offsetPosition,
                        behavior: 'smooth'
                    });

                    // Close mobile navbar after click
                     const navbarToggler = document.querySelector('.navbar-toggler');
                    const navbarCollapse = document.querySelector('.navbar-collapse');
                     if (navbarToggler && navbarCollapse.classList.contains('show')) {
                         // Use Bootstrap's Collapse instance to hide
                         var bsCollapse = bootstrap.Collapse.getInstance(navbarCollapse);
                         if (bsCollapse) {
                             bsCollapse.hide();
                         } else {
                              // Fallback if instance not found (shouldn't happen often)
                              navbarCollapse.classList.remove('show');
                         }
                         navbarToggler.classList.add('collapsed'); // Ensure toggler state is correct
                         navbarToggler.setAttribute('aria-expanded', 'false');
                     }
                }
             });
         });

         // Add js class to html tag for styles relying on JS
         document.documentElement.classList.remove('no-js');
         document.documentElement.classList.add('js');

     </script>

</body>
</html>
