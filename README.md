<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Mahfuz Hasan Nasim | Web Developer Portfolio</title>

    <meta name="description"
        content="Mahfuz Hasan Nasim - Diploma in Computer Technology student and Web Development Learner.">

    <meta name="author" content="Mahfuz Hasan Nasim">

    <style>
        /* =========================
           GLOBAL
        ========================== */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        :root {
            --primary: #00d4ff;
            --secondary: #7c3aed;
            --dark: #070b14;
            --dark2: #0d1322;
            --card: #111827;
            --text: #f5f7fa;
            --muted: #aab3c5;
            --border: rgba(255,255,255,0.08);
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: var(--dark);
            color: var(--text);
            line-height: 1.6;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        img {
            max-width: 100%;
            display: block;
        }

        .container {
            width: 90%;
            max-width: 1150px;
            margin: auto;
        }

        .section {
            padding: 90px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 38px;
            margin-bottom: 10px;
        }

        .section-title span {
            color: var(--primary);
        }

        .section-title p {
            color: var(--muted);
        }


        /* =========================
           NAVBAR
        ========================== */

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(7, 11, 20, 0.85);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid var(--border);
        }

        nav {
            height: 70px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
        }

        .logo span {
            color: var(--primary);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 28px;
        }

        .nav-links a {
            color: #dce3ef;
            font-weight: 500;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        .menu-btn {
            display: none;
            font-size: 28px;
            cursor: pointer;
        }


        /* =========================
           HERO
        ========================== */

        #home {
            min-height: 100vh;
            display: flex;
            align-items: center;
            background:
                radial-gradient(circle at 20% 20%, rgba(0,212,255,0.12), transparent 30%),
                radial-gradient(circle at 80% 70%, rgba(124,58,237,0.15), transparent 30%);
        }

        .hero {
            display: grid;
            grid-template-columns: 1.3fr 0.7fr;
            align-items: center;
            gap: 50px;
            padding-top: 70px;
        }

        .hero-text small {
            color: var(--primary);
            font-size: 18px;
            font-weight: bold;
        }

        .hero-text h1 {
            font-size: clamp(42px, 7vw, 75px);
            line-height: 1.1;
            margin: 15px 0;
        }

        .hero-text h1 span {
            color: var(--primary);
        }

        .hero-text h3 {
            color: #d6dbea;
            font-size: 24px;
            margin-bottom: 18px;
        }

        .hero-text p {
            color: var(--muted);
            max-width: 650px;
            font-size: 17px;
        }

        .buttons {
            display: flex;
            gap: 15px;
            margin-top: 30px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 13px 25px;
            border-radius: 8px;
            font-weight: bold;
            border: 1px solid var(--primary);
            transition: 0.3s;
            display: inline-block;
        }

        .btn-primary {
            background: var(--primary);
            color: #001018;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0,212,255,0.25);
        }

        .btn-outline {
            color: var(--primary);
        }

        .btn-outline:hover {
            background: var(--primary);
            color: #001018;
        }

        .hero-card {
            display: flex;
            justify-content: center;
        }

        .profile-circle {
            width: 290px;
            height: 290px;
            border-radius: 50%;
            background:
                linear-gradient(135deg, var(--primary), var(--secondary));
            padding: 7px;
            box-shadow: 0 0 60px rgba(0,212,255,0.2);
        }

        .profile-inner {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background: var(--dark2);
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 30px;
        }

        .profile-inner h2 {
            font-size: 28px;
        }


        /* =========================
           ABOUT
        ========================== */

        #about {
            background: var(--dark2);
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-text h3 {
            font-size: 30px;
            margin-bottom: 18px;
        }

        .about-text h3 span {
            color: var(--primary);
        }

        .about-text p {
            color: var(--muted);
            margin-bottom: 15px;
        }

        .info-box {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }

        .info {
