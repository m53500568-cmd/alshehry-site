<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مكتب هاني بن عبدالله | تعقيب معتمد - استخراج تصاريح زواج، تجنيس، تأشيرات</title>
    <meta name="description" content="مكتب هاني بن عبدالله للتعقيب المعتمد - ننجز جميع المعاملات الحكومية، تصاريح الزواج، التجنيس، التأشيرات، الجوازات السعودية بسرعة واحترافية">
    
    <!-- الروابط الخارجية -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Arabic:wght@300;400;500;600;700;800&family=Tajawal:wght@300;400;500;700&display=swap" rel="stylesheet">
    
    <style>
        /* أنماط متقدمة */
        :root {
            --primary: #1a4722;
            --primary-dark: #0d3515;
            --primary-light: #2d6b3a;
            --secondary: #d4a017;
            --secondary-dark: #b8860b;
            --accent: #e8c547;
            --light: #f8f9fa;
            --dark: #2c3e50;
            --gray: #6c757d;
            --light-gray: #e9ecef;
            --gold-gradient: linear-gradient(135deg, #d4a017 0%, #e8c547 50%, #ffdd70 100%);
            --green-gradient: linear-gradient(135deg, #1a4722 0%, #2d6b3a 50%, #3e8e46 100%);
            --shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            --shadow-lg: 0 20px 50px rgba(0, 0, 0, 0.15);
            --transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            --border-radius: 12px;
            --border-radius-lg: 20px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 100px;
        }

        body {
            font-family: 'Noto Sans Arabic', 'Tajawal', sans-serif;
            color: var(--dark);
            background: #ffffff;
            direction: rtl;
            overflow-x: hidden;
            line-height: 1.8;
        }

        /* تصميم القائمة المتطورة */
        .header-master {
            position: fixed;
            top: 0;
            right: 0;
            left: 0;
            z-index: 9999;
            background: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(26, 71, 34, 0.1);
            transition: var(--transition);
            box-shadow: var(--shadow);
        }

        .header-master.scrolled {
            padding: 10px 0;
            background: rgba(255, 255, 255, 0.98);
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.12);
        }

        .mega-nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }

        .logo-container {
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .official-logo {
            position: relative;
        }

        .official-logo .main-logo {
            font-size: 2.2rem;
            font-weight: 800;
            color: var(--primary);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .official-logo .main-logo i {
            color: var(--secondary);
            font-size: 2.5rem;
        }

        .official-badge {
            position: absolute;
            top: -8px;
            right: -15px;
            background: var(--gold-gradient);
            color: var(--primary-dark);
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.7rem;
            font-weight: 700;
            transform: rotate(5deg);
            box-shadow: 0 4px 10px rgba(212, 160, 23, 0.3);
        }

        /* القائمة الرئيسية */
        .nav-main {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .nav-item {
            position: relative;
        }

        .nav-link {
            color: var(--dark);
            text-decoration: none;
            padding: 12px 20px;
            font-weight: 600;
            font-size: 1rem;
            display: flex;
            align-items: center;
            gap: 8px;
            border-radius: var(--border-radius);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .nav-link:before {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 0;
            height: 3px;
            background: var(--secondary);
            transition: var(--transition);
        }

        .nav-link:hover:before,
        .nav-link.active:before {
            width: 100%;
        }

        .nav-link:hover,
        .nav-link.active {
            color: var(--primary);
            background: rgba(26, 71, 34, 0.05);
        }

        /* القوائم المنسدلة الكبيرة */
        .mega-menu {
            position: absolute;
            top: 100%;
            right: 0;
            width: 800px;
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow-lg);
            padding: 30px;
            opacity: 0;
            visibility: hidden;
            transform: translateY(20px);
            transition: var(--transition);
            z-index: 1000;
            border: 1px solid var(--light-gray);
        }

        .nav-item:hover .mega-menu {
            opacity: 1;
            visibility: visible;
            transform: translateY(0);
        }

        .mega-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
        }

        .mega-column h4 {
            color: var(--primary);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--secondary);
            font-size: 1.2rem;
        }

        .mega-column ul {
            list-style: none;
        }

        .mega-column li {
            margin-bottom: 12px;
        }

        .mega-column a {
            color: var(--dark);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 8px 12px;
            border-radius: 8px;
            transition: var(--transition);
        }

        .mega-column a:hover {
            background: rgba(26, 71, 34, 0.08);
            color: var(--primary);
            transform: translateX(-5px);
        }

        /* أزرار الاتصال */
        .contact-actions {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .whatsapp-master {
            background: var(--gold-gradient);
            color: var(--primary-dark);
            padding: 14px 28px;
            border-radius: var(--border-radius);
            text-decoration: none;
            font-weight: 700;
            font-size: 1.1rem;
            display: flex;
            align-items: center;
            gap: 10px;
            transition: var(--transition);
            box-shadow: 0 6px 20px rgba(212, 160, 23, 0.3);
            position: relative;
            overflow: hidden;
        }

        .whatsapp-master:before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent 30%, rgba(255,255,255,0.3) 50%, transparent 70%);
            transform: translateX(-100%);
            transition: transform 0.6s;
        }

        .whatsapp-master:hover:before {
            transform: translateX(100%);
        }

        .whatsapp-master:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 25px rgba(212, 160, 23, 0.4);
        }

        /* القسم الرئيسي */
        .hero-premium {
            min-height: 100vh;
            background: var(--green-gradient);
            position: relative;
            overflow: hidden;
            display: flex;
            align-items: center;
            padding-top: 100px;
        }

        .hero-premium:before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            bottom: 0;
            left: 0;
            background: url('https://images.unsplash.com/photo-1551135049-8a33b2c16a43?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80') center/cover no-repeat;
            opacity: 0.1;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            color: white;
            padding: 80px 0;
        }

        .hero-badge {
            display: inline-block;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
            padding: 10px 25px;
            border-radius: 50px;
            margin-bottom: 30px;
            border: 1px solid rgba(255, 255, 255, 0.3);
            font-size: 0.9rem;
            letter-spacing: 1px;
        }

        .hero-title {
            font-size: 4rem;
            font-weight: 800;
            margin-bottom: 25px;
            line-height: 1.2;
            text-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .hero-title span {
            color: var(--accent);
            position: relative;
            display: inline-block;
        }

        .hero-title span:after {
            content: '';
            position: absolute;
            bottom: 10px;
            right: 0;
            width: 100%;
            height: 8px;
            background: rgba(232, 197, 71, 0.3);
            z-index: -1;
        }

        .hero-description {
            font-size: 1.4rem;
            max-width: 800px;
            margin-bottom: 40px;
            opacity: 0.95;
            line-height: 1.8;
        }

        /* بطاقات الخدمات */
        .services-master {
            padding: 120px 0;
            background: var(--light);
            position: relative;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
            margin-top: 50px;
        }

        .service-card-premium {
            background: white;
            border-radius: var(--border-radius-lg);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
            border: 1px solid var(--light-gray);
        }

        .service-card-premium:hover {
            transform: translateY(-20px);
            box-shadow: var(--shadow-lg);
            border-color: var(--secondary);
        }

        .service-icon-wrapper {
            height: 200px;
            background: var(--green-gradient);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
        }

        .service-icon-wrapper i {
            font-size: 5rem;
            color: white;
            filter: drop-shadow(0 5px 15px rgba(0,0,0,0.3));
            z-index: 2;
        }

        .service-content {
            padding: 35px;
        }

        .service-title {
            font-size: 1.8rem;
            color: var(--primary);
            margin-bottom: 20px;
            font-weight: 700;
        }

        .service-features {
            list-style: none;
            margin: 25px 0;
        }

        .service-features li {
            padding: 10px 0;
            border-bottom: 1px solid var(--light-gray);
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .service-features li:last-child {
            border-bottom: none;
        }

        .service-features i {
            color: var(--secondary);
            font-size: 1.2rem;
        }

        /* معرض المستندات */
        .documents-gallery {
            padding: 100px 0;
            background: white;
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .document-item {
            position: relative;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            height: 300px;
        }

        .document-item:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: var(--shadow-lg);
        }

        .document-overlay {
            position: absolute;
            bottom: 0;
            right: 0;
            left: 0;
            background: linear-gradient(to top, rgba(26, 71, 34, 0.9), transparent);
            color: white;
            padding: 30px;
            transform: translateY(100%);
            transition: var(--transition);
        }

        .document-item:hover .document-overlay {
            transform: translateY(0);
        }

        /* قسم الإحصائيات */
        .stats-counter {
            padding: 100px 0;
            background: var(--primary-dark);
            color: white;
            position: relative;
            overflow: hidden;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            text-align: center;
        }

        .stat-item {
            position: relative;
            z-index: 2;
        }

        .counter {
            font-size: 4.5rem;
            font-weight: 800;
            color: var(--accent);
            margin-bottom: 15px;
            font-family: 'Tajawal', sans-serif;
        }

        /* قسم الأسئلة */
        .faq-advanced {
            padding: 100px 0;
            background: var(--light);
        }

        .faq-item {
            background: white;
            border-radius: var(--border-radius);
            margin-bottom: 20px;
            overflow: hidden;
            box-shadow: var(--shadow);
            border: 1px solid var(--light-gray);
        }

        .faq-question {
            padding: 25px 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            cursor: pointer;
            font-weight: 600;
            font-size: 1.2rem;
            color: var(--primary);
            transition: var(--transition);
        }

        .faq-question:hover {
            background: rgba(26, 71, 34, 0.05);
        }

        .faq-answer {
            max-height: 0;
            overflow: hidden;
            transition: var(--transition);
            padding: 0 30px;
        }

        .faq-answer.active {
            max-height: 500px;
            padding: 0 30px 30px;
        }

        /* الفوتر المتطور */
        .footer-master {
            background: var(--primary-dark);
            color: white;
            padding-top: 100px;
            position: relative;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 50px;
            margin-bottom: 60px;
        }

        .footer-section {
            position: relative;
        }

        .footer-title {
            color: var(--accent);
            font-size: 1.4rem;
            margin-bottom: 30px;
            padding-bottom: 15px;
            position: relative;
        }

        .footer-title:after {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 60px;
            height: 3px;
            background: var(--secondary);
        }

        .footer-links li {
            margin-bottom: 15px;
        }

        .footer-links a {
            color: #ddd;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 12px;
            transition: var(--transition);
            padding: 8px 0;
        }

        .footer-links a:hover {
            color: var(--accent);
            transform: translateX(-10px);
        }

        .contact-details li {
            display: flex;
            align-items: flex-start;
            gap: 15px;
            margin-bottom: 25px;
        }

        .contact-details i {
            color: var(--accent);
            font-size: 1.3rem;
            margin-top: 5px;
        }

        .footer-bottom {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding: 30px 0;
            text-align: center;
            color: #aaa;
        }

        /* الأزرار العائمة */
        .floating-actions {
            position: fixed;
            bottom: 40px;
            left: 40px;
            z-index: 9998;
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .float-btn {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.8rem;
            box-shadow: var(--shadow-lg);
            transition: var(--transition);
            text-decoration: none;
            position: relative;
        }

        .float-btn.whatsapp {
            background: var(--gold-gradient);
        }

        .float-btn.phone {
            background: var(--green-gradient);
        }

        .float-btn:hover {
            transform: scale(1.1) rotate(10deg);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3);
        }

        /* تأثيرات متقدمة */
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        .floating {
            animation: float 6s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.7; }
        }

        .pulse {
            animation: pulse 2s ease-in-out infinite;
        }

        /* التجاوب */
        @media (max-width: 1200px) {
            .mega-menu {
                width: 700px;
            }
            
            .hero-title {
                font-size: 3.5rem;
            }
        }

        @media (max-width: 992px) {
            .mega-menu {
                width: 600px;
                right: -100px;
            }
            
            .mega-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .hero-title {
                font-size: 3rem;
            }
            
            .nav-main {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block !important;
            }
        }

        @media (max-width: 768px) {
            .hero-title {
                font-size: 2.5rem;
            }
            
            .hero-description {
                font-size: 1.2rem;
            }
            
            .services-grid,
            .gallery-grid,
            .stats-grid,
            .footer-content {
                grid-template-columns: 1fr;
            }
            
            .mega-menu {
                width: calc(100vw - 40px);
                right: 20px;
            }
            
            .floating-actions {
                bottom: 20px;
                left: 20px;
            }
            
            .float-btn {
                width: 60px;
                height: 60px;
                font-size: 1.5rem;
            }
        }

        @media (max-width: 576px) {
            .hero-title {
                font-size: 2rem;
            }
            
            .whatsapp-master {
                padding: 
