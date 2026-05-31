<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>BuggCloud Geomatics — Premium Surveying Solutions | Secunderabad</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
:root {
  --bg-dark: #0a0e27;
  --bg-card: #111835;
  --bg-accent: #1a2447;
  --gold-primary: #d4a574;
  --gold-bright: #f5c85f;
  --orange-accent: #ff8c42;
  --safety-yellow: #ffc107;
  --text-primary: #ffffff;
  --text-secondary: #b0b8d4;
  --text-muted: #7a8299;
  --border-color: rgba(212, 165, 116, 0.15);
  --border-bright: rgba(245, 200, 95, 0.25);
}

*, *::before, *::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Inter', sans-serif;
  background: var(--bg-dark);
  color: var(--text-primary);
  overflow-x: hidden;
  line-height: 1.6;
}

/* ════════════════════════════════════════════════════════════ */
/* NAV BAR - PREMIUM STICKY */
/* ════════════════════════════════════════════════════════════ */

nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
  height: 72px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 60px;
  background: rgba(10, 14, 39, 0.92);
  backdrop-filter: blur(20px);
  border-bottom: 1px solid var(--border-color);
  transition: all 0.3s ease;
}

nav.scrolled {
  height: 64px;
  padding: 0 50px;
  background: rgba(10, 14, 39, 0.98);
  border-bottom-color: var(--border-bright);
}

.nav-logo-container {
  display: flex;
  align-items: center;
  gap: 16px;
  text-decoration: none;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.nav-logo-container:hover {
  transform: scale(1.05);
}

.nav-logo-img {
  height: 48px;
  width: auto;
  object-fit: contain;
  filter: drop-shadow(0 4px 12px rgba(212, 165, 116, 0.3));
}

.nav-logo-text {
  display: flex;
  flex-direction: column;
  line-height: 1;
}

.nav-brand {
  font-family: 'Syne', sans-serif;
  font-size: 16px;
  font-weight: 700;
  color: var(--text-primary);
  letter-spacing: 0.05em;
}

.nav-tagline {
  font-size: 10px;
  color: var(--gold-primary);
  letter-spacing: 0.15em;
  text-transform: uppercase;
  margin-top: 2px;
}

.nav-menu {
  display: flex;
  gap: 48px;
  list-style: none;
}

.nav-menu a {
  font-size: 13px;
  font-weight: 500;
  color: var(--text-secondary);
  text-decoration: none;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  position: relative;
  transition: color 0.3s ease;
}

.nav-menu a::after {
  content: '';
  position: absolute;
  bottom: -6px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--gold-primary);
  transition: width 0.3s ease;
}

.nav-menu a:hover {
  color: var(--gold-primary);
}

.nav-menu a:hover::after {
  width: 100%;
}

.nav-cta {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 11px 28px;
  background: var(--gold-primary);
  color: var(--bg-dark);
  border: none;
  border-radius: 6px;
  font-family: 'Syne', sans-serif;
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
}

.nav-cta:hover {
  background: var(--gold-bright);
  transform: translateY(-2px);
  box-shadow: 0 12px 24px rgba(245, 200, 95, 0.3);
}

/* ════════════════════════════════════════════════════════════ */
/* HERO - FULL SCREEN CINEMATIC */
/* ════════════════════════════════════════════════════════════ */

.hero {
  position: relative;
  width: 100%;
  height: 100vh;
  min-height: 800px;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}

.hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 800"><defs><linearGradient id="g1" x1="0%" y1="0%" x2="100%" y2="100%"><stop offset="0%" style="stop-color:rgba(255,140,66,0.12);stop-opacity:1" /><stop offset="100%" style="stop-color:rgba(212,165,116,0.08);stop-opacity:1" /></linearGradient></defs><rect width="1200" height="800" fill="url(%23g1)"/><circle cx="200" cy="200" r="300" fill="rgba(255,140,66,0.05)" /><circle cx="1000" cy="600" r="400" fill="rgba(212,165,116,0.05)" /></svg>');
  background-size: cover;
  background-position: center;
}

.hero-bg-image {
    position: absolute;
    inset: 0;
    background:
    linear-gradient(
        rgba(0,0,0,0.55),
        rgba(0,0,0,0.55)
    ),
    url('images/banner.jpeg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    z-index: 0;
}

.hero-bg-image::after {
  content: '';
  position: absolute;
  inset: 0;
  background: 
    radial-gradient(ellipse 600px 400px at 30% 50%, rgba(255, 140, 66, 0.15) 0%, transparent 70%),
    radial-gradient(ellipse 700px 500px at 70% 50%, rgba(212, 165, 116, 0.1) 0%, transparent 60%);
  opacity: 0.8;
}

.hero-construction-overlay {
  position: absolute;
  inset: 0;
  background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="construction" x="0" y="0" width="100" height="100" patternUnits="userSpaceOnUse"><rect x="0" y="0" width="50" height="50" fill="rgba(255,193,7,0.02)"/><rect x="50" y="50" width="50" height="50" fill="rgba(255,193,7,0.02)"/><line x1="0" y1="0" x2="100" y2="100" stroke="rgba(212,165,116,0.03)" stroke-width="1"/></pattern></defs><rect width="100" height="100" fill="url(%23construction)"/></svg>');
  z-index: 1;
  opacity: 0.6;
}

.hero-content {
  position: relative;
  z-index: 10;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 100px 40px;
  max-width: 1100px;
  margin: 0 auto;
}

/* LOGO - MASSIVE AND ICONIC */
.hero-logo {
  width: 280px;
  height: 280px;
  margin-bottom: 40px;
  filter: drop-shadow(0 20px 40px rgba(212, 165, 116, 0.4));
  animation: logoFloat 6s ease-in-out infinite;
}

@keyframes logoFloat {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-20px); }
}

.hero-eyebrow {
  display: inline-block;
  font-family: 'Syne', sans-serif;
  font-size: 14px;
  font-weight: 600;
  color: var(--gold-primary);
  letter-spacing: 0.2em;
  text-transform: uppercase;
  margin-bottom: 20px;
  padding: 12px 24px;
  border: 1px solid var(--border-bright);
  border-radius: 40px;
  background: rgba(245, 200, 95, 0.08);
  animation: slideUp 0.8s ease 0.2s both;
}

.hero-h1 {
  font-family: 'Syne', sans-serif;
  font-size: clamp(48px, 10vw, 90px);
  font-weight: 800;
  line-height: 1.1;
  color: var(--text-primary);
  margin-bottom: 16px;
  animation: slideUp 0.8s ease 0.3s both;
  letter-spacing: -0.02em;
}

.hero-h1-gold {
  color: var(--gold-bright);
  position: relative;
  display: inline-block;
}

.hero-h1-gold::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(90deg, var(--gold-primary), var(--orange-accent));
  border-radius: 2px;
  animation: scaleX 0.8s ease 0.5s both;
}

@keyframes scaleX {
  from { transform: scaleX(0); transform-origin: left; }
  to { transform: scaleX(1); transform-origin: left; }
}

.hero-subtitle {
  font-size: 20px;
  color: var(--text-secondary);
  line-height: 1.6;
  max-width: 700px;
  margin: 24px auto 40px;
  animation: slideUp 0.8s ease 0.4s both;
}

.hero-cta-group {
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
  animation: slideUp 0.8s ease 0.5s both;
}

.btn-primary {
  display: inline-flex;
  align-items: center;
  gap: 12px;
  padding: 18px 42px;
  background: var(--gold-primary);
  color: var(--bg-dark);
  border: 2px solid var(--gold-primary);
  border-radius: 8px;
  font-family: 'Syne', sans-serif;
  font-size: 14px;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.btn-primary::before {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--orange-accent);
  z-index: -1;
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.3s ease;
}

.btn-primary:hover {
  color: var(--text-primary);
  border-color: var(--orange-accent);
  transform: translateY(-3px);
}

.btn-primary:hover::before {
  transform: scaleX(1);
}

.btn-secondary {
  display: inline-flex;
  align-items: center;
  gap: 12px;
  padding: 18px 42px;
  background: transparent;
  color: var(--text-primary);
  border: 2px solid var(--text-secondary);
  border-radius: 8px;
  font-family: 'Syne', sans-serif;
  font-size: 14px;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.3s ease;
}

.btn-secondary:hover {
  border-color: var(--gold-primary);
  color: var(--gold-primary);
  transform: translateY(-3px);
  background: rgba(212, 165, 116, 0.1);
}

.hero-stats {
  position: absolute;
  bottom: 80px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  gap: 80px;
  animation: slideUp 0.8s ease 0.6s both;
}

.stat {
  text-align: center;
}

.stat-number {
  font-family: 'Syne', sans-serif;
  font-size: 48px;
  font-weight: 800;
  color: var(--gold-bright);
  line-height: 1;
  margin-bottom: 8px;
}

.stat-label {
  font-size: 12px;
  color: var(--text-muted);
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

.scroll-indicator {
  position: absolute;
  bottom: 30px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 11;
  animation: slideUp 1s ease 0.8s both;
}

.scroll-arrow {
  width: 24px;
  height: 40px;
  border: 2px solid var(--text-muted);
  border-radius: 12px;
  position: relative;
  margin: 0 auto 12px;
}

.scroll-arrow::after {
  content: '';
  position: absolute;
  top: 8px;
  left: 50%;
  transform: translateX(-50%);
  width: 4px;
  height: 8px;
  background: var(--text-muted);
  border-radius: 2px;
  animation: scrollBounce 1.5s infinite;
}

@keyframes scrollBounce {
  0%, 100% { transform: translateX(-50%) translateY(0); opacity: 1; }
  100% { transform: translateX(-50%) translateY(16px); opacity: 0; }
}

.scroll-text {
  font-size: 11px;
  color: var(--text-muted);
  letter-spacing: 0.15em;
  text-transform: uppercase;
  animation: pulse 2s infinite;
}

@keyframes slideUp {
  from { opacity: 0; transform: translateY(30px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes pulse {
  0%, 100% { opacity: 0.7; }
  50% { opacity: 1; }
}

/* ════════════════════════════════════════════════════════════ */
/* SECTION BASE STYLES */
/* ════════════════════════════════════════════════════════════ */

section {
  padding: 120px 60px;
}

.sec-label {
  display: inline-flex;
  align-items: center;
  gap: 12px;
  font-family: 'Syne', sans-serif;
  font-size: 12px;
  font-weight: 700;
  color: var(--gold-primary);
  letter-spacing: 0.2em;
  text-transform: uppercase;
  margin-bottom: 16px;
}

.sec-label::before {
  content: '';
  width: 40px;
  height: 2px;
  background: var(--gold-primary);
}

.sec-h2 {
  font-family: 'Syne', sans-serif;
  font-size: clamp(36px, 5vw, 64px);
  font-weight: 800;
  line-height: 1.1;
  color: var(--text-primary);
  margin-bottom: 20px;
  letter-spacing: -0.01em;
}

.sec-h2 em {
  color: var(--gold-bright);
  font-style: normal;
}

.sec-desc {
  font-size: 16px;
  color: var(--text-secondary);
  max-width: 600px;
  line-height: 1.8;
  margin-bottom: 60px;
}

/* ════════════════════════════════════════════════════════════ */
/* SERVICES SHOWCASE - GRID WITH IMAGES */
/* ════════════════════════════════════════════════════════════ */

.services {
  background: var(--bg-dark);
}

.srv-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 32px;
  margin-bottom: 80px;
}

.srv-card {
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  border-radius: 12px;
  overflow: hidden;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  position: relative;
  group: card;
}

.srv-card:hover {
  border-color: var(--gold-primary);
  background: var(--bg-accent);
  transform: translateY(-8px);
  box-shadow: 0 20px 40px rgba(212, 165, 116, 0.2);
}

.srv-image {
  position: relative;
  width: 100%;
  aspect-ratio: 16/10;
  background: linear-gradient(135deg, rgba(255, 140, 66, 0.2) 0%, rgba(212, 165, 116, 0.15) 100%);
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 13px;
  color: var(--text-muted);
  text-align: center;
  padding: 20px;
  border-bottom: 1px solid var(--border-color);
  font-style: italic;
}

.srv-image::before {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(circle at center, rgba(245, 200, 95, 0.1) 0%, transparent 70%);
  opacity: 0;
  transition: opacity 0.4s ease;
}

.srv-card:hover .srv-image::before {
  opacity: 1;
}

.srv-content {
  padding: 32px;
}

.srv-icon {
  width: 56px;
  height: 56px;
  background: linear-gradient(135deg, var(--gold-primary), var(--orange-accent));
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  font-size: 28px;
}

.srv-title {
  font-family: 'Syne', sans-serif;
  font-size: 18px;
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: 12px;
  letter-spacing: -0.01em;
}

.srv-bullets {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.srv-bullets li {
  font-size: 14px;
  color: var(--text-secondary);
  display: flex;
  align-items: center;
  gap: 10px;
  transition: transform 0.2s ease;
}

.srv-bullets li::before {
  content: '';
  width: 6px;
  height: 6px;
  background: var(--gold-primary);
  border-radius: 50%;
  flex-shrink: 0;
}

.srv-bullets li:hover {
  transform: translateX(8px);
  color: var(--gold-primary);
}

/* ════════════════════════════════════════════════════════════ */
/* EQUIPMENT SHOWCASE */
/* ════════════════════════════════════════════════════════════ */

.equipment-showcase {
  background: var(--bg-dark);
  margin: 0 -60px;
  padding: 100px 60px;
  border-top: 1px solid var(--border-color);
  border-bottom: 1px solid var(--border-color);
}

.equipment-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 40px;
  align-items: center;
}

.equipment-left {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

.equipment-item {
  position: relative;
  aspect-ratio: 1;
  border-radius: 12px;
  overflow: hidden;
  border: 1px solid var(--border-color);
  background: linear-gradient(135deg, rgba(255, 140, 66, 0.15) 0%, rgba(212, 165, 116, 0.1) 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 12px;
  color: var(--text-muted);
  text-align: center;
  padding: 20px;
  cursor: pointer;
  transition: all 0.4s ease;
}

.equipment-item:hover {
  border-color: var(--gold-primary);
  background: linear-gradient(135deg, rgba(255, 140, 66, 0.25) 0%, rgba(212, 165, 116, 0.15) 100%);
  transform: scale(1.05);
  box-shadow: 0 12px 24px rgba(212, 165, 116, 0.2);
}

.equipment-label {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(to top, rgba(10, 14, 39, 0.9), transparent);
  padding: 16px 12px 12px;
  font-family: 'Syne', sans-serif;
  font-size: 13px;
  font-weight: 600;
  color: var(--gold-primary);
  text-align: center;
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

.equipment-right {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.equipment-desc {
  font-size: 16px;
  color: var(--text-secondary);
  line-height: 1.8;
  margin-bottom: 20px;
}

.equipment-features {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.feature {
  display: flex;
  gap: 16px;
  padding: 16px;
  background: rgba(212, 165, 116, 0.08);
  border-radius: 8px;
  border-left: 3px solid var(--gold-primary);
}

.feature-icon {
  font-size: 24px;
  flex-shrink: 0;
}

.feature-text {
  flex: 1;
}

.feature-title {
  font-family: 'Syne', sans-serif;
  font-size: 14px;
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: 4px;
}

.feature-desc {
  font-size: 13px;
  color: var(--text-secondary);
  line-height: 1.6;
}

/* ════════════════════════════════════════════════════════════ */
/* STAT SHOWCASE */
/* ════════════════════════════════════════════════════════════ */

.stats-showcase {
  background: linear-gradient(135deg, rgba(255, 140, 66, 0.1) 0%, rgba(212, 165, 116, 0.08) 100%);
  margin: 0 -60px;
  padding: 80px 60px;
  border-top: 1px solid var(--border-bright);
  border-bottom: 1px solid var(--border-bright);
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 40px;
  text-align: center;
}

.stat-card {
  padding: 40px 20px;
  transition: transform 0.3s ease;
}

.stat-card:hover {
  transform: translateY(-8px);
}

.stat-big {
  font-family: 'Syne', sans-serif;
  font-size: clamp(36px, 8vw, 60px);
  font-weight: 800;
  background: linear-gradient(135deg, var(--gold-primary), var(--gold-bright));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 12px;
}

.stat-small {
  font-size: 14px;
  color: var(--text-secondary);
  letter-spacing: 0.1em;
  text-transform: uppercase;
  font-weight: 600;
}

/* ════════════════════════════════════════════════════════════ */
/* ABOUT SECTION */
/* ════════════════════════════════════════════════════════════ */

.about {
  background: var(--bg-dark);
}

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
  align-items: center;
}

.about-content {}

.about-points {
  display: flex;
  flex-direction: column;
  gap: 32px;
  margin-top: 40px;
}

.point {
  display: flex;
  gap: 24px;
}

.point-num {
  font-family: 'Syne', sans-serif;
  font-size: 32px;
  font-weight: 800;
  color: var(--gold-bright);
  flex-shrink: 0;
}

.point-text {}

.point-title {
  font-family: 'Syne', sans-serif;
  font-size: 16px;
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: 8px;
}

.point-desc {
  font-size: 14px;
  color: var(--text-secondary);
  line-height: 1.7;
}

.about-image {
  position: relative;
  width: 100%;
  aspect-ratio: 4/5;
  border-radius: 12px;
  overflow: hidden;
  border: 2px solid var(--border-color);
  background: linear-gradient(135deg, rgba(255, 140, 66, 0.2) 0%, rgba(212, 165, 116, 0.15) 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 14px;
  color: var(--text-muted);
  text-align: center;
  padding: 40px;
  font-style: italic;
}

.about-image::before {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(circle at center, rgba(245, 200, 95, 0.15) 0%, transparent 70%);
}

/* ════════════════════════════════════════════════════════════ */
/* CONTACT SECTION */
/* ════════════════════════════════════════════════════════════ */

.contact {
  background: var(--bg-dark);
  border-top: 1px solid var(--border-color);
}

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 60px;
}

.contact-info {}

.contact-items {
  display: flex;
  flex-direction: column;
  gap: 24px;
  margin-top: 40px;
}

.contact-item {
  display: flex;
  gap: 20px;
  padding: 24px;
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  border-radius: 10px;
  transition: all 0.3s ease;
}

.contact-item:hover {
  border-color: var(--gold-primary);
  background: var(--bg-accent);
}

.contact-icon {
  width: 48px;
  height: 48px;
  background: linear-gradient(135deg, var(--gold-primary), var(--orange-accent));
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 24px;
  flex-shrink: 0;
}

.contact-text {}

.contact-label {
  font-size: 11px;
  color: var(--gold-primary);
  letter-spacing: 0.15em;
  text-transform: uppercase;
  margin-bottom: 4px;
}

.contact-value {
  font-family: 'Syne', sans-serif;
  font-size: 15px;
  font-weight: 600;
  color: var(--text-primary);
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.form-label {
  font-family: 'Syne', sans-serif;
  font-size: 12px;
  font-weight: 700;
  color: var(--text-primary);
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

.form-input {
  padding: 14px 18px;
  background: var(--bg-card);
  border: 1px solid var(--border-color);
  border-radius: 8px;
  color: var(--text-primary);
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  transition: all 0.3s ease;
}

.form-input:focus {
  outline: none;
  border-color: var(--gold-primary);
  background: var(--bg-accent);
  box-shadow: 0 0 0 3px rgba(212, 165, 116, 0.1);
}

.form-input::placeholder {
  color: var(--text-muted);
}

textarea.form-input {
  resize: vertical;
  min-height: 140px;
}

.form-submit {
  padding: 16px 32px;
  background: var(--gold-primary);
  color: var(--bg-dark);
  border: none;
  border-radius: 8px;
  font-family: 'Syne', sans-serif;
  font-size: 14px;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
  margin-top: 8px;
}

.form-submit:hover {
  background: var(--gold-bright);
  transform: translateY(-2px);
  box-shadow: 0 12px 24px rgba(245, 200, 95, 0.3);
}

/* ════════════════════════════════════════════════════════════ */
/* FOOTER */
/* ════════════════════════════════════════════════════════════ */

footer {
  background: var(--bg-dark);
  border-top: 1px solid var(--border-color);
  padding: 60px;
  display: grid;
  grid-template-columns: 2fr 1fr 1fr 1fr;
  gap: 60px;
}

.footer-brand {}

.footer-logo {
  height: 50px;
  width: auto;
  margin-bottom: 16px;
  object-fit: contain;
}

.footer-tagline {
  font-family: 'Syne', sans-serif;
  font-size: 12px;
  font-weight: 700;
  color: var(--gold-primary);
  letter-spacing: 0.15em;
  text-transform: uppercase;
  margin-bottom: 12px;
}

.footer-desc {
  font-size: 13px;
  color: var(--text-secondary);
  line-height: 1.7;
}

.footer-col-title {
  font-family: 'Syne', sans-serif;
  font-size: 12px;
  font-weight: 700;
  color: var(--text-primary);
  letter-spacing: 0.1em;
  text-transform: uppercase;
  margin-bottom: 20px;
}

.footer-links {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.footer-links a {
  font-size: 13px;
  color: var(--text-secondary);
  text-decoration: none;
  transition: all 0.3s ease;
  display: inline-flex;
  align-items: center;
  gap: 8px;
}

.footer-links a::before {
  content: '→';
  opacity: 0;
  transform: translateX(-8px);
  transition: all 0.3s ease;
}

.footer-links a:hover {
  color: var(--gold-primary);
}

.footer-links a:hover::before {
  opacity: 1;
  transform: translateX(0);
}

.footer-bottom {
  grid-column: 1 / -1;
  padding-top: 40px;
  border-top: 1px solid var(--border-color);
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 12px;
  color: var(--text-muted);
}

/* ════════════════════════════════════════════════════════════ */
/* RESPONSIVE */
/* ════════════════════════════════════════════════════════════ */

@media (max-width: 1024px) {
  nav { padding: 0 40px; }
  section { padding: 80px 40px; }
  .equipment-grid { grid-template-columns: 1fr; }
  .about-grid { grid-template-columns: 1fr; gap: 40px; }
  .contact-grid { grid-template-columns: 1fr; }
  footer { grid-template-columns: 1fr 1fr; }
}

@media (max-width: 768px) {
  nav { padding: 0 20px; }
  .nav-menu { display: none; }
  section { padding: 60px 20px; }
  .hero-logo { width: 180px; height: 180px; }
  .hero-stats { gap: 40px; }
  .srv-grid { grid-template-columns: 1fr; }
  .equipment-left { grid-template-columns: 1fr; }
  .contact-item { flex-direction: column; }
  footer { grid-template-columns: 1fr; gap: 40px; }
}
</style>
</head>
<body>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- NAVIGATION -->
<!-- ════════════════════════════════════════════════════════════ -->
<nav id="navbar">
  <a class="nav-logo-container" href="#">
    <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAgGBgcGBQgHBwcJCQgKDBQNDAsLDBkSEw8UHRofHh0aHBwgJC4nICIsIxwcKDcpLDAxNDQ0Hyc5PTgyPC4zNDL/2wBDAQkJCQwLDBgNDRgyIRwhMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjL/wAARCABQAFADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWm5ybnJ2eoqOkpaanqKmqsrO0tba2uLm6wsPExcbHyMnK0tPU1dbW2Nna4uPk5ebn6Onq8vP09fb2+Pn6/8QAHwEAAwEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlbaWmJmaoqOkpaanqKmqsrO0tba2uLm6wsPExcbHyMnK0tPU1dbW2Nna4uPk5ebn6Onq8vP09fb2+Pn6/9oADAMBAAIRAxEAPwD3+iiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD/2Q==" alt="BuggCloud Geomatics" class="nav-logo-img">
    <div class="nav-logo-text">
      <div class="nav-brand">BuggCloud</div>
      <div class="nav-tagline">Geomatics</div>
    </div>
  </a>
  <ul class="nav-menu">
    <li><a href="#services">Services</a></li>
    <li><a href="#equipment">Technology</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
  <a href="mailto:info@buggcloud.com" class="nav-cta">Get Quote</a>
</nav>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- HERO - CINEMATIC FULL SCREEN -->
<!-- ════════════════════════════════════════════════════════════ -->
<section class="hero">
  <div class="hero-bg-image">
    <div class="hero-bg-image"></div>
  </div>
  <div class="hero-construction-overlay"></div>

  <div class="hero-content">
    <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAgGBgcGBQgHBwcJCQgKDBQNDAsLDBkSEw8UHRofHh0aHBwgJC4nICIsIxwcKDcpLDAxNDQ0Hyc5PTgyPC4zNDL/2wBDAQkJCQwLDBgNDRgyIRwhMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjL/wAARCABQAFADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWm5ybnJ2eoqOkpaanqKmqsrO0tba2uLm6wsPExcbHyMnK0tPU1dbW2Nna4uPk5ebn6Onq8vP09fb2+Pn6/8QAHwEAAwEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlbaWmJmaoqOkpaanqKmqsrO0tba2uLm6wsPExcbHyMnK0tPU1dbW2Nna4uPk5ebn6Onq8vP09fb2+Pn6/9oADAMBAAIRAxEAPwD3+iiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD/2Q==" alt="BuggCloud Geomatics Logo" class="hero-logo">

    <div class="hero-eyebrow">Precision in Survey • Perfection in Results</div>

    <h1 class="hero-h1">Mapping the Future<br><span class="hero-h1-gold">With Precision.</span></h1>

    <p class="hero-subtitle">Professional Land Surveying, Drone Mapping, GIS Solutions & Infrastructure Surveys. Trusted by India's leading construction & development firms.</p>

    <div class="hero-cta-group">
      <a href="mailto:info@buggcloud.com" class="btn-primary">
        📞 Request a Quote
      </a>
      <a href="#services" class="btn-secondary">
        ↓ Explore Services
      </a>
    </div>

    <div class="hero-stats">
      <div class="stat">
        <div class="stat-number">500+</div>
        <div class="stat-label">Projects Delivered</div>
      </div>
      <div class="stat">
        <div class="stat-number">±5mm</div>
        <div class="stat-label">DGPS Accuracy</div>
      </div>
      <div class="stat">
        <div class="stat-number">15+</div>
        <div class="stat-label">Years Experience</div>
      </div>
    </div>
  </div>

  <div class="scroll-indicator">
    <div class="scroll-arrow"></div>
    <div class="scroll-text">Scroll to explore</div>
  </div>
</section>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- SERVICES -->
<!-- ════════════════════════════════════════════════════════════ -->
<section class="services" id="services">
  <div class="sec-label">What We Deliver</div>
  <h2 class="sec-h2">Professional Surveying <em>Services</em></h2>
  <p class="sec-desc">Complete geospatial solutions covering every aspect of land surveying, infrastructure mapping, and spatial intelligence.</p>

  <div class="srv-grid">
    <!-- Card 1 -->
    <div class="srv-card">
      <div class="srv-image">🎯 Land Survey & Total Station Mapping</div>
      <div class="srv-content">
        <div class="srv-icon">🗺️</div>
        <h3 class="srv-title">Land Surveys</h3>
        <ul class="srv-bullets">
          <li>Total Station Surveys</li>
          <li>Boundary Demarcation</li>
          <li>Layout Marking</li>
          <li>As-Built Surveys</li>
        </ul>
      </div>
    </div>

    <!-- Card 2 -->
    <div class="srv-card">
      <div class="srv-image">📡 DGPS & High-Precision Positioning</div>
      <div class="srv-content">
        <div class="srv-icon">📍</div>
        <h3 class="srv-title">DGPS Surveys</h3>
        <ul class="srv-bullets">
          <li>Sub-centimeter Accuracy</li>
          <li>Geospatial Data Collection</li>
          <li>RTK Positioning</li>
          <li>Real-time Corrections</li>
        </ul>
      </div>
    </div>

    <!-- Card 3 -->
    <div class="srv-card">
      <div class="srv-image">🌐 GIS Mapping & Spatial Analysis</div>
      <div class="srv-content">
        <div class="srv-icon">🧭</div>
        <h3 class="srv-title">GIS Mapping</h3>
        <ul class="srv-bullets">
          <li>Multi-layer Mapping</li>
          <li>Data Visualization</li>
          <li>Spatial Analysis</li>
          <li>AutoCAD Drafting</li>
        </ul>
      </div>
    </div>

    <!-- Card 4 -->
    <div class="srv-card">
      <div class="srv-image">🚁 Aerial Drone Surveys & 4K Mapping</div>
      <div class="srv-content">
        <div class="srv-icon">🛸</div>
        <h3 class="srv-title">Drone Solutions</h3>
        <ul class="srv-bullets">
          <li>4K Aerial Mapping</li>
          <li>3D Terrain Models</li>
          <li>Orthomosaics</li>
          <li>Volume Calculations</li>
        </ul>
      </div>
    </div>

    <!-- Card 5 -->
    <div class="srv-card">
      <div class="srv-image">🏗️ Infrastructure & Government Projects</div>
      <div class="srv-content">
        <div class="srv-icon">🏛️</div>
        <h3 class="srv-title">Infrastructure</h3>
        <ul class="srv-bullets">
          <li>Road & Rail Projects</li>
          <li>Highway Surveys</li>
          <li>HMDA/DTCP Works</li>
          <li>Construction Monitoring</li>
        </ul>
      </div>
    </div>

    <!-- Card 6 -->
    <div class="srv-card">
      <div class="srv-image">📊 Topographic & Site Analysis</div>
      <div class="srv-content">
        <div class="srv-icon">📐</div>
        <h3 class="srv-title">Topographic Surveys</h3>
        <ul class="srv-bullets">
          <li>Contour Mapping</li>
          <li>Site Analysis</li>
          <li>Terrain Modeling</li>
          <li>Engineering Studies</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- EQUIPMENT & TECHNOLOGY -->
<!-- ════════════════════════════════════════════════════════════ -->
<section class="equipment-showcase" id="equipment">
  <div class="sec-label">Advanced Technology</div>
  <h2 class="sec-h2">World-Class <em>Equipment</em></h2>

  <div class="equipment-grid">
    <div class="equipment-left">
      <div class="equipment-item">
        <div class="equipment-label">Total Station</div>
      </div>
      <div class="equipment-item">
        <div class="equipment-label">DGPS Receiver</div>
      </div>
      <div class="equipment-item">
        <div class="equipment-label">Drone Fleet (4K)</div>
      </div>
      <div class="equipment-item">
        <div class="equipment-label">GIS Software Suite</div>
      </div>
    </div>

    <div class="equipment-right">
      <p class="equipment-desc">Our arsenal includes the latest surveying instruments from Trimble, Leica, and DJI — ensuring millimeter-level accuracy and enterprise-grade results.</p>

      <div class="equipment-features">
        <div class="feature">
          <div class="feature-icon">⚡</div>
          <div class="feature-text">
            <div class="feature-title">Real-Time RTK Corrections</div>
            <div class="feature-desc">Sub-centimeter accuracy through real-time kinematic positioning systems</div>
          </div>
        </div>
        <div class="feature">
          <div class="feature-icon">📸</div>
          <div class="feature-text">
            <div class="feature-title">4K Aerial Imaging</div>
            <div class="feature-desc">Enterprise drones with millimeter-resolution orthomosaic generation</div>
          </div>
        </div>
        <div class="feature">
          <div class="feature-icon">💾</div>
          <div class="feature-text">
            <div class="feature-title">Cloud Processing</div>
            <div class="feature-desc">Rapid 3D model generation, volume calculations, and GIS integration</div>
          </div>
        </div>
        <div class="feature">
          <div class="feature-icon">🔒</div>
          <div class="feature-text">
            <div class="feature-title">Enterprise Compliance</div>
            <div class="feature-desc">TG Government licensed, ISO-certified workflows, audit trails</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- STATS -->
<!-- ════════════════════════════════════════════════════════════ -->
<section class="stats-showcase">
  <div class="stats-grid">
    <div class="stat-card">
      <div class="stat-big">500+</div>
      <div class="stat-small">Projects Delivered</div>
    </div>
    <div class="stat-card">
      <div class="stat-big">15+</div>
      <div class="stat-small">Years Experience</div>
    </div>
    <div class="stat-card">
      <div class="stat-big">2000+</div>
      <div class="stat-small">Happy Clients</div>
    </div>
    <div class="stat-card">
      <div class="stat-big">100%</div>
      <div class="stat-small">On-Time Delivery</div>
    </div>
  </div>
</section>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- ABOUT -->
<!-- ════════════════════════════════════════════════════════════ -->
<section class="about" id="about">
  <div class="sec-label">Who We Are</div>
  <h2 class="sec-h2">Why <em>BuggCloud</em></h2>

  <div class="about-grid">
    <div class="about-content">
      <p class="sec-desc">TG Government Licensed Surveyors with expertise in geospatial intelligence, infrastructure mapping, and precision surveying.</p>

      <div class="about-points">
        <div class="point">
          <div class="point-num">01</div>
          <div class="point-text">
            <div class="point-title">TG Licensed & Verified</div>
            <div class="point-desc">Certified Telangana Government Licensed Surveyors with complete legal compliance for all government and institutional projects.</div>
          </div>
        </div>
        <div class="point">
          <div class="point-num">02</div>
          <div class="point-text">
            <div class="point-title">Drone + Ground Integration</div>
            <div class="point-desc">Combine 4K aerial UAV data with DGPS/Total Station ground truth for unparalleled accuracy and coverage.</div>
          </div>
        </div>
        <div class="point">
          <div class="point-num">03</div>
          <div class="point-text">
            <div class="point-title">End-to-End Solutions</div>
            <div class="point-desc">From field acquisition to GIS deliverables, CAD drawings, and official reports—everything under one roof in Secunderabad.</div>
          </div>
        </div>
        <div class="point">
          <div class="point-num">04</div>
          <div class="point-text">
            <div class="point-title">HMDA/DTCP Specialists</div>
            <div class="point-desc">Deep expertise in government works, layout approvals, and infrastructure projects across the Hyderabad metro region.</div>
          </div>
        </div>
      </div>
    </div>

    <div class="about-image">
      🏗️ [Professional Surveyor on Construction Site - High Resolution Photo]
    </div>
  </div>
</section>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- CONTACT -->
<!-- ════════════════════════════════════════════════════════════ -->
<section class="contact" id="contact">
  <div class="sec-label">Get In Touch</div>
  <h2 class="sec-h2">Start Your <em>Survey Project</em></h2>

  <div class="contact-grid">
    <div class="contact-info">
      <p class="sec-desc">Located in East Marredpally, Secunderabad. We respond within one business day.</p>

      <div class="contact-items">
        <div class="contact-item">
          <div class="contact-icon">📞</div>
          <div class="contact-text">
            <div class="contact-label">Phone</div>
            <div class="contact-value">+91 6305155099 • +91 9100539972</div>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">✉️</div>
          <div class="contact-text">
            <div class="contact-label">Email</div>
            <div class="contact-value">info@buggcloud.com</div>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-icon">📍</div>
          <div class="contact-text">
            <div class="contact-label">Office</div>
            <div class="contact-value">East Marredpally, Secunderabad, Telangana</div>
          </div>
        </div>
      </div>
    </div>

    <form class="contact-form" onsubmit="event.preventDefault(); alert('Thank you! We will contact you within 24 hours.'); this.reset();">
      <div class="form-group">
        <label class="form-label">Full Name *</label>
        <input type="text" class="form-input" placeholder="Your name" required>
      </div>
      <div class="form-group">
        <label class="form-label">Email *</label>
        <input type="email" class="form-input" placeholder="your@company.com" required>
      </div>
      <div class="form-group">
        <label class="form-label">Service Required *</label>
        <select class="form-input" required>
          <option value="">Select a service…</option>
          <option>Land Survey / Total Station</option>
          <option>DGPS Surveys</option>
          <option>GIS Mapping</option>
          <option>Drone Solutions</option>
          <option>Infrastructure Surveys</option>
          <option>Topographic Surveys</option>
          <option>Government Works (HMDA/DTCP)</option>
          <option>Other</option>
        </select>
      </div>
      <div class="form-group">
        <label class="form-label">Project Details</label>
        <textarea class="form-input" placeholder="Describe your project, location, and timeline…"></textarea>
      </div>
      <button type="submit" class="form-submit">Submit Enquiry →</button>
    </form>
  </div>
</section>

<!-- ════════════════════════════════════════════════════════════ -->
<!-- FOOTER -->
<!-- ════════════════════════════════════════════════════════════ -->
<footer>
  <div class="footer-brand">
    <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAgGBgcGBQgHBwcJCQgKDBQNDAsLDBkSEw8UHRofHh0aHBwgJC4nICIsIxwcKDcpLDAxNDQ0Hyc5PTgyPC4zNDL/2wBDAQkJCQwLDBgNDRgyIRwhMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjL/wAARCABQAFADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWm5ybnJ2eoqOkpaanqKmqsrO0tba2uLm6wsPExcbHyMnK0tPU1dbW2Nna4uPk5ebn6Onq8vP09fb2+Pn6/8QAHwEAAwEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlbaWmJmaoqOkpaanqKmqsrO0tba2uLm6wsPExcbHyMnK0tPU1dbW2Nna4uPk5ebn6Onq8vP09fb2+Pn6/9oADAMBAAIRAxEAPwD3+iiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD/2Q==" alt="BuggCloud Geomatics" class="footer-logo">
    <div class="footer-tagline">Precision in Survey • Perfection in Results</div>
    <p class="footer-desc">TG Government Licensed Surveyors delivering enterprise-grade geospatial solutions across Telangana and India.</p>
  </div>

  <div>
    <div class="footer-col-title">Services</div>
    <ul class="footer-links">
      <li><a href="#services">Land Surveys</a></li>
      <li><a href="#services">DGPS Surveys</a></li>
      <li><a href="#services">GIS Mapping</a></li>
      <li><a href="#services">Drone Solutions</a></li>
      <li><a href="#services">Infrastructure</a></li>
    </ul>
  </div>

  <div>
    <div class="footer-col-title">Company</div>
    <ul class="footer-links">
      <li><a href="#about">About Us</a></li>
      <li><a href="#equipment">Technology</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="https://www.linkedin.com/company/buggcloud-geomatics-land-surveyors" target="_blank">LinkedIn</a></li>
    </ul>
  </div>

  <div>
    <div class="footer-col-title">Connect</div>
    <ul class="footer-links">
      <li><a href="mailto:info@buggcloud.com">info@buggcloud.com</a></li>
      <li><a href="tel:+916305155099">+91 6305155099</a></li>
      <li><a href="tel:+919100539972">+91 9100539972</a></li>
      <li><a href="#">LinkedIn Geomatics</a></li>
    </ul>
  </div>

  <div class="footer-bottom">
    <p>© 2026 BuggCloud Geomatics & Land Surveyors. All rights reserved.</p>
    <p>East Marredpally, Secunderabad, Telangana, India</p>
  </div>
</footer>

<script>
// Sticky nav on scroll
const navbar = document.getElementById('navbar');
window.addEventListener('scroll', () => {
  if (window.scrollY > 100) {
    navbar.classList.add('scrolled');
  } else {
    navbar.classList.remove('scrolled');
  }
});

// Smooth scroll for links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function (e) {
    const href = this.getAttribute('href');
    if (href !== '#') {
      e.preventDefault();
      const target = document.querySelector(href);
      if (target) {
        target.scrollIntoView({ behavior: 'smooth' });
      }
    }
  });
});

// Intersection Observer for fade-in animations
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

document.querySelectorAll('.srv-card, .point, .stat-card').forEach(el => {
  el.style.opacity = '0';
  el.style.transform = 'translateY(20px)';
  el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
  observer.observe(el);
});
</script>

</body>
</html>
