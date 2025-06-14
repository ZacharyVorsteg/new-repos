<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Palm Beach Industrial Warehouses - Premium Spaces Available</title>
  <meta name="description" content="Discover prime industrial warehouse spaces in Palm Beach. From 1,000 to 50,000+ sq ft. Expert guidance, immediate availability. Call (561) 718-6725">
  
  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800;900&family=Space+Grotesk:wght@700;900&display=swap" rel="stylesheet">
  
  <style>
    /* --------- GLOBAL STYLES --------- */
    :root {
      --navy: #1a365d;
      --blue: #2b6cb0;
      --teal: #319795;
      --success: #38a169;
      --gray: #f7fafc;
      --white: #ffffff;
      --text-primary: #2d3748;
      --text-secondary: #4a5568;
      --shadow-md: 0 4px 6px rgba(0,0,0,0.1);
      --shadow-lg: 0 10px 15px rgba(0,0,0,0.12);
      --shadow-xl: 0 20px 25px rgba(0,0,0,0.15);
      --primary-font: 'Inter', sans-serif;
      --headline-font: 'Space Grotesk', sans-serif;
      --gradient-hero: linear-gradient(135deg, #1a365d, #2b6cb0);
      --gradient-cta: linear-gradient(120deg, #2b6cb0, #319795);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: var(--primary-font);
      color: var(--text-primary);
      background: var(--gray);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
    }

    a {
      text-decoration: none;
      color: var(--blue);
      transition: color 0.2s ease;
    }
    a:hover {
      color: var(--teal);
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 20px;
    }

    /* --------- ANIMATIONS --------- */
    @keyframes pulse {
      0% { transform: scale(1); box-shadow: 0 0 0 0 rgba(49, 151, 149, 0.4); }
      70% { transform: scale(1.05); box-shadow: 0 0 0 10px rgba(49, 151, 149, 0); }
      100% { transform: scale(1); box-shadow: 0 0 0 0 rgba(49, 151, 149, 0); }
    }

    @keyframes shake {
      0%, 100% { transform: rotate(0deg); }
      10% { transform: rotate(-5deg); }
      20% { transform: rotate(5deg); }
      30% { transform: rotate(-5deg); }
      40% { transform: rotate(5deg); }
      50% { transform: rotate(0deg); }
    }

    @keyframes slideIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes subtlePulse {
      0%, 100% {
        transform: scale(1);
        box-shadow: 0 2px 10px rgba(0,0,0,0.2);
      }
      50% {
        transform: scale(1.02);
        box-shadow: 0 3px 15px rgba(49,151,149,0.3);
      }
    }

    /* --------- HEADER --------- */
    header {
      background: var(--white);
      box-shadow: var(--shadow-md);
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 999;
    }
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 0;
    }
    .logo {
      font-family: var(--headline-font);
      font-size: 1.8rem;
      font-weight: 900;
      color: var(--navy);
      letter-spacing: -0.5px;
    }
    .logo span {
      color: var(--teal);
    }
    .nav-links {
      display: flex;
      gap: 2rem;
      align-items: center;
    }
    .nav-links a {
      font-weight: 600;
      color: var(--text-primary);
      position: relative;
      padding-bottom: 2px;
    }
    .nav-links a::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 0;
      height: 2px;
      background: var(--teal);
      transition: width 0.3s ease;
    }
    .nav-links a:hover::after {
      width: 100%;
    }
    .nav-cta {
      display: flex;
      gap: 1.5rem;
      align-items: center;
    }
    .phone-number {
      font-weight: 700;
      font-size: 1.1rem;
      color: var(--teal);
      transition: transform 0.2s ease;
      white-space: nowrap;
      display: inline-block;
    }
    .phone-number:hover {
      transform: scale(1.05);
    }
    .nav-button {
      background: var(--gradient-cta);
      color: #fff;
      padding: 0.7rem 1.2rem;
      border-radius: 5px;
      font-weight: 700;
      transition: all 0.3s ease;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    .nav-button:hover {
      transform: translateY(-2px);
      box-shadow: 0 4px 8px rgba(0,0,0,0.15);
      color: #fff;
    }

    /* Mobile Menu Toggle */
    .mobile-menu-toggle {
      display: none;
      background: none;
      border: none;
      font-size: 1.5rem;
      cursor: pointer;
      color: var(--navy);
    }

    /* Mobile Menu Overlay */
    .mobile-menu {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.95);
      z-index: 9999;
      display: none;
      opacity: 0;
      transition: opacity 0.3s ease;
    }
    .mobile-menu.active {
      display: block;
      opacity: 1;
    }
    .mobile-menu-content {
      background: var(--white);
      width: 85%;
      max-width: 350px;
      height: 100%;
      position: absolute;
      right: 0;
      top: 0;
      padding: 2rem;
      box-shadow: -5px 0 20px rgba(0,0,0,0.2);
      transform: translateX(100%);
      transition: transform 0.3s ease;
    }
    .mobile-menu.active .mobile-menu-content {
      transform: translateX(0);
    }
    .mobile-menu-close {
      position: absolute;
      top: 1rem;
      right: 1rem;
      background: none;
      border: none;
      font-size: 2rem;
      cursor: pointer;
      color: var(--navy);
      width: 40px;
      height: 40px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      transition: all 0.2s ease;
    }
    .mobile-menu-close:hover {
      background: var(--gray);
    }
    .mobile-menu-links {
      margin-top: 4rem;
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
    }
    .mobile-menu-links a {
      font-size: 1.2rem;
      font-weight: 600;
      color: var(--navy);
      padding: 0.8rem 0;
      border-bottom: 1px solid #e2e8f0;
      transition: all 0.2s ease;
    }
    .mobile-menu-links a:hover {
      color: var(--teal);
      padding-left: 0.5rem;
    }
    .mobile-menu-phone {
      color: var(--teal) !important;
      font-weight: 700;
    }
    .mobile-menu-cta {
      background: var(--gradient-cta);
      color: #fff !important;
      text-align: center;
      padding: 1rem !important;
      border-radius: 5px;
      border: none !important;
      margin-top: 1rem;
    }
    .mobile-menu-cta:hover {
      transform: scale(1.02);
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
    }

    /* --------- HERO --------- */
    .hero {
      background: var(--gradient-hero);
      color: #fff;
      padding: 7rem 0 4rem;
      margin-top: 4.5rem;
    }
    .hero-content {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 3rem;
      align-items: center;
    }
    .hero-text h1 {
      font-family: var(--headline-font);
      font-size: 3rem;
      font-weight: 900;
      margin-bottom: 1rem;
      animation: slideIn 0.6s ease-out;
    }
    .hero-text .highlight {
      color: var(--teal);
    }
    .hero-subtitle {
      font-size: 1.25rem;
      margin-bottom: 1rem;
      opacity: 0.95;
      animation: slideIn 0.8s ease-out;
    }
    .hero-features {
      display: flex;
      gap: 1rem;
      margin-bottom: 2rem;
      flex-wrap: wrap;
      animation: slideIn 1s ease-out;
    }
    .hero-feature {
      display: flex;
      align-items: center;
      font-size: 1.07rem;
    }
    .hero-feature::before {
      content: "✓";
      color: var(--success);
      font-weight: bold;
      margin-right: 0.3em;
    }

    /* --------- CONTACT FORM --------- */
    .contact-form {
      background: #fff;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: var(--shadow-lg);
      animation: slideIn 1.2s ease-out;
    }
    .form-header {
      text-align: center;
      margin-bottom: 1.5rem;
    }
    .form-header h2 {
      font-family: var(--headline-font);
      font-size: 2rem;
      color: var(--navy);
      margin-bottom: 0.5rem;
    }
    .form-subtitle {
      color: var(--text-secondary);
      font-size: 1rem;
    }
    .form-group {
      margin-bottom: 1rem;
    }
    .form-group label {
      display: block;
      margin-bottom: 0.3rem;
      font-weight: 600;
      color: var(--text-primary);
    }
    .form-group input,
    .form-group select,
    .form-group textarea {
      width: 100%;
      padding: 0.8rem;
      border: 2px solid #e2e8f0;
      border-radius: 5px;
      font-size: 1rem;
      font-family: var(--primary-font);
      transition: all 0.3s ease;
    }
    .form-group input:focus,
    .form-group select:focus,
    .form-group textarea:focus {
      outline: none;
      border-color: var(--teal);
      box-shadow: 0 0 0 3px rgba(49,151,149,0.1);
      transform: translateY(-1px);
    }
    .submit-button {
      background: var(--gradient-cta);
      color: #fff;
      border: none;
      padding: 1rem;
      font-weight: 800;
      font-size: 1.05rem;
      border-radius: 5px;
      width: 100%;
      cursor: pointer;
      transition: all 0.3s ease;
      position: relative;
      overflow: hidden;
    }
    .submit-button::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      width: 0;
      height: 0;
      border-radius: 50%;
      background: rgba(255,255,255,0.2);
      transform: translate(-50%, -50%);
      transition: width 0.6s, height 0.6s;
    }
    .submit-button:hover::before {
      width: 300px;
      height: 300px;
    }
    .submit-button:hover {
      transform: translateY(-2px);
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }
    .submit-button:disabled {
      opacity: 0.7;
      cursor: not-allowed;
    }

    .form-disclaimer {
      text-align: center;
      margin-top: 1rem;
      font-size: 0.9rem;
      color: var(--text-secondary);
    }
    .form-disclaimer strong {
      color: var(--teal);
      font-size: 1rem;
    }

    /* --------- PROPERTIES --------- */
    .properties {
      background: var(--gray);
      padding: 5rem 0;
    }
    .section-header {
      text-align: center;
      margin-bottom: 2.5rem;
    }
    .section-header h2 {
      font-family: var(--headline-font);
      font-size: 2.4rem;
      color: var(--navy);
      margin-bottom: 0.5rem;
    }
    .section-header p {
      color: var(--text-secondary);
      font-size: 1.1rem;
    }
    .properties-grid {
      display: grid;
      gap: 2rem;
      grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    }
    .property-card {
      background: #fff;
      border-radius: 8px;
      box-shadow: var(--shadow-md);
      overflow: hidden;
      transition: all 0.3s ease;
      cursor: pointer;
    }
    .property-card:hover {
      transform: translateY(-5px);
      box-shadow: var(--shadow-xl);
    }
    .property-image {
      height: 220px;
      background: #e2e8f0;
      position: relative;
      background-size: cover;
      background-position: center;
      background-color: #e2e8f0;
      overflow: hidden;
    }
    /* Fallback pattern when no image */
    .property-image:not([style*="background-image"]) {
      background-image:
        linear-gradient(45deg, #e2e8f0 25%, transparent 25%, transparent 75%, #e2e8f0 75%, #e2e8f0),
        linear-gradient(45deg, #e2e8f0 25%, transparent 25%, transparent 75%, #e2e8f0 75%, #e2e8f0);
      background-size: 30px 30px;
      background-position: 0 0, 15px 15px;
    }
    .property-image::after {
      content: '🏢 Industrial Space';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: #cbd5e0;
      font-size: 1.2rem;
      font-weight: 600;
      text-align: center;
      opacity: 0.5;
    }
    .property-image[style*="background-image"]::after {
      display: none;
    }
    .property-badge {
      position: absolute;
      top: 1rem;
      left: 1rem;
      background: var(--teal);
      color: #fff;
      padding: 0.4rem 0.8rem;
      border-radius: 4px;
      font-weight: 700;
      font-size: 0.88rem;
      animation: pulse 2s infinite;
    }
    .availability-badge {
      position: absolute;
      bottom: 1rem;
      right: 1rem;
      background: rgba(56, 161, 105, 0.95);
      color: #fff;
      padding: 0.5rem 1rem;
      border-radius: 20px;
      font-weight: 700;
      font-size: 0.85rem;
      box-shadow: 0 2px 10px rgba(0,0,0,0.2);
      animation: slideIn 0.5s ease-out;
      display: flex;
      align-items: center;
      gap: 0.4rem;
      letter-spacing: 0.3px;
    }
    .property-details {
      padding: 1.5rem;
    }
    .property-title {
      font-size: 1.2rem;
      font-weight: 800;
      color: var(--navy);
      margin-bottom: 0.4rem;
    }
    .property-location {
      color: var(--text-secondary);
      margin-bottom: 0.8rem;
    }
    .property-specs {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 0.5rem;
      margin-bottom: 1rem;
    }
    .spec-label {
      font-weight: 600;
      color: var(--navy);
    }
    .spec-value {
      color: var(--text-secondary);
    }
    .property-features {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-bottom: 1rem;
    }
    .feature-tag {
      background: #f7fafc;
      color: var(--text-primary);
      padding: 0.25rem 0.6rem;
      font-size: 0.88rem;
      border-radius: 4px;
      border: 1px solid #e2e8f0;
    }
    .property-cta {
      display: flex;
      gap: 1rem;
    }
    .property-button {
      flex: 1;
      text-align: center;
      font-weight: 700;
      padding: 0.7rem 0;
      border-radius: 5px;
      transition: all 0.2s ease;
      position: relative;
      overflow: hidden;
    }
    .property-button.primary {
      background: var(--blue);
      color: #fff;
    }
    .property-button.primary:hover {
      background: var(--teal);
      color: #fff;
      animation: shake 0.5s ease-in-out;
    }
    .property-button.secondary {
      background: transparent;
      border: 2px solid var(--blue);
      color: var(--blue);
    }
    .property-button.secondary:hover {
      background: var(--blue);
      color: #fff;
    }

    /* --------- BENEFITS --------- */
    .benefits {
      padding: 4rem 0;
      background: #fff;
    }
    .benefits-grid {
      display: grid;
      gap: 2rem;
      grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    }
    .benefit-card {
      text-align: center;
      padding: 1rem 0;
      transition: transform 0.3s ease;
    }
    .benefit-card:hover {
      transform: translateY(-5px);
    }
    .benefit-icon {
      background: #e6f2ff;
      border-radius: 50%;
      width: 70px;
      height: 70px;
      margin: 0 auto 1rem;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      transition: all 0.3s ease;
    }
    .benefit-card:hover .benefit-icon {
      background: var(--gradient-cta);
      transform: scale(1.1);
    }
    .benefit-card h3 {
      font-size: 1.2rem;
      color: var(--navy);
      margin-bottom: 0.5rem;
      font-weight: 700;
    }
    .benefit-card p {
      color: var(--text-secondary);
      font-size: 1rem;
    }

    /* --------- CTA SECTION --------- */
    .cta-section {
      background: var(--gradient-cta);
      color: #fff;
      text-align: center;
      padding: 4rem 0;
    }
    .cta-content h2 {
      font-family: var(--headline-font);
      font-size: 2.4rem;
      margin-bottom: 0.8rem;
      font-weight: 800;
    }
    .cta-phone {
      font-size: 2rem;
      font-weight: 900;
      color: #fff;
      display: inline-block;
      margin-bottom: 0.5rem;
      text-shadow: 0 1px 4px rgba(0,0,0,0.2);
      animation: pulse 2s infinite;
      padding: 0.5rem 1rem;
      border-radius: 30px;
      background: rgba(255,255,255,0.1);
      transition: all 0.3s ease;
    }
    .cta-phone:hover {
      color: #fff;
      transform: scale(1.1);
      background: rgba(255,255,255,0.2);
    }
    .cta-subtext {
      font-size: 1rem;
      opacity: 0.9;
      margin-top: 0.5rem;
    }

    /* --------- BLOG SECTION --------- */
    .blog-section {
      padding: 4rem 0;
      background: #f7fafc;
    }
    .blog-grid {
      display: grid;
      gap: 2rem;
      grid-template-columns: repeat(auto-fit, minmax(330px, 1fr));
    }
    .blog-card {
      background: #fff;
      border-radius: 8px;
      padding: 1.5rem;
      box-shadow: var(--shadow-md);
      transition: all 0.3s ease;
      cursor: pointer;
      position: relative;
      overflow: hidden;
    }
    .blog-card.expanded {
      grid-column: 1 / -1;
      max-width: 800px;
      margin: 0 auto;
      width: 100%;
    }
    .blog-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 3px;
      background: var(--gradient-cta);
      transform: scaleX(0);
      transform-origin: left;
      transition: transform 0.3s ease;
    }
    .blog-card:hover::before {
      transform: scaleX(1);
    }
    .blog-card:hover {
      transform: translateY(-5px);
      box-shadow: var(--shadow-xl);
    }
    .blog-category {
      background: var(--blue);
      color: #fff;
      padding: 0.3rem 0.6rem;
      border-radius: 4px;
      font-size: 0.75rem;
      font-weight: 700;
      display: inline-block;
      margin-bottom: 0.5rem;
    }
    .blog-card h3 {
      font-size: 1.2rem;
      color: var(--navy);
      font-weight: 800;
      margin-bottom: 0.5rem;
      cursor: pointer;
    }
    .blog-excerpt {
      color: var(--text-secondary);
      line-height: 1.5;
      margin-bottom: 0.5rem;
    }
    .blog-meta {
      font-size: 0.85rem;
      color: #6b7280;
      margin-bottom: 0.5rem;
    }
    .blog-link {
      color: var(--teal);
      font-weight: 700;
      transition: all 0.2s;
      display: inline-flex;
      align-items: center;
      gap: 0.3rem;
    }
    .blog-link::after {
      content: '→';
      transition: transform 0.2s;
    }
    .blog-link:hover {
      color: var(--blue);
      gap: 0.5rem;
    }
    .blog-link:hover::after {
      transform: translateX(3px);
    }

    /* Expanded blog content */
    .blog-full-content {
      display: none;
      margin-top: 1.5rem;
      padding-top: 1.5rem;
      border-top: 1px solid #e2e8f0;
      animation: slideIn 0.3s ease-out;
    }
    .blog-card.expanded .blog-full-content {
      display: block;
    }
    .blog-card.expanded .blog-excerpt {
      display: none;
    }
    .blog-card.expanded .blog-link {
      display: none;
    }
    .blog-full-content p {
      color: var(--text-primary);
      line-height: 1.8;
      margin-bottom: 1rem;
    }
    .blog-full-content h3 {
      font-size: 1.3rem;
      color: var(--navy);
      margin: 2rem 0 1rem;
      font-weight: 700;
    }
    .blog-close {
      display: none;
      color: var(--teal);
      font-weight: 700;
      cursor: pointer;
      margin-top: 1rem;
    }
    .blog-card.expanded .blog-close {
      display: inline-flex;
      align-items: center;
      gap: 0.3rem;
    }
    .blog-close::before {
      content: '←';
      transition: transform 0.2s;
    }
    .blog-close:hover {
      color: var(--blue);
    }
    .blog-close:hover::before {
      transform: translateX(-3px);
    }

    .blog-cta {
      background: var(--gradient-hero);
      color: #fff;
      border-radius: 8px;
      padding: 2rem;
      text-align: center;
      margin-top: 2rem;
    }
    .newsletter-form {
      display: flex;
      gap: 1rem;
      margin-top: 1rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }
    .newsletter-form input {
      flex: 1;
      padding: 1rem;
      border: none;
      border-radius: 4px;
      font-size: 1rem;
    }
    .newsletter-form button {
      background: var(--teal);
      color: #fff;
      font-weight: 700;
      border: none;
      border-radius: 4px;
      padding: 1rem 1.5rem;
      cursor: pointer;
      transition: all 0.3s;
    }
    .newsletter-form button:hover {
      background: var(--success);
      transform: translateY(-2px);
    }

    /* --------- FAQ SECTION --------- */
    .faq-section {
      background: #f7fafc;
      padding: 4rem 0;
    }
    .faq-container {
      max-width: 800px;
      margin: 0 auto;
    }
    .faq-item {
      background: #fff;
      border-radius: 8px;
      box-shadow: var(--shadow-md);
      margin-bottom: 1rem;
      overflow: hidden;
      transition: all 0.3s ease;
    }
    .faq-item:hover {
      box-shadow: var(--shadow-lg);
    }
    .faq-question {
      padding: 1.2rem;
      font-weight: 700;
      cursor: pointer;
      display: flex;
      justify-content: space-between;
      align-items: center;
      transition: background 0.2s;
    }
    .faq-question:hover {
      background: #f7fafc;
    }
    .faq-answer {
      display: none;
      padding: 0 1.2rem 1rem;
      color: var(--text-secondary);
      line-height: 1.5;
    }
    .faq-icon {
      transition: transform 0.3s;
      color: var(--teal);
    }

    /* --------- ABOUT SECTION --------- */
    .about-section {
      background: #fff;
      padding: 4rem 0;
    }
    .about-content {
      display: grid;
      gap: 3rem;
      grid-template-columns: 1.5fr 1fr;
      align-items: start;
    }
    .about-text h3 {
      font-family: var(--headline-font);
      font-size: 1.8rem;
      color: var(--navy);
      margin-bottom: 1rem;
      font-weight: 800;
    }
    .about-lead {
      font-size: 1.15rem;
      color: var(--text-secondary);
      margin-bottom: 1.5rem;
      line-height: 1.7;
    }
    .about-text p {
      color: var(--text-primary);
      line-height: 1.7;
      margin-bottom: 1.5rem;
    }
    .about-text ul li {
      color: var(--text-primary);
      line-height: 1.8;
    }
    .about-cta-box {
      background: linear-gradient(135deg, #f7fafc, #e6f2ff);
      border: 1px solid #e2e8f0;
      border-radius: 8px;
      padding: 2.5rem 2rem;
      text-align: center;
      box-shadow: var(--shadow-lg);
      position: sticky;
      top: 100px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .about-cta-box h3 {
      font-size: 1.6rem;
      font-weight: 800;
      color: var(--navy);
      margin-bottom: 0.5rem;
    }
    .about-cta-box p {
      color: var(--text-secondary);
      margin-bottom: 1rem;
      max-width: 280px;
      margin-left: auto;
      margin-right: auto;
    }
    .about-phone {
      display: inline-block;
      font-size: 1.8rem;
      font-weight: 700;
      color: var(--teal);
      margin: 0.5rem 0 0.5rem;
      transition: all 0.3s;
      padding: 0.5rem 1rem;
      border-radius: 30px;
    }
    .about-phone:hover {
      transform: scale(1.1);
      background: var(--teal);
      color: #fff;
    }
    .about-availability {
      color: var(--text-secondary);
      font-size: 0.9rem;
      margin-bottom: 1.5rem;
    }
    .about-features {
      text-align: left;
      margin-bottom: 1rem;
      width: 100%;
      max-width: 250px;
    }
    .about-feature {
      color: var(--text-primary);
      margin-bottom: 0.5rem;
      font-size: 0.95rem;
    }
    .about-cta-box .submit-button {
      width: 100%;
      max-width: 250px;
    }

    /* --------- FOOTER --------- */
    footer {
      background: var(--navy);
      color: #fff;
      padding: 3rem 0 2rem;
      text-align: center;
      position: relative;
    }
    .footer-content h3 {
      font-size: 1.5rem;
      margin-bottom: 1rem;
    }
    .footer-links {
      display: flex;
      justify-content: center;
      gap: 2rem;
      margin-bottom: 2rem;
    }
    .footer-links a {
      color: #fff;
      opacity: 0.8;
      transition: opacity 0.2s;
    }
    .footer-links a:hover {
      opacity: 1;
      color: var(--teal);
    }
    .footer-bottom {
      border-top: 1px solid rgba(255,255,255,0.1);
      margin-top: 2rem;
      padding-top: 2rem;
      font-size: 0.9rem;
      opacity: 0.7;
    }

    /* Terms & Privacy Dropdown */
    .terms-dropdown {
      position: fixed;
      bottom: 0;
      left: 0;
      right: 0;
      background: rgba(0,0,0,0.95);
      backdrop-filter: blur(10px);
      max-height: 70vh;
      overflow-y: auto;
      z-index: 1000;
      animation: slideUp 0.3s ease-out;
    }
    @keyframes slideUp {
      from { transform: translateY(100%); }
      to { transform: translateY(0); }
    }
    .terms-content {
      max-width: 800px;
      margin: 0 auto;
      padding: 2rem;
      color: #fff;
    }
    .terms-content h4 {
      font-size: 1.8rem;
      margin-bottom: 1.5rem;
      color: var(--teal);
    }
    .terms-section {
      margin-bottom: 2rem;
    }
    .terms-section h5 {
      font-size: 1.2rem;
      margin-bottom: 0.8rem;
      color: #fff;
    }
    .terms-section p {
      margin-bottom: 0.8rem;
      line-height: 1.6;
      opacity: 0.9;
    }
    .terms-section ul {
      list-style: none;
      padding: 0;
    }
    .terms-section ul li {
      margin-bottom: 0.5rem;
      padding-left: 1.5rem;
      position: relative;
      line-height: 1.6;
      opacity: 0.9;
    }
    .terms-section ul li::before {
      content: "•";
      position: absolute;
      left: 0;
      color: var(--teal);
    }
    .terms-close {
      background: var(--teal);
      color: #fff;
      border: none;
      padding: 0.8rem 2rem;
      border-radius: 5px;
      font-weight: 700;
      cursor: pointer;
      transition: all 0.3s ease;
      margin-top: 1rem;
    }
    .terms-close:hover {
      background: var(--blue);
      transform: translateY(-2px);
    }

    //* --------- FLOATING CTA --------- */
.floating-cta {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: #10b981;
  color: #fff;
  font-size: 1rem;
  font-weight: 600;
  padding: 0.9rem 1.4rem;
  border-radius: 999px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
  z-index: 9999;
  display: flex;
  align-items: center;
  gap: 0.5rem;
  text-decoration: none;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.floating-cta:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.25);
}



    /* --------- RIPPLE EFFECT --------- */
    .ripple {
      position: absolute;
      background: rgba(255,255,255,0.3);
      border-radius: 50%;
      pointer-events: none;
      animation: rippleEffect 0.6s ease-out;
    }
    @keyframes rippleEffect {
      to {
        transform: scale(4);
        opacity: 0;
      }
    }

    /* --------- RESPONSIVE --------- */
    @media (max-width: 768px) {
      .nav-links {
        display: none;
      }
      .mobile-menu-toggle {
        display: block;
      }
      .nav-cta {
        gap: 0.8rem;
      }
      .phone-number {
        font-size: 0.95rem;
      }
      .nav-button {
        display: none; /* Hide on mobile to save space */
      }
      .hero-content {
        grid-template-columns: 1fr;
        text-align: center;
      }
      .hero-text h1 {
        font-size: 2rem;
      }
      .form-grid {
        grid-template-columns: 1fr;
      }
      .properties-grid {
        grid-template-columns: 1fr;
      }
      .benefits-grid {
        grid-template-columns: 1fr;
      }
      .about-content {
        grid-template-columns: 1fr;
      }
      .about-cta-box {
        position: static;
        margin-top: 2rem;
      }
      .about-stats {
        grid-template-columns: repeat(2, 1fr);
        gap: 1.5rem;
      }
      .footer-links {
        flex-direction: column;
        gap: 0.5rem;
      }
    }
  </style>
</head>
<body>

<!-- FLOATING CTA -->
<a href="tel:+15617186725" class="floating-cta">
  📞 Call Now
</a>


  <!-- HEADER -->
<header>
    <nav class="container">
        <div class="logo">
            <img src="logo.png" alt="Industrial Space" style="height: 55px; margin-right: 14px;">
            <div class="logo-text">
                <span class="logo-main">INDUSTRIAL<span>SPACE</span></span>
                <span class="logo-tagline">Premium Commercial Properties</span>
            </div>
        </div>
        <div class="nav-links">
            <a href="#properties">Properties</a>
            <a href="#about">About</a>
            <a href="#faq">FAQ</a>
        </div>
        <div class="nav-cta">
            <a href="tel:+15617186725" class="phone-number">
                <span class="phone-icon-wrapper">📞</span>
                <span class="phone-text">561-718-6725</span>
            </a>
                            <a href="#hero-form" class="nav-button">Get Available Properties</a>
        </div>
        <button class="mobile-menu-toggle">☰</button>
    </nav>
</header>

<style>
/* Enhanced Header Styles - Add to your existing CSS */
header {
    background: #ffffff;
    box-shadow: 0 2px 10px rgba(0,0,0,0.08);
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
    transition: box-shadow 0.3s ease;
}

header.scrolled {
    box-shadow: 0 4px 20px rgba(0,0,0,0.12);
}

nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 80px;
    gap: 40px;
}

/* Enhanced Logo */
.logo {
    display: flex;
    align-items: center;
    flex-shrink: 0;
    gap: 0;
}

.logo-text {
    display: flex;
    flex-direction: column;
    line-height: 1.1;
}

.logo-main {
    font-size: 1.625rem;
    font-weight: 900;
    color: #1a1f36;
    letter-spacing: -0.02em;
}

.logo-main span {
    color: #2563eb;
    font-weight: 300;
}

.logo-tagline {
    font-size: 0.75rem;
    font-weight: 500;
    color: #64748b;
    margin-top: 2px;
    letter-spacing: 0.02em;
}

/* Enhanced Navigation Links */
.nav-links {
    display: flex;
    gap: 36px;
    flex: 1;
    justify-content: center;
}

.nav-links a {
    color: #475569;
    text-decoration: none;
    font-weight: 500;
    font-size: 1rem;
    transition: color 0.2s;
    position: relative;
}

.nav-links a::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 0;
    height: 2px;
    background: #2563eb;
    transition: width 0.3s ease;
}

.nav-links a:hover {
    color: #1a1f36;
}

.nav-links a:hover::after {
    width: 100%;
}

/* Enhanced CTA Section */
.nav-cta {
    display: flex;
    align-items: center;
    gap: 20px;
    flex-shrink: 0;
}

/* Premium Phone Number */
.phone-number {
    display: flex;
    align-items: center;
    gap: 10px;
    text-decoration: none;
    color: #1a1f36;
    font-weight: 700;
    font-size: 1.125rem;
    transition: all 0.2s;
    position: relative;
}

.phone-icon-wrapper {
    background: #10b981;
    color: white;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    animation: ring 4s ease-in-out infinite;
}

@keyframes ring {
    0%, 100% { transform: rotate(0deg); }
    5%, 15% { transform: rotate(-10deg); }
    10%, 20% { transform: rotate(10deg); }
    25% { transform: rotate(0deg); }
}

.phone-number:hover .phone-text {
    color: #10b981;
}

/* Premium CTA Button */
.nav-button {
    background: #2563eb;
    color: white;
    padding: 14px 28px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 700;
    font-size: 1rem;
    transition: all 0.3s;
    box-shadow: 0 4px 14px rgba(37, 99, 235, 0.25);
    position: relative;
    overflow: hidden;
}

.nav-button::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 0;
    height: 0;
    background: rgba(255,255,255,0.2);
    border-radius: 50%;
    transform: translate(-50%, -50%);
    transition: width 0.6s, height 0.6s;
}

.nav-button:hover::before {
    width: 300px;
    height: 300px;
}

.nav-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(37, 99, 235, 0.35);
}

/* Enhanced Mobile Menu */
.mobile-menu-toggle {
    display: none;
    background: white;
    border: 2px solid #e5e7eb;
    font-size: 1.5rem;
    cursor: pointer;
    padding: 8px 12px;
    border-radius: 8px;
    color: #1a1f36;
    transition: all 0.2s;
}

.mobile-menu-toggle:hover {
    background: #f3f4f6;
    border-color: #d1d5db;
}

/* Responsive Design */
@media (max-width: 768px) {
    nav {
        height: 70px;
    }

    .logo {
        font-size: 1.25rem;
    }

    .logo img {
        height: 45px !important;
    }

    .logo-tagline {
        display: none;
    }

    .nav-links {
        display: none;
    }

    .phone-number {
        font-size: 1rem;
    }

    .phone-icon-wrapper {
        width: 32px;
        height: 32px;
        font-size: 16px;
    }

    .nav-button {
        padding: 12px 20px;
        font-size: 0.9375rem;
    }

    .mobile-menu-toggle {
        display: block;
    }
}

@media (max-width: 480px) {
    .phone-text {
        display: none;
    }

    .nav-button {
        padding: 10px 16px;
        font-size: 0.875rem;
    }
}
</style>

<script>
// Add scroll effect to header
window.addEventListener('scroll', function() {
    const header = document.querySelector('header');
    if (window.scrollY > 50) {
        header.classList.add('scrolled');
    } else {
        header.classList.remove('scrolled');
    }
});

// Smooth scroll for anchor links
document.addEventListener('DOMContentLoaded', function() {
    const links = document.querySelectorAll('a[href^="#"]');
    
    links.forEach(link => {
        link.addEventListener('click', function(e) {
            e.preventDefault();
            
            const targetId = this.getAttribute('href');
            const targetElement = document.querySelector(targetId);
            
            if (targetElement) {
                const headerHeight = document.querySelector('header').offsetHeight;
                const targetPosition = targetElement.offsetTop - headerHeight - 20;
                
                window.scrollTo({
                    top: targetPosition,
                    behavior: 'smooth'
                });
            }
        });
    });
});
</script>

<style>
/* Enhanced Header Styles - Add to your existing CSS */
header {
    background: #ffffff;
    box-shadow: 0 2px 10px rgba(0,0,0,0.08);
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
    transition: box-shadow 0.3s ease;
}

header.scrolled {
    box-shadow: 0 4px 20px rgba(0,0,0,0.12);
}

nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 80px;
    gap: 40px;
}

/* Enhanced Logo */
.logo {
    display: flex;
    align-items: center;
    font-size: 1.5rem;
    font-weight: 900;
    color: #1a1f36;
    letter-spacing: -0.02em;
    position: relative;
    flex-shrink: 0;
}

.logo span {
    color: #2563eb;
    font-weight: 300;
}

.trust-indicator {
    position: absolute;
    bottom: -18px;
    left: 57px;
    font-size: 0.625rem;
    font-weight: 600;
    color: #10b981;
    letter-spacing: 0.05em;
    white-space: nowrap;
}

/* Enhanced Navigation Links */
.nav-links {
    display: flex;
    gap: 36px;
    flex: 1;
    justify-content: center;
}

.nav-links a {
    color: #475569;
    text-decoration: none;
    font-weight: 500;
    font-size: 1rem;
    transition: color 0.2s;
    position: relative;
}

.nav-links a::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 0;
    height: 2px;
    background: #2563eb;
    transition: width 0.3s ease;
}

.nav-links a:hover {
    color: #1a1f36;
}

.nav-links a:hover::after {
    width: 100%;
}

/* Enhanced CTA Section */
.nav-cta {
    display: flex;
    align-items: center;
    gap: 20px;
    flex-shrink: 0;
}

/* Premium Phone Number */
.phone-number {
    display: flex;
    align-items: center;
    gap: 10px;
    text-decoration: none;
    color: #1a1f36;
    font-weight: 700;
    font-size: 1.125rem;
    transition: all 0.2s;
    position: relative;
}

.phone-icon-wrapper {
    background: #10b981;
    color: white;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    animation: ring 4s ease-in-out infinite;
}

@keyframes ring {
    0%, 100% { transform: rotate(0deg); }
    5%, 15% { transform: rotate(-10deg); }
    10%, 20% { transform: rotate(10deg); }
    25% { transform: rotate(0deg); }
}

.phone-number:hover .phone-text {
    color: #10b981;
}

/* Premium CTA Button */
.nav-button {
    background: #2563eb;
    color: white;
    padding: 14px 28px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 700;
    font-size: 1rem;
    transition: all 0.3s;
    box-shadow: 0 4px 14px rgba(37, 99, 235, 0.25);
    position: relative;
    overflow: hidden;
}

.nav-button::before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 0;
    height: 0;
    background: rgba(255,255,255,0.2);
    border-radius: 50%;
    transform: translate(-50%, -50%);
    transition: width 0.6s, height 0.6s;
}

.nav-button:hover::before {
    width: 300px;
    height: 300px;
}

.nav-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(37, 99, 235, 0.35);
}

/* Enhanced Mobile Menu */
.mobile-menu-toggle {
    display: none;
    background: white;
    border: 2px solid #e5e7eb;
    font-size: 1.5rem;
    cursor: pointer;
    padding: 8px 12px;
    border-radius: 8px;
    color: #1a1f36;
    transition: all 0.2s;
}

.mobile-menu-toggle:hover {
    background: #f3f4f6;
    border-color: #d1d5db;
}

/* Responsive Design */
@media (max-width: 768px) {
    nav {
        height: 70px;
    }

    .logo {
        font-size: 1.25rem;
    }

    .logo img {
        height: 35px !important;
    }

    .trust-indicator {
        display: none;
    }

    .nav-links {
        display: none;
    }

    .phone-number {
        font-size: 1rem;
    }

    .phone-icon-wrapper {
        width: 32px;
        height: 32px;
        font-size: 16px;
    }

    .nav-button {
        padding: 12px 20px;
        font-size: 0.9375rem;
    }

    .mobile-menu-toggle {
        display: block;
    }
}

@media (max-width: 480px) {
    .phone-text {
        display: none;
    }

    .nav-button {
        padding: 10px 16px;
        font-size: 0.875rem;
    }
}
</style>

<script>
// Add scroll effect to header
window.addEventListener('scroll', function() {
    const header = document.querySelector('header');
    if (window.scrollY > 50) {
        header.classList.add('scrolled');
    } else {
        header.classList.remove('scrolled');
    }
});
</script>

  <!-- HERO SECTION -->
<section class="hero">
    <div class="container">
        <div class="hero-content">
            <div class="hero-text">
                <!-- Trust Badge -->
                <div class="alert-badge">
                    <span class="pulse"></span>
                    LIMITED AVAILABILITY – Tour Today
                </div>

                <h1>
                    Get The <span class="highlight">Industrial Space</span> 
                    You Need <span class="underline">This Week</span>
                </h1>
                
                <p class="hero-subtitle">
                    Skip the waiting lists. View available properties now in Palm Beach County.
                    <strong>Move in as fast as 48 hours.</strong>
                </p>

                <!-- Enhanced Features -->
                <div class="hero-features">
                    <div class="hero-feature">
                        <span class="icon">✓</span>
                        <div>
                            <strong>1,000 - 50,000+ sq ft</strong>
                            <span>Perfect size for your business</span>
                        </div>
                    </div>
                    <div class="hero-feature">
                        <span class="icon">✓</span>
                        <div>
                            <strong>Move-in Ready NOW</strong>
                            <span>No construction delays</span>
                        </div>
                    </div>
                    <div class="hero-feature">
                        <span class="icon">✓</span>
                        <div>
                            <strong>Flexible Terms</strong>
                            <span>Month-to-month available</span>
                        </div>
                    </div>
                </div>

                <!-- Mobile CTA (hidden on desktop) -->
                <div class="mobile-cta">
                    <a href="#hero-form" class="btn-primary-mobile">
                        See Available Properties
                        <svg viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"/>
                        </svg>
                    </a>
                    <div class="or-text">or call</div>
                    <a href="tel:+15617186725" class="phone-button-mobile">
                        <span class="phone-icon">📞</span>
                        <span>561-718-6725</span>
                    </a>
                </div>

                <!-- Desktop Trust Signals -->
                <div class="trust-signals">
                    <div class="trust-item">
                        <svg viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"/>
                        </svg>
                        Licensed Agent
                    </div>
                    <div class="trust-item">
                        <svg viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z"/>
                        </svg>
                        Same-Day Tours
                    </div>
                    <div class="trust-item">
                        <svg viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10 2a1 1 0 00-.894.553L7.382 6H4a1 1 0 000 2v10a2 2 0 002 2h8a2 2 0 002-2V8a1 1 0 100-2h-3.382l-1.724-3.447A1 1 0 0010 2zM6 8h8v10H6V8z"/>
                        </svg>
                        All Properties Verified
                    </div>
                </div>
            </div>

            <!-- MAIN CONTACT FORM -->
            <div class="contact-form" id="hero-form">
                <div class="form-header">
                    <h2>Schedule Your Tour</h2>
                    <p class="form-subtitle">Get exclusive access to pre-market deals</p>
                </div>
                
                <!-- NETLIFY FORM -->
                <form id="propertyInquiry" 
                      name="propertyInquiry" 
                      method="POST" 
                      data-netlify="true"
                      netlify-honeypot="bot-field">
                    
                    <!-- Hidden fields for Netlify -->
                    <input type="hidden" name="form-name" value="propertyInquiry">
                    <div style="display:none">
                        <label>Don't fill this out: <input name="bot-field"></label>
                    </div>
                    
                    <div class="form-group">
                        <input type="text" id="name" name="name" placeholder="Full Name *" required>
                    </div>
                    
                    <div class="form-group">
                        <input type="email" id="email" name="email" placeholder="Email Address *" required>
                    </div>
                    
                    <div class="form-group">
                        <input type="tel" id="phone" name="phone" placeholder="Phone Number *" required>
                    </div>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <select id="spaceSize" name="spaceSize" required>
                                <option value="">Space Size Needed *</option>
                                <option value="1000-2500">1,000 - 2,500 sq ft</option>
                                <option value="2500-5000">2,500 - 5,000 sq ft</option>
                                <option value="5000-10000">5,000 - 10,000 sq ft</option>
                                <option value="10000+">10,000+ sq ft</option>
                            </select>
                        </div>
                        
                        <div class="form-group">
                            <select id="budget" name="budget" required>
                                <option value="">Monthly Budget *</option>
                                <option value="under-2000">Under $2,000</option>
                                <option value="2000-5000">$2,000 - $5,000</option>
                                <option value="5000-10000">$5,000 - $10,000</option>
                                <option value="10000+">$10,000+</option>
                            </select>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <select id="propertyUse" name="propertyUse" required>
                            <option value="">Intended Property Use *</option>
                            <option value="warehouse">Warehouse/Storage</option>
                            <option value="manufacturing">Manufacturing</option>
                            <option value="distribution">Distribution Center</option>
                            <option value="flex">Flex Space (Office + Warehouse)</option>
                            <option value="showroom">Showroom</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <select id="moveInDate" name="moveInDate" required>
                            <option value="">Desired Move-in Date *</option>
                            <option value="asap">ASAP (Within 1 week)</option>
                            <option value="2-weeks">Within 2 weeks</option>
                            <option value="1-month">Within 1 month</option>
                            <option value="2-months">Within 2 months</option>
                            <option value="flexible">Flexible</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <textarea id="message" name="message" rows="2" 
                                  placeholder="Special requirements? (Loading docks, office space, parking, etc.)"></textarea>
                    </div>
                    
                    <button type="submit" class="submit-button">
                        <span class="button-text-desktop">GET PROPERTY LIST & SCHEDULE TOUR</span>
                        <span class="button-text-mobile">GET PROPERTIES</span>
                        <svg viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"/>
                        </svg>
                    </button>
                    
                    <div class="form-disclaimer">
                        <svg viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"/>
                        </svg>
                        <span><strong>Your information is secure</strong><br>
                        Immediate response within business hours</span>
                    </div>
                </form>
                
                <p class="agent-info">
                    Operated by Zachary Vorsteg, Licensed Agent with Cornerstone Realty (SL3603483).
                </p>
            </div>
        </div>
    </div>
</section>

<style>
/* Hero Section Base */
.hero {
    background: linear-gradient(135deg, #1a1f36 0%, #2d3748 100%);
    color: white;
    padding: 100px 0 60px;
    position: relative;
    overflow: hidden;
}

.hero::after {
    content: '';
    position: absolute;
    top: 0;
    right: -300px;
    width: 600px;
    height: 600px;
    background: radial-gradient(circle, rgba(59, 130, 246, 0.08) 0%, transparent 70%);
    border-radius: 50%;
}

.container {
    max-width: 1400px;
    margin: 0 auto;
    padding: 0 24px;
    position: relative;
    z-index: 1;
    width: 100%;
}

/* Hero Content Layout */
.hero-content {
    display: grid;
    grid-template-columns: 1fr 420px;
    gap: 60px;
    align-items: start;
}

@media (min-width: 1025px) {
    .hero-content {
        grid-template-columns: 1fr 420px;
    }
}

/* Alert Badge */
.alert-badge {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: rgba(239, 68, 68, 0.1);
    border: 1px solid #ef4444;
    padding: 10px 20px;
    border-radius: 30px;
    margin-bottom: 28px;
    font-size: 0.875rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: #fecaca;
}

.pulse {
    width: 6px;
    height: 6px;
    background: #ef4444;
    border-radius: 50%;
    animation: pulse 2s infinite;
}

@keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 1; }
    50% { transform: scale(1.5); opacity: 0.6; }
}

/* Typography */
h1 {
    font-size: clamp(1.875rem, 4vw, 2.75rem);
    font-weight: 800;
    line-height: 1.1;
    margin-bottom: 16px;
    letter-spacing: -0.02em;
}

.highlight {
    background: linear-gradient(135deg, #60a5fa 0%, #3b82f6 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.underline {
    position: relative;
}

.underline::after {
    content: '';
    position: absolute;
    bottom: 2px;
    left: 0;
    right: 0;
    height: 3px;
    background: #fbbf24;
    transform: scaleX(0.8);
}

.hero-subtitle {
    font-size: 1.125rem;
    line-height: 1.6;
    color: rgba(255, 255, 255, 0.9);
    margin-bottom: 24px;
    max-width: 600px;
}

.hero-subtitle strong {
    color: #fbbf24;
    font-weight: 700;
}

/* Hero Features */
.hero-features {
    display: flex;
    flex-direction: column;
    gap: 14px;
    margin-bottom: 36px;
}

.hero-feature {
    display: flex;
    align-items: center;
    gap: 16px;
    padding: 14px 20px;
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 10px;
    backdrop-filter: blur(10px);
    transition: all 0.3s;
}

.hero-feature:hover {
    background: rgba(255, 255, 255, 0.08);
    border-color: rgba(255, 255, 255, 0.2);
    transform: translateX(4px);
}

.hero-feature .icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 26px;
    height: 26px;
    background: #10b981;
    color: white;
    border-radius: 50%;
    font-weight: 700;
    flex-shrink: 0;
    font-size: 0.875rem;
}

.hero-feature div {
    display: flex;
    flex-direction: column;
    gap: 2px;
}

.hero-feature strong {
    font-size: 1.0625rem;
    color: white;
}

.hero-feature span {
    font-size: 0.875rem;
    color: rgba(255, 255, 255, 0.7);
}

/* Mobile CTA (hidden on desktop) */
.mobile-cta {
    display: none;
}

/* Trust Signals */
.trust-signals {
    display: flex;
    gap: 28px;
    padding-top: 28px;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    flex-wrap: wrap;
}

.trust-item {
    display: flex;
    align-items: center;
    gap: 10px;
    color: rgba(255, 255, 255, 0.8);
    font-size: 0.9375rem;
    font-weight: 500;
}

.trust-item svg {
    width: 20px;
    height: 20px;
    color: #60a5fa;
    flex-shrink: 0;
}

/* Contact Form Styles */
.contact-form {
    background: white;
    border-radius: 16px;
    padding: 32px;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
}

.form-header {
    text-align: center;
    margin-bottom: 28px;
}

.form-header h2 {
    color: #1a1f36;
    font-size: 1.625rem;
    font-weight: 800;
    margin-bottom: 6px;
}

.form-subtitle {
    color: #64748b;
    font-size: 0.9375rem;
}

/* Form Layout */
.form-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 14px;
}

.form-group {
    margin-bottom: 14px;
}

.form-group input,
.form-group select,
.form-group textarea {
    width: 100%;
    padding: 14px;
    border: 2px solid #e5e7eb;
    border-radius: 8px;
    font-size: 0.9375rem;
    transition: all 0.3s;
    background: #f9fafb;
    font-family: inherit;
}

.form-group input:focus,
.form-group select:focus,
.form-group textarea:focus {
    outline: none;
    border-color: #3b82f6;
    background: white;
    box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.1);
}

.form-group select {
    cursor: pointer;
}

/* Submit Button */
.submit-button {
    width: 100%;
    background: #3b82f6;
    color: white;
    padding: 16px 20px;
    border: none;
    border-radius: 10px;
    font-size: 1rem;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.3s;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    margin-top: 20px;
    font-family: inherit;
}

.submit-button:hover {
    background: #2563eb;
    transform: translateY(-2px);
    box-shadow: 0 10px 25px rgba(59, 130, 246, 0.3);
}

.submit-button svg {
    width: 18px;
    height: 18px;
}

.button-text-mobile {
    display: none;
}

@media (max-width: 580px) {
    .button-text-desktop {
        display: none;
    }
    .button-text-mobile {
        display: inline;
    }
}

/* Form Disclaimer */
.form-disclaimer {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-top: 16px;
    padding: 14px;
    background: #f0f9ff;
    border-radius: 8px;
    font-size: 0.8125rem;
    color: #0c4a6e;
}

.form-disclaimer svg {
    width: 18px;
    height: 18px;
    color: #0284c7;
    flex-shrink: 0;
}

.agent-info {
    font-size: 0.75rem;
    color: #64748b;
    text-align: center;
    margin-top: 14px;
    line-height: 1.4;
}

/* Responsive Design */
@media (max-width: 1200px) {
    .hero-content {
        grid-template-columns: 1fr 380px;
        gap: 40px;
    }
    
    .contact-form {
        padding: 20px;
    }
}

@media (max-width: 1024px) {
    .hero {
        padding: 80px 0 30px;
    }
    
    .hero-content {
        grid-template-columns: 1fr;
        gap: 36px;
    }

    .contact-form {
        max-width: 460px;
        margin: 0 auto;
    }
}

@media (max-width: 768px) {
    .hero {
        padding: 70px 0 40px;
    }

    .hero-content {
        grid-template-columns: 1fr;
    }

    h1 {
        font-size: 1.875rem;
    }

    .hero-subtitle {
        font-size: 1rem;
        margin-bottom: 24px;
    }

    .hero-features {
        margin-bottom: 24px;
        gap: 10px;
    }
    
    .hero-feature {
        padding: 10px 14px;
    }

    /* Show mobile CTA */
    .mobile-cta {
        display: flex;
        flex-direction: column;
        gap: 10px;
        margin-bottom: 24px;
    }

    .btn-primary-mobile {
        background: #fbbf24;
        color: #1a1f36;
        padding: 12px 18px;
        border-radius: 8px;
        font-weight: 700;
        font-size: 0.9375rem;
        text-decoration: none;
        display: inline-flex;
        align-items: center;
        justify-content: center;
        gap: 8px;
        box-shadow: 0 4px 20px rgba(251, 191, 36, 0.3);
    }

    .btn-primary-mobile svg {
        width: 16px;
        height: 16px;
    }

    .or-text {
        text-align: center;
        color: rgba(255, 255, 255, 0.6);
        font-size: 0.75rem;
    }

    .phone-button-mobile {
        background: white;
        color: #1a1f36;
        padding: 10px 16px;
        border-radius: 8px;
        text-decoration: none;
        display: inline-flex;
        align-items: center;
        justify-content: center;
        gap: 8px;
        font-weight: 700;
        font-size: 0.9375rem;
    }

    .phone-icon {
        font-size: 1rem;
    }

    .trust-signals {
        gap: 16px;
        margin-bottom: 32px;
    }

    .trust-item {
        font-size: 0.75rem;
    }

    .contact-form {
        padding: 24px;
        max-width: 100%;
    }

    .form-row {
        grid-template-columns: 1fr;
    }

    .form-header h2 {
        font-size: 1.25rem;
    }
    
    .form-subtitle {
        font-size: 0.8125rem;
    }

    .submit-button {
        font-size: 0.875rem;
        padding: 12px 16px;
    }
}

@media (max-width: 480px) {
    .hero {
        padding: 60px 0 30px;
    }

    .container {
        padding: 0 16px;
    }

    h1 {
        font-size: 1.625rem;
        margin-bottom: 16px;
    }
    
    .hero-subtitle {
        font-size: 0.9375rem;
        margin-bottom: 24px;
    }
    
    .alert-badge {
        font-size: 0.75rem;
        padding: 6px 14px;
        margin-bottom: 20px;
    }

    .hero-feature {
        padding: 10px 14px;
    }
    
    .hero-feature strong {
        font-size: 0.9375rem;
    }
    
    .hero-feature span {
        font-size: 0.75rem;
    }

    .trust-signals {
        flex-direction: column;
        align-items: center;
        gap: 12px;
    }

    .contact-form {
        padding: 24px 18px;
        border-radius: 12px;
    }
    
    .form-header h2 {
        font-size: 1.375rem;
    }

    .form-group input,
    .form-group select,
    .form-group textarea {
        padding: 12px;
        font-size: 0.875rem;
    }
    
    .form-disclaimer {
        font-size: 0.75rem;
        padding: 12px;
    }
    
    .agent-info {
        font-size: 0.6875rem;
    }
}

/* Very small screens */
@media (max-width: 360px) {
    h1 {
        font-size: 1.5rem;
    }
    
    .hero-feature {
        flex-direction: column;
        text-align: center;
        gap: 8px;
    }
    
    .submit-button {
        font-size: 0.875rem;
    }
}
</style>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Available Properties - Optimized</title>
    <style>
        /* Reset and Base Variables */
        * { margin: 0; padding: 0; box-sizing: border-box; }

        :root {
            --primary: #1a1f36;
            --accent: #4a69ff;
            --success: #00d4aa;
            --warning: #ff6b35;
            --text-primary: #1a1f36;
            --text-secondary: #6b7280;
            --bg-primary: #fff;
            --bg-secondary: #f8fafc;
            --border: #e5e7eb;
            --shadow: 0 4px 6px -1px rgba(0,0,0,0.1);
            --radius: 16px;
            --transition: all 0.2s ease;
        }

        /* Base Styles */
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: var(--bg-secondary);
            color: var(--text-primary);
            line-height: 1.6;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 40px 20px 60px;
        }

        /* Typography */
        .section-header { text-align: center; margin-bottom: 3rem; }
        .section-header h2 {
            font-size: clamp(1.75rem, 4vw, 2.5rem);
            font-weight: 800;
            margin-bottom: 1rem;
            background: linear-gradient(135deg, var(--primary) 0%, var(--accent) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .section-header p {
            font-size: 1.125rem;
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto;
        }

        /* Shared Component Styles */
        .card {
            background: var(--bg-primary);
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            overflow: hidden;
        }

        .input-field {
            width: 100%;
            height: 44px;
            padding: 0 1rem;
            border: 2px solid var(--border);
            border-radius: 8px;
            font-size: 0.9375rem;
            transition: var(--transition);
            background: var(--bg-primary);
        }

        .input-field:focus {
            outline: none;
            border-color: var(--accent);
            box-shadow: 0 0 0 3px rgba(74, 105, 255, 0.1);
        }

        .btn {
            padding: 14px 20px;
            border-radius: 10px;
            font-weight: 700;
            transition: var(--transition);
            border: 2px solid transparent;
            text-align: center;
            text-decoration: none;
            cursor: pointer;
            font-size: 0.9375rem;
        }

        .btn-primary {
            background: var(--success);
            color: white;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow);
        }

        .btn-secondary {
            background: transparent;
            color: var(--accent);
            border-color: var(--accent);
        }

        .btn-secondary:hover {
            background: var(--accent);
            color: white;
        }

        /* Filter Section */
        .filter-section {
            padding: 28px;
            margin-bottom: 2.25rem;
        }

        .filter-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .filter-group label {
            display: block;
            font-size: 0.75rem;
            font-weight: 600;
            color: var(--text-secondary);
            margin-bottom: 0.5rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
        }

        /* Results Bar */
        .results-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 1rem;
            padding: 20px 24px;
            margin-bottom: 2rem;
        }

        .results-count strong { color: var(--accent); }

        .contact-info {
            color: var(--text-secondary);
            font-size: 0.875rem;
        }

        .contact-info a {
            color: var(--accent);
            text-decoration: none;
            font-weight: 600;
            margin-left: 0.5rem;
        }

        /* Property Grid */
        .properties-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(min(100%, 380px), 1fr));
            gap: 24px;
            margin-bottom: 3rem;
        }

        /* Property Card */
        .property-card {
            display: flex;
            flex-direction: column;
            height: 100%;
            transition: var(--transition);
            border: 2px solid transparent;
            position: relative;
        }

        .property-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 20px 25px -5px rgba(0,0,0,0.1);
            border-color: var(--accent);
        }

        .property-image {
            position: relative;
            height: 220px;
            background: linear-gradient(135deg, #e0e7ff 0%, #c7d2fe 100%);
            background-size: cover;
            background-position: center;
        }

        .badge {
            position: absolute;
            border-radius: 15px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 0.03em;
        }

        .badge-type {
            top: 12px;
            left: 12px;
            padding: 4px 10px;
            font-size: 0.5rem;
            background: var(--primary);
            color: white;
        }

        .badge-status {
            top: 12px;
            right: 12px;
            padding: 3px 8px;
            font-size: 0.5rem;
            background: var(--success);
            color: white;
        }

        .property-content {
            flex: 1;
            display: flex;
            flex-direction: column;
            padding: 24px;
            gap: 1rem;
        }

        .property-title {
            font-size: 1.375rem;
            font-weight: 700;
            line-height: 1.3;
        }

        .property-location {
            color: var(--text-secondary);
            font-size: 0.9375rem;
            padding-left: 1.25rem;
            position: relative;
        }

        .property-location::before {
            content: "📍";
            position: absolute;
            left: 0;
        }

        .property-specs {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1rem;
            padding: 1rem;
            background: var(--bg-secondary);
            border-radius: 12px;
        }

        .spec-item {
            font-size: 0.9375rem;
        }

        .spec-label {
            color: var(--text-secondary);
            font-weight: 500;
        }

        .spec-value {
            color: var(--text-primary);
            font-weight: 600;
        }

        .property-features {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            min-height: 52px;
        }

        .feature-tag {
            background: rgba(74, 105, 255, 0.1);
            color: var(--accent);
            padding: 6px 12px;
            border-radius: 6px;
            font-size: 0.8125rem;
            font-weight: 500;
            white-space: nowrap;
        }

        .property-actions {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 12px;
            margin-top: auto;
        }

        /* No Results */
        .no-results {
            text-align: center;
            padding: 80px 20px;
        }

        .no-results h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .no-results p {
            color: var(--text-secondary);
            margin-bottom: 1.5rem;
        }

        /* Loading State */
        .skeleton {
            background: linear-gradient(90deg, #f0f0f0 25%, #e0e0e0 50%, #f0f0f0 75%);
            background-size: 200% 100%;
            animation: loading 1.5s infinite;
        }

        @keyframes loading {
            0% { background-position: 200% 0; }
            100% { background-position: -200% 0; }
        }

        /* Responsive */
        @media (max-width: 768px) {
            .container { padding: 40px 16px 60px; }
            .filter-grid { grid-template-columns: 1fr; }
            .results-bar { text-align: center; }
            .property-specs { grid-template-columns: 1fr; }
            .property-actions { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>
    <section class="properties" id="properties">
        <div class="container">
            <div class="section-header">
                <h2>Currently Available Properties</h2>
                <p>Professional industrial spaces ready for immediate occupancy</p>
            </div>

            <!-- Filters -->
            <div class="filter-section card">
                <form id="filterForm" class="filter-grid">
                    <div class="filter-group">
                        <label for="search">Quick Search</label>
                        <input type="text" id="search" class="input-field" placeholder="Location, size, or features...">
                    </div>
                    
                    <div class="filter-group">
                        <label for="type">Property Type</label>
                        <select id="type" class="input-field">
                            <option value="">All Types</option>
                            <option value="warehouse">Warehouse</option>
                            <option value="office">Office</option>
                            <option value="flex">Flex Space</option>
                            <option value="land">Land</option>
                        </select>
                    </div>

                    <div class="filter-group">
                        <label for="size">Size Range</label>
                        <select id="size" class="input-field">
                            <option value="">Any Size</option>
                            <option value="0-1000">Under 1,000 SF</option>
                            <option value="1000-3000">1,000 - 3,000 SF</option>
                            <option value="3000-5000">3,000 - 5,000 SF</option>
                            <option value="5000+">5,000+ SF</option>
                        </select>
                    </div>

                    <div class="filter-group">
                        <label for="price">Monthly Budget</label>
                        <select id="price" class="input-field">
                            <option value="">Any Budget</option>
                            <option value="0-2000">Under $2,000</option>
                            <option value="2000-5000">$2,000 - $5,000</option>
                            <option value="5000-10000">$5,000 - $10,000</option>
                            <option value="10000+">$10,000+</option>
                        </select>
                    </div>

                    <div class="filter-group">
                        <label for="sort">Sort By</label>
                        <select id="sort" class="input-field">
                            <option value="featured">Featured First</option>
                            <option value="price-low">Lowest Price</option>
                            <option value="price-high">Highest Price</option>
                            <option value="size-low">Smallest First</option>
                            <option value="size-high">Largest First</option>
                        </select>
                    </div>
                </form>
            </div>

            <!-- Results Bar -->
            <div class="results-bar card">
                <div class="results-count">
                    Showing <strong id="resultCount">0</strong> properties
                </div>
                <div class="contact-info">
                    Need assistance?
                    <a href="tel:+15617186725">(561) 718-6725</a>
                </div>
            </div>

            <!-- Properties Grid -->
            <div class="properties-grid" id="propertiesGrid"></div>

            <!-- No Results -->
            <div class="no-results card" id="noResults" style="display: none;">
                <h3>No properties match your criteria</h3>
                <p>Try adjusting your filters or contact us for personalized assistance</p>
                <a href="tel:+15617186725" class="btn btn-primary" style="display: inline-block;">
                    Call for More Options
                </a>
            </div>
        </div>
    </section>

    <script>
        // Optimized Property Management System
        class PropertyManager {
            constructor() {
                this.properties = [];
                this.filteredProperties = [];
                this.filters = {
                    search: '',
                    type: '',
                    size: '',
                    price: '',
                    sort: 'featured'
                };
                this.init();
            }

            init() {
                this.loadProperties();
                this.setupEventListeners();
                this.render();
            }

            loadProperties() {
                // In production, this would be an API call
                this.properties = [
                    {
                        id: 1,
                        title: "Small Bay Warehouse",
                        location: "Near I-95 & Belvedere",
                        type: "warehouse",
                        size: 1250,
                        sizeUnit: "SF",
                        clearHeight: "16'",
                        monthlyRent: 2395.83,
                        ratePSF: 23.00,
                        features: ["10×12 Roll-up Door", "Concrete Building", "Restroom", "Industrial Gross"],
                        image: "property1.jpg",
                        available: true
                    },
                    {
                        id: 2,
                        title: "Agricultural Land",
                        location: "West Palm Beach",
                        type: "land",
                        size: 0.5,
                        sizeUnit: "Acres",
                        monthlyRent: null,
                        features: ["Private", "Filled Land", "Gated Access", "Camera Surveillance"],
                        image: "property2.jpg",
                        available: true,
                        additionalInfo: { security: "24/7 Cameras", management: "On-Site" }
                    },
                    {
                        id: 3,
                        title: "Prime Corner Warehouse",
                        location: "Southern Blvd",
                        type: "warehouse",
                        size: 3600,
                        sizeUnit: "SF",
                        clearHeight: "16'",
                        monthlyRent: 7050.00,
                        ratePSF: 23.50,
                        features: ["200 SF A/C Office", "(2) 10×12 Doors", "Grade Level", "Near Turnpike"],
                        image: "property3.jpg",
                        available: true
                    },
                    {
                        id: 4,
                        title: "Free-Standing Flex Industrial Building",
                        location: "West Palm Beach",
                        type: "flex",
                        size: 11400,
                        sizeUnit: "SF",
                        clearHeight: "18-20'",
                        monthlyRent: 23987.50,
                        ratePSF: 19.00,
                        rateType: "NNN",
                        features: ["5 Private Offices", "Conference Room", "(3) 14×14 Doors", "3-Phase Power", "Fenced/Gated Lot"],
                        image: "property4.jpg",
                        available: true
                    },
                    {
                        id: 5,
                        title: "Professional Office Suite",
                        location: "East Side - Near I-95 & Airport",
                        type: "office",
                        size: 550,
                        sizeUnit: "SF",
                        monthlyRent: 1100.00,
                        features: ["Two Private Offices", "Walk-Up Convenience", "Abundant Parking", "Separate AC Controls"],
                        image: "property5.jpg",
                        available: true,
                        leaseType: "Industrial Gross"
                    },
                    {
                        id: 6,
                        title: "Office/Warehouse Combination",
                        location: "Fort Lauderdale",
                        type: "flex",
                        size: 1825,
                        sizeUnit: "SF",
                        clearHeight: "17'",
                        monthlyRent: 2813.54,
                        ratePSF: 18.50,
                        features: ["700 SF A/C Office", "1,125 SF Warehouse", "12×12 Grade-Level Door", "Light Industrial"],
                        image: "property6.jpg",
                        available: true
                    },
                    {
                        id: 7,
                        title: "Flex Warehouse Space",
                        location: "S Military Trail, West Palm Beach",
                        type: "flex",
                        size: 3375,
                        sizeUnit: "SF",
                        clearHeight: "17'",
                        monthlyRent: 7031.25,
                        ratePSF: 25.00,
                        features: ["750 SF Office", "1,775 SF A/C Warehouse", "(3) 10×10 Doors", "High Visibility"],
                        image: "property7.jpg",
                        available: true
                    },
                    {
                        id: 8,
                        title: "Commercial Warehouse Unit",
                        location: "Lantana Industrial Park",
                        type: "warehouse",
                        size: 2230,
                        sizeUnit: "SF",
                        clearHeight: "18'",
                        monthlyRent: null,
                        features: ["400 SF A/C Office", "A/C Warehouse", "12×14 Overhead Door", "Near I-95"],
                        image: "property8.jpg",
                        available: true
                    },
                    {
                        id: 9,
                        title: "Large Industrial Space with Mezzanine",
                        location: "Lantana Industrial Park",
                        type: "warehouse",
                        size: 6237,
                        sizeUnit: "SF",
                        clearHeight: "16-18'",
                        monthlyRent: null,
                        features: ["1,000 SF Office", "3,600 SF A/C Warehouse", "1,637 SF Mezzanine", "(2) 12×14 Doors"],
                        image: "property9.jpg",
                        available: true,
                        availableDate: "August 2025"
                    }
                ];
                this.filteredProperties = [...this.properties];
            }

            setupEventListeners() {
                const form = document.getElementById('filterForm');
                const inputs = form.querySelectorAll('input, select');
                
                // Debounced handler for all filters
                let filterTimeout;
                const handleFilterChange = (e) => {
                    clearTimeout(filterTimeout);
                    filterTimeout = setTimeout(() => {
                        this.filters[e.target.id] = e.target.value;
                        this.applyFilters();
                    }, 300);
                };

                inputs.forEach(input => {
                    input.addEventListener('input', handleFilterChange);
                    input.addEventListener('change', handleFilterChange);
                });
            }

            applyFilters() {
                this.filteredProperties = this.properties.filter(property => {
                    // Search filter
                    if (this.filters.search) {
                        const searchTerm = this.filters.search.toLowerCase();
                        const searchText = `${property.title} ${property.location} ${property.features.join(' ')} ${property.type}`.toLowerCase();
                        if (!searchText.includes(searchTerm)) return false;
                    }

                    // Type filter
                    if (this.filters.type && property.type !== this.filters.type) return false;

                    // Size filter
                    if (this.filters.size) {
                        const sizeInSF = property.sizeUnit === 'Acres' ? property.size * 43560 : property.size;
                        const [min, max] = this.filters.size.split('-').map(s => s === '+' ? Infinity : parseInt(s));
                        if (sizeInSF < min || sizeInSF > (max || Infinity)) return false;
                    }

                    // Price filter
                    if (this.filters.price) {
                        if (!property.monthlyRent) return this.filters.price === '10000+';
                        const [min, max] = this.filters.price.split('-').map(s => s === '+' ? Infinity : parseInt(s));
                        if (property.monthlyRent < min || property.monthlyRent > (max || Infinity)) return false;
                    }

                    return true;
                });

                // Sort
                this.sortProperties();
                this.render();
            }

            sortProperties() {
                const sortMap = {
                    'price-low': (a, b) => (a.monthlyRent || 999999) - (b.monthlyRent || 999999),
                    'price-high': (a, b) => (b.monthlyRent || 0) - (a.monthlyRent || 0),
                    'size-low': (a, b) => this.getSizeInSF(a) - this.getSizeInSF(b),
                    'size-high': (a, b) => this.getSizeInSF(b) - this.getSizeInSF(a),
                    'featured': () => 0
                };

                const sortFn = sortMap[this.filters.sort];
                if (sortFn) this.filteredProperties.sort(sortFn);
            }

            getSizeInSF(property) {
                return property.sizeUnit === 'Acres' ? property.size * 43560 : property.size;
            }

            formatCurrency(amount) {
                return amount ? `$${amount.toLocaleString('en-US', { minimumFractionDigits: 2, maximumFractionDigits: 2 })}` : 'Call for Rates';
            }

            getPropertySpecs(property) {
                const specs = [];
                
                if (property.size) {
                    specs.push({ label: 'Size', value: `${property.size.toLocaleString()} ${property.sizeUnit}` });
                }
                
                if (property.clearHeight) {
                    specs.push({ label: 'Clear Height', value: property.clearHeight });
                } else if (property.type === 'office') {
                    specs.push({ label: 'Type', value: 'Professional Office' });
                }
                
                specs.push({ 
                    label: 'Monthly Rent', 
                    value: this.formatCurrency(property.monthlyRent) 
                });
                
                if (property.ratePSF) {
                    specs.push({ 
                        label: 'Rate PSF', 
                        value: `$${property.ratePSF.toFixed(2)}/yr ${property.rateType || ''}`.trim() 
                    });
                }
                
                return specs;
            }

            createPropertyCard(property) {
                const specs = this.getPropertySpecs(property);
                const imageUrl = property.image || '';
                const imageStyle = imageUrl ? `background-image: url('${imageUrl}');` : '';
                
                return `
                    <article class="property-card card" data-id="${property.id}">
                        <div class="property-image" style="${imageStyle}">
                            <span class="badge badge-type">LEASE</span>
                            <span class="badge badge-status">AVAILABLE NOW</span>
                        </div>
                        <div class="property-content">
                            <h3 class="property-title">${property.title}</h3>
                            <p class="property-location">${property.location}</p>
                            
                            <div class="property-specs">
                                ${specs.map(spec => `
                                    <div class="spec-item">
                                        <span class="spec-label">${spec.label}:</span>
                                        <span class="spec-value">${spec.value}</span>
                                    </div>
                                `).join('')}
                            </div>
                            
                            <div class="property-features">
                                ${property.features.slice(0, 4).map(feature => 
                                    `<span class="feature-tag">${feature}</span>`
                                ).join('')}
                            </div>
                            
                            <div class="property-actions">
                                <a href="tel:+15617186725" class="btn btn-primary">Call Now</a>
                                <a href="#contact" class="btn btn-secondary">Schedule Tour</a>
                            </div>
                        </div>
                    </article>
                `;
            }

            render() {
                const grid = document.getElementById('propertiesGrid');
                const noResults = document.getElementById('noResults');
                const count = document.getElementById('resultCount');
                
                count.textContent = this.filteredProperties.length;
                
                if (this.filteredProperties.length === 0) {
                    grid.style.display = 'none';
                    noResults.style.display = 'block';
                } else {
                    grid.style.display = 'grid';
                    noResults.style.display = 'none';
                    grid.innerHTML = this.filteredProperties
                        .map(property => this.createPropertyCard(property))
                        .join('');
                }
            }
        }

        // Initialize when DOM is ready
        document.addEventListener('DOMContentLoaded', () => {
            new PropertyManager();
        });
    </script>
</body>
</html>

  <!-- BLOG SECTION -->
  <section class="blog-section">
    <div class="container">
      <div class="section-header">
        <h2>Industrial Real Estate Insights</h2>
        <p>Stay informed about the Palm Beach market</p>
      </div>
      
      <div class="blog-grid">
      <!-- Blog Card 1 -->
<div class="blog-card" id="blog-quantum">
  <span class="blog-category">TECHNOLOGY & INNOVATION</span>
  <h3>Tech & Logistics Boom: How Palm Beach County Industrial Adapts</h3>
  <p class="blog-excerpt">
    From e-commerce fulfillment to tech startups, Palm Beach County's industrial market is evolving to meet modern business demands...
  </p>
  <p class="blog-meta">January 15, 2025 • 5 min read</p>
  <a href="#" class="blog-link">Read Full Analysis</a>
  
  <div class="blog-full-content">
    <p>Palm Beach County's industrial market is experiencing a significant transformation as technology companies and modern logistics operations seek alternatives to traditional tech hubs. With no state income tax, growing infrastructure, and available industrial space, the area is attracting diverse businesses from AI startups to massive e-commerce operations.</p>
    
    <h3>The Tech Migration Reality</h3>
    <p>Tech companies are discovering that Palm Beach County offers compelling advantages: significantly lower operating costs than Silicon Valley or New York, an expanding talent pool as remote workers relocate permanently, and industrial spaces that can be converted for modern uses. While we're not becoming the next Silicon Valley overnight, the trend is real and accelerating.</p>
    
    <h3>E-commerce and Modern Logistics</h3>
    <p>The real growth story is in logistics and fulfillment. Amazon's 855,000 square foot facility in Boynton Beach's Park of Commerce isn't an anomaly - it's part of a broader trend. Last-mile delivery operations are expanding rapidly, with new facilities in Wellington and Royal Palm Beach serving the growing online shopping demand. These operations need 24-32 foot clear heights, proximity to residential areas, and excellent highway access.</p>
    
    <h3>What Tech Companies Actually Need</h3>
    <p>Modern tech operations require more than just office space. They need: reliable fiber internet (widely available in newer industrial parks), flexible spaces that can combine office and light manufacturing, power infrastructure for server rooms and equipment, and proximity to talent pools. Many industrial properties can be adapted for these uses at competitive rates.</p>
    
    <h3>The Workforce Factor</h3>
    <p>Palm Beach County's workforce is evolving. We have Florida Atlantic University producing engineering graduates, Palm Beach State College's technical programs, and an influx of experienced professionals from other markets. The lifestyle advantages - no state income tax, year-round sunshine, and beach proximity - help attract and retain talent.</p>
    
    <h3>Market Opportunities</h3>
    <p>The opportunities are substantial: growing demand, diverse tenant base, and strong fundamentals. Property owners who understand these trends and adapt their spaces accordingly are seeing strong occupancy and rental growth. The key is matching the right property features with evolving tenant needs.</p>
    
    <p>Exploring tech-friendly industrial spaces? Contact us at (561) 718-6725 for properties with the right infrastructure and zoning flexibility.</p>
    
    <span class="blog-close">Close Article</span>
  </div>
</div>

<!-- Blog Card 2 -->
<div class="blog-card" id="blog-market">
  <span class="blog-category">LOCATION GUIDE</span>
  <h3>Top 10 Industrial Zones in Palm Beach County</h3>
  <p class="blog-excerpt">
    Comprehensive guide to Palm Beach County's major industrial corridors, with insights on infrastructure, access, and market dynamics...
  </p>
  <p class="blog-meta">January 10, 2025 • 6 min read</p>
  <a href="#" class="blog-link">View Full Guide</a>
  
  <div class="blog-full-content">
    <p>Palm Beach County's diverse industrial market offers opportunities across multiple submarkets, each with distinct advantages. Understanding these differences helps businesses find their ideal location while appreciating the value each area provides.</p>
    
    <h3>1. Park of Commerce, Boynton Beach</h3>
    <p><strong>Market Position:</strong> The county's premier industrial park at 1,600 acres. Home to Amazon, FedEx, and 300+ successful businesses. Dual I-95/Turnpike access provides unmatched logistics advantages. Buildings from 5,000 to 500,000+ SF accommodate all business sizes.<br>
    <strong>Ideal For:</strong> E-commerce, major distribution, regional operations<br>
    <strong>Value Proposition:</strong> Premium infrastructure and location justify market-leading rents</p>
    
    <h3>2. Riviera Beach Port District</h3>
    <p><strong>Market Position:</strong> Strategic port-adjacent location with Foreign Trade Zone benefits. Heavy industrial zoning permits uses not available elsewhere. Direct access to Caribbean and Central American shipping routes. Robust infrastructure supports intensive operations.<br>
    <strong>Ideal For:</strong> Import/export, marine industries, heavy equipment<br>
    <strong>Value Proposition:</strong> Specialized capabilities command appropriate pricing</p>
    
    <h3>3. Wellington Commerce Park</h3>
    <p><strong>Market Position:</strong> Modern facilities along State Road 7 serving western communities. Contemporary construction with current building standards. Strategic location for last-mile delivery. Proximity to Wellington's unique equestrian market.<br>
    <strong>Ideal For:</strong> Local distribution, equestrian suppliers, western market coverage<br>
    <strong>Value Proposition:</strong> Newer construction and strategic location support strong rates</p>
    
    <h3>4. Airport Area Industrial</h3>
    <p><strong>Market Position:</strong> Specialized location near PBI Airport. Select properties permit 24/7 operations. Established aerospace cluster with Pratt & Whitney anchor. Time-sensitive logistics advantages.<br>
    <strong>Ideal For:</strong> Air freight, aerospace suppliers, time-critical operations<br>
    <strong>Value Proposition:</strong> Unique operational permissions and airport proximity drive demand</p>
    
    <h3>5. Lake Worth/Lantana Corridor</h3>
    <p><strong>Market Position:</strong> Established industrial corridor with diverse inventory. Central location between major employment centers. Mix of building sizes and configurations. Strong small business community.<br>
    <strong>Ideal For:</strong> Contractors, growing businesses, central operations<br>
    <strong>Value Proposition:</strong> Competitive rates reflect market conditions and building age</p>
    
    <h3>6. Royal Palm Beach Business Areas</h3>
    <p><strong>Market Position:</strong> Emerging market serving western expansion. Modern construction standards and infrastructure. Strategic Okeechobee Boulevard location. Positioned for significant growth.<br>
    <strong>Ideal For:</strong> Clean operations, businesses serving western suburbs<br>
    <strong>Value Proposition:</strong> Growth potential and modern facilities support investment</p>
    
    <h3>7. Delray Beach Industrial</h3>
    <p><strong>Market Position:</strong> Benefits from Delray's strong economic environment. Congress Avenue visibility and access. Flexible zoning allows creative uses. Established business community.<br>
    <strong>Ideal For:</strong> Food production, marine industries, showroom/warehouse combinations<br>
    <strong>Value Proposition:</strong> Delray Beach address and flexibility justify premium</p>
    
    <h3>8. Jupiter/Palm Beach Gardens</h3>
    <p><strong>Market Position:</strong> Extremely limited industrial inventory in affluent markets. Strict architectural standards maintain property values. Serving the county's highest-income demographics. Consistent high occupancy.<br>
    <strong>Ideal For:</strong> Luxury goods, yacht services, high-end contractors<br>
    <strong>Value Proposition:</strong> Scarcity and demographics support highest county rents</p>
    
    <h3>9. Greenacres Industrial Parks</h3>
    <p><strong>Market Position:</strong> Municipal advantages including city-owned utilities. Three distinct parks provide options. Central location with good access. Established tenant base.<br>
    <strong>Ideal For:</strong> Light manufacturing, utility-intensive operations<br>
    <strong>Value Proposition:</strong> Utility savings can offset occupancy costs</p>
    
    <h3>10. Turnpike Commerce Centers</h3>
    <p><strong>Market Position:</strong> Institutional-quality logistics facilities. State-of-the-art specifications and management. Designed for maximum operational efficiency. Professional ownership ensures consistency.<br>
    <strong>Ideal For:</strong> Major distribution, corporate logistics, high-volume operations<br>
    <strong>Value Proposition:</strong> Best-in-class facilities merit institutional pricing</p>
    
    <h3>Market Outlook</h3>
    <p>Palm Beach County's industrial market continues to strengthen with growing demand, limited new supply, and diverse tenant requirements. Each submarket offers unique advantages, and understanding these helps businesses appreciate the value proposition of different locations.</p>
    
    <p>For expert guidance on Palm Beach County industrial properties, call (561) 718-6725. We'll help you understand how each area's advantages align with your business needs.</p>
    
    <span class="blog-close">Close Article</span>
  </div>
</div>

<!-- Blog Card 3 -->
<div class="blog-card" id="blog-guide">
  <span class="blog-category">INDUSTRY INSIGHTS</span>
  <h3>5 Industrial Property Trends Reshaping Palm Beach County</h3>
  <p class="blog-excerpt">
    From automation-ready warehouses to sustainable features, discover the trends driving industrial real estate evolution in 2025...
  </p>
  <p class="blog-meta">January 8, 2025 • 6 min read</p>
  <a href="#" class="blog-link">Read Full Analysis</a>
  
  <div class="blog-full-content">
    <p>Palm Beach County's industrial market is evolving rapidly as new technologies and business models reshape space requirements. Understanding these trends helps property owners and businesses prepare for the future of industrial real estate.</p>
    
    <h3>1. Automation and Robotics Integration</h3>
    <p>Modern distribution centers increasingly incorporate automation, from autonomous mobile robots (AMRs) to sophisticated conveyor systems. Properties with 30+ foot clear heights, reinforced floors supporting 1,000+ PSF loads, and robust power infrastructure command premium rents. Forward-thinking properties are pre-installing conduit pathways for future automation needs. The Park of Commerce in Boynton Beach leads this trend with several fully automated facilities.</p>
    
    <h3>2. Last-Mile Delivery Evolution</h3>
    <p>E-commerce growth drives demand for smaller, strategically located facilities near population centers. Properties from 20,000-50,000 SF in Wellington, Royal Palm Beach, and Delray Beach are being converted for quick-turn delivery operations. Features like multiple dock doors, cross-dock configurations, and ample van parking are essential. This trend creates opportunities for older properties with good locations to capture new demand.</p>
    
    <h3>3. Sustainability as Standard</h3>
    <p>Environmental features have moved from "nice-to-have" to market expectation. LED lighting, solar-ready roofs, high-efficiency HVAC, and EV charging stations are becoming standard. LEED certification increasingly influences tenant decisions, particularly for corporate users. Properties investing in sustainability improvements see higher occupancy rates and rental premiums averaging 5-7% above non-green buildings.</p>
    
    <h3>4. Flex Space Renaissance</h3>
    <p>The line between industrial and office continues to blur. Modern businesses need spaces that accommodate warehousing, light manufacturing, showrooms, and creative offices. Properties offering 20-30% office buildout with quality finishes attract diverse tenants from tech startups to established distributors. Delray Beach and Jupiter markets particularly benefit from this trend.</p>
    
    <h3>5. Cold Storage and Controlled Environments</h3>
    <p>Growing demand for temperature-controlled space extends beyond traditional cold storage. Pharmaceutical distribution, specialty foods, and even electronics require climate control. Properties with existing refrigeration infrastructure or power capacity for retrofits see strong demand. The Airport Industrial area particularly suits temperature-sensitive operations requiring quick transport.</p>
    
    <h3>Infrastructure Investments Driving Growth</h3>
    <p>Major infrastructure projects enhance industrial property values across the county. The I-95 express lanes, Turnpike widening, and planned Northlake Boulevard interchange improve logistics efficiency. Properties near these improvements see accelerated rent growth. Smart owners position their properties to benefit from these public investments.</p>
    
    <h3>Technology Integration</h3>
    <p>Beyond physical infrastructure, digital connectivity becomes crucial. Properties with redundant fiber optic connections, 5G readiness, and smart building systems attract tech-savvy tenants. Building management systems that provide real-time data on energy usage, security, and maintenance help tenants optimize operations.</p>
    
    <h3>Looking Ahead</h3>
    <p>These trends accelerate rather than replace traditional industrial demand. While automation and sustainability reshape expectations, location, access, and basic functionality remain paramount. Properties that combine traditional strengths with modern features position themselves for long-term success in Palm Beach County's dynamic industrial market.</p>
    
    <p>To explore how these trends affect specific properties or markets, contact our industrial team at (561) 718-6725. We'll help you understand which improvements offer the best return on investment for your property type and location.</p>
    
    <span class="blog-close">Close Article</span>
  </div>
</div>
</div>
      
      <!-- Newsletter CTA -->
      <div class="blog-cta">
        <h3>Stay Ahead of the Market</h3>
        <p>Get exclusive industrial real estate insights delivered to your inbox</p>
        
        <!-- FIXED NEWSLETTER FORM -->
        <form class="newsletter-form" 
              name="newsletter" 
              method="POST" 
              data-netlify="true"
              netlify-honeypot="bot-field">
          
          <!-- Hidden fields for Netlify -->
          <input type="hidden" name="form-name" value="newsletter">
          <div style="display:none">
            <label>Don't fill this out: <input name="bot-field"></label>
          </div>
          
          <input type="email" name="email" placeholder="Enter your email" required>
          <button type="submit">Subscribe</button>
        </form>
      </div>
    </div>
  </section>

  <!-- FAQ SECTION -->
  <section class="faq-section" id="faq">
    <div class="container">
      <div class="section-header">
        <h2>Frequently Asked Questions</h2>
        <p>Answers to common industrial leasing questions</p>
      </div>
      
      <div class="faq-container">
        <div class="faq-item">
          <div class="faq-question">
            What are the current warehouse rental rates in West Palm Beach?
            <span class="faq-icon">▼</span>
          </div>
          <div class="faq-answer">
            Current warehouse rental rates in West Palm Beach range from $22-25 per square foot gross annually, depending on location, amenities, and lease terms. Premium locations near major highways command higher rates. Contact us for specific pricing on available properties.
          </div>
        </div>
        
        <div class="faq-item">
          <div class="faq-question">
            What size spaces are available?
            <span class="faq-icon">▼</span>
          </div>
          <div class="faq-answer">
            We have industrial spaces ranging from 1,000 sq ft for small operations up to 50,000+ sq ft for large distribution centers. Many properties offer divisible space, allowing you to lease exactly what you need. We also help businesses plan for future expansion.
          </div>
        </div>
        
        <div class="faq-item">
          <div class="faq-question">
            How quickly can I move in?
            <span class="faq-icon">▼</span>
          </div>
          <div class="faq-answer">
            Most of our featured properties are move-in ready within 30-60 days. The timeline depends on lease negotiations, any required improvements, and permit requirements. We work closely with property owners to expedite the process for qualified tenants.
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT SECTION -->
  <section class="about-section" id="about">
    <div class="container">
      <div class="section-header">
        <h2>About Palm Beach Warehouses</h2>
        <p>Your resource for industrial and warehouse space in Palm Beach County</p>
      </div>
      
      <div class="about-content">
        <div class="about-text">
          <h3>Industrial Real Estate in Palm Beach County</h3>
          <p class="about-lead">
            Palm Beach Warehouses connects businesses with available industrial, warehouse, and flex spaces throughout Palm Beach County. We provide comprehensive property listings and direct access to property owners and managers.
          </p>
          
          <p>Whether you're a small business looking for your first warehouse space or an established company seeking to expand operations, our platform helps you find and compare available properties in key industrial areas including West Palm Beach, Boynton Beach, Lake Worth, and surrounding communities.</p>
          
          <h3>What We Offer</h3>
          <ul style="list-style: none; padding: 0;">
            <li style="margin-bottom: 0.8rem;">✓ <strong>Current Listings:</strong> Up-to-date availability of warehouse and industrial spaces</li>
            <li style="margin-bottom: 0.8rem;">✓ <strong>Direct Contact:</strong> Connect directly with property representatives</li>
            <li style="margin-bottom: 0.8rem;">✓ <strong>Property Details:</strong> Clear information on sizes, features, and pricing</li>
            <li style="margin-bottom: 0.8rem;">✓ <strong>Local Focus:</strong> Exclusively focused on Palm Beach County properties</li>
          </ul>
          
          <h3>Palm Beach County Industrial Market</h3>
          <p>Palm Beach County offers diverse industrial real estate options, from small flex spaces perfect for startups to large distribution centers for major operations. The area benefits from:</p>
          <ul style="list-style: none; padding: 0; margin-top: 1rem;">
            <li style="margin-bottom: 0.5rem;">• Strategic location with access to major highways (I-95, Florida Turnpike)</li>
            <li style="margin-bottom: 0.5rem;">• Proximity to Port of Palm Beach and three international airports</li>
            <li style="margin-bottom: 0.5rem;">• Growing business community and skilled workforce</li>
            <li style="margin-bottom: 0.5rem;">• Year-round operational advantages with Florida's climate</li>
          </ul>
        </div>
        
        <div class="about-cta-box">
          <h3>Ready to Find Your Space?</h3>
          <p>Browse our current listings or speak with a representative</p>
          <a href="tel:+15617186725" class="about-phone">561-718-6725</a>
          <p class="about-availability">Available to Answer Your Questions</p>
          
          <div class="about-features">
            <p class="about-feature">✓ View Available Properties</p>
            <p class="about-feature">✓ Schedule Property Tours</p>
            <p class="about-feature">✓ Get Pricing Information</p>
            <p class="about-feature">✓ Learn About Lease Terms</p>
          </div>
          
          <a href="#propertyForm" class="submit-button" style="margin-top: 1rem;">
            Get Started →
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="container">
      <div class="footer-content">
        <h3>INDUSTRIAL<span style="color: var(--teal);">SPACE</span></h3>
        <p>Your trusted partner for industrial real estate in Palm Beach County</p>
        
        <div class="footer-links">
          <a href="#properties">Properties</a>
          <a href="#about">About</a>
          <a href="#faq">FAQ</a>
          <a href="tel:+15617186725">Contact</a>
        </div>
        
        <div class="footer-bottom">
          <p>&copy; 2025 IndustrialSpace. All rights reserved. | 
            <a href="#" id="terms-toggle" style="color: var(--teal); cursor: pointer;">Terms & Privacy</a>
          </p>
          
          <p style="margin-top: 1rem; color: #ccc; font-size: 0.9rem;">
Zachary Vorsteg, Licensed Florida Real Estate Agent | Cornerstone Realty (License #SL3603483)<br>
This website is independently operated and not the official website of Cornerstone Realty.
</p>
          
          <!-- Terms & Privacy Dropdown -->
          <div id="terms-dropdown" class="terms-dropdown" style="display: none;">
            <div class="terms-content">
              <h4>Terms of Use & Privacy</h4>
              
              <div class="terms-section">
                <h5>Your Privacy Matters</h5>
                <p>We respect your privacy and are committed to protecting your information. When you submit an inquiry through our forms:</p>
                <ul>
                  <li>Your information is used solely to connect you with relevant property owners and managers</li>
                  <li>We do not sell, share, or distribute your personal data to third parties</li>
                  <li>Email addresses are used only for property-related communications</li>
                  <li>You may request removal from our contact list at any time</li>
                </ul>
              </div>
              
              <div class="terms-section">
                <h5>Terms of Service</h5>
                <p>By using this website, you acknowledge that:</p>
                <ul>
                  <li>Property information is subject to change and availability</li>
                  <li>We act as a connection service between prospective tenants and property representatives</li>
                  <li>Final lease terms and agreements are between you and the property owner/manager</li>
                  <li>We are not responsible for the accuracy of third-party property listings</li>
                  <li>This site is for informational purposes to facilitate real estate connections</li>
                </ul>
              </div>
              
              <div class="terms-section">
                <h5>Contact & Data Requests</h5>
                <p>For any questions about your data or to request removal from our systems, please contact us at 561-718-6725 or through our contact form. We're committed to transparency and will respond to all privacy-related requests promptly.</p>
              </div>
              
              <button class="terms-close" onclick="document.getElementById('terms-dropdown').style.display='none'">
                Close
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>

  <!-- FLOATING CTA -->
  <a href="tel:+15617186725" class="floating-cta">
    📞 Call Now
  </a>

  <!-- JAVASCRIPT -->
  <script>
    // Contact form submission
    const inquiryForm = document.getElementById('propertyInquiry');
    if(inquiryForm) {
      inquiryForm.addEventListener('submit', async (e) => {
        e.preventDefault();
        const submitBtn = e.target.querySelector('button[type="submit"]');
        submitBtn.disabled = true;
        submitBtn.textContent = 'Submitting...';

        const formData = new FormData(inquiryForm);

        try {
          let response = await fetch('/', {
            method: 'POST',
            headers: { "Content-Type": "application/x-www-form-urlencoded" },
            body: new URLSearchParams(formData).toString()
          });

          if (response.ok) {
            inquiryForm.innerHTML = `
              <div style="text-align:center; padding:2rem;">
                <h3 style="color: var(--teal); margin-bottom:1rem;">✓ Thank You!</h3>
                <p style="margin-bottom:1.5rem;">We've received your inquiry and will contact you within 24 hours.</p>
                <p style="font-size:1.2rem; font-weight:700; margin-bottom:1rem;">Want to speak now?</p>
                <a href="tel:+15617186725" class="submit-button" style="display:inline-block; padding:1rem 2rem;">
                  📞 Call (561) 718-6725
                </a>
              </div>
            `;
          } else {
            alert('Submission failed. Please call (561) 718-6725 directly.');
            submitBtn.disabled = false;
            submitBtn.textContent = 'GET PROPERTY LIST & SCHEDULE TOUR →';
          }
        } catch (err) {
          alert('Could not submit form. Please call (561) 718-6725 directly.');
          submitBtn.disabled = false;
          submitBtn.textContent = 'GET PROPERTY LIST & SCHEDULE TOUR →';
        }
      });
    }

    // Newsletter form submission
    document.querySelectorAll('.newsletter-form').forEach(form => {
      form.addEventListener('submit', async function(e) {
        e.preventDefault();
        const submitBtn = form.querySelector('button[type="submit"]');
        submitBtn.disabled = true;
        submitBtn.textContent = 'Subscribing...';
        const formData = new FormData(form);

        try {
          let response = await fetch('/', {
            method: 'POST',
            headers: { "Content-Type": "application/x-www-form-urlencoded" },
            body: new URLSearchParams(formData).toString()
          });

          if (response.ok) {
            form.innerHTML = `<div style="text-align:center; padding:1.5rem 0;">
              <strong style="color: var(--teal); font-size:1.2rem;">Thank you for subscribing!</strong><br>
              Market insights will be delivered to your inbox.
            </div>`;
          } else {
            submitBtn.disabled = false;
            submitBtn.textContent = 'Subscribe';
            alert('Could not subscribe. Please try again or call (561) 718-6725.');
          }
        } catch (err) {
          submitBtn.disabled = false;
          submitBtn.textContent = 'Subscribe';
          alert('Could not subscribe. Please try again or call (561) 718-6725.');
        }
      });
    });

    // Phone number formatting
    const phoneInput = document.getElementById('phone');
    if(phoneInput) {
      phoneInput.addEventListener('input', (e) => {
        let value = e.target.value.replace(/\D/g, '');
        let formatted = '';
        if(value.length > 0) {
          formatted = '(' + value.substring(0,3);
        }
        if(value.length >= 4) {
          formatted += ') ' + value.substring(3,6);
        }
        if(value.length >= 7) {
          formatted += '-' + value.substring(6,10);
        }
        e.target.value = formatted;
      });
    }

    // Smooth scroll for internal anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', (e) => {
        const href = anchor.getAttribute('href');
        if (href === '#' || href.startsWith('#blog-')) return;

        const targetID = href.replace('#','');
        const targetElem = document.getElementById(targetID);
        if(targetElem) {
          e.preventDefault();
          targetElem.scrollIntoView({ behavior: 'smooth', block: 'start' });
        }
      });
    });

    // Floating CTA hide/show on scroll
    let lastScrollPos = 0;
    const floatCTA = document.querySelector('.floating-cta');
    window.addEventListener('scroll', () => {
      const currentScroll = window.pageYOffset;
      if(currentScroll > 300) {
        if(currentScroll > lastScrollPos) {
          floatCTA.style.transform = 'translateY(100px)';
        } else {
          floatCTA.style.transform = 'translateY(0)';
        }
      }
      lastScrollPos = currentScroll;
    });

    // FAQ Accordion
    const faqItems = document.querySelectorAll('.faq-item');
    faqItems.forEach(item => {
      const question = item.querySelector('.faq-question');
      const answer = item.querySelector('.faq-answer');
      const icon = item.querySelector('.faq-icon');
      question.addEventListener('click', () => {
        const isOpen = answer.style.display === 'block';

        // Close all
        faqItems.forEach(faq => {
          faq.querySelector('.faq-answer').style.display = 'none';
          faq.querySelector('.faq-icon').style.transform = 'rotate(0deg)';
        });

        // Toggle
        if(!isOpen) {
          answer.style.display = 'block';
          icon.style.transform = 'rotate(180deg)';
        }
      });
    });

    // Blog toggle
    document.querySelectorAll('.blog-card').forEach(card => {
      const link = card.querySelector('.blog-link');
      const closeBtn = card.querySelector('.blog-close');
      const title = card.querySelector('h3');

      [link, title].forEach(element => {
        if (element) {
          element.addEventListener('click', (e) => {
            e.preventDefault();
            e.stopPropagation();
            document.querySelectorAll('.blog-card.expanded').forEach(otherCard => {
              if (otherCard !== card) {
                otherCard.classList.remove('expanded');
              }
            });
            card.classList.toggle('expanded');
            if (card.classList.contains('expanded')) {
              setTimeout(() => {
                card.scrollIntoView({ behavior: 'smooth', block: 'start' });
              }, 100);
            }
          });
        }
      });

      if (closeBtn) {
        closeBtn.addEventListener('click', (e) => {
          e.stopPropagation();
          card.classList.remove('expanded');
        });
      }
    });

    // Mobile menu toggle
    const mobileToggle = document.querySelector('.mobile-menu-toggle');
    const mobileMenu = document.createElement('div');
    mobileMenu.className = 'mobile-menu';
    mobileMenu.innerHTML = `
      <div class="mobile-menu-content">
        <button class="mobile-menu-close">✕</button>
        <div class="mobile-menu-links">
          <a href="#properties">Properties</a>
          <a href="#about">About</a>
          <a href="#faq">FAQ</a>
          <a href="tel:+15617186725" class="mobile-menu-phone">📞 Call 561-718-6725</a>
          <a href="#propertyForm" class="mobile-menu-cta">Get Available Properties</a>
        </div>
      </div>
    `;
    document.body.appendChild(mobileMenu);
    
    if(mobileToggle) {
      mobileToggle.addEventListener('click', () => {
        mobileMenu.classList.add('active');
        document.body.style.overflow = 'hidden';
      });
    }
    
    const mobileMenuClose = mobileMenu.querySelector('.mobile-menu-close');
    mobileMenuClose.addEventListener('click', () => {
      mobileMenu.classList.remove('active');
      document.body.style.overflow = '';
    });
    
    // Close mobile menu when clicking links
    mobileMenu.querySelectorAll('a').forEach(link => {
      link.addEventListener('click', () => {
        mobileMenu.classList.remove('active');
        document.body.style.overflow = '';
      });
    });

    // Animate on scroll
    const observerOptions = {
      threshold: 0.1,
      rootMargin: '0px 0px -50px 0px'
    };
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = '1';
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, observerOptions);

    // Observe property/benefit cards
    document.querySelectorAll('.property-card').forEach((card, index) => {
      card.style.opacity = '0';
      card.style.transform = 'translateY(20px)';
      card.style.transition = `all 0.5s ease ${index * 0.1}s`;
      observer.observe(card);
    });
    document.querySelectorAll('.benefit-card').forEach((card, index) => {
      card.style.opacity = '0';
      card.style.transform = 'translateY(20px)';
      card.style.transition = `all 0.5s ease ${index * 0.1}s`;
      observer.observe(card);
    });

    // Ripple effect
    document.querySelectorAll('.property-button, .nav-button').forEach(button => {
      button.addEventListener('click', function(e) {
        const ripple = document.createElement('span');
        const rect = this.getBoundingClientRect();
        const size = Math.max(rect.width, rect.height);
        const x = e.clientX - rect.left - size / 2;
        const y = e.clientY - rect.top - size / 2;

        ripple.style.width = ripple.style.height = size + 'px';
        ripple.style.left = x + 'px';
        ripple.style.top = y + 'px';
        ripple.classList.add('ripple');
        this.appendChild(ripple);
        setTimeout(() => ripple.remove(), 600);
      });
    });

    // Performance
    window.addEventListener('load', () => {
      if ('performance' in window) {
        const perfData = window.performance.timing;
        const pageLoadTime = perfData.loadEventEnd - perfData.navigationStart;
        console.log('Page load time:', pageLoadTime + 'ms');
      }
    });

    // Availability hover/click
    function initializeAvailabilityFeatures() {
      document.querySelectorAll('.availability-badge').forEach(badge => {
        const originalText = badge.textContent;
        badge.addEventListener('mouseenter', () => {
          badge.style.transform = 'scale(1.05)';
          badge.style.cursor = 'pointer';
          if (badge.classList.contains('urgent')) {
            badge.textContent = 'Call to Secure';
          }
        });
        badge.addEventListener('mouseleave', () => {
          badge.style.transform = 'scale(1)';
          badge.textContent = originalText;
        });
        badge.addEventListener('click', () => {
          window.location.href = 'tel:+15617186725';
        });
      });
    }
    initializeAvailabilityFeatures();

    // Terms & Privacy dropdown toggle
    const termsToggle = document.getElementById('terms-toggle');
    const termsDropdown = document.getElementById('terms-dropdown');
    
    if (termsToggle) {
      termsToggle.addEventListener('click', (e) => {
        e.preventDefault();
        termsDropdown.style.display = termsDropdown.style.display === 'none' ? 'block' : 'none';
      });
    }
    
    // Close dropdown when clicking outside
    document.addEventListener('click', (e) => {
      if (!e.target.closest('#terms-dropdown') && !e.target.closest('#terms-toggle')) {
        if (termsDropdown) termsDropdown.style.display = 'none';
      }
    });

    // Basic call tracking
    document.querySelectorAll('a[href^="tel:"]').forEach(link => {
      link.addEventListener('click', () => {
        console.log('Phone call initiated:', link.getAttribute('href'));
      });
    });
  </script>
</body>
</html>
