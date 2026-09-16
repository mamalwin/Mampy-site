<!DOCTYPE html>
<html lang="fa" dir="rtl" data-theme="dark">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MAMPY Helper | راهنمای جامع</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;600;700;800;900&family=Orbitron:wght@400;500;700;900&display=swap" rel="stylesheet">
<style>
:root{
  --navy-1:#050a1f;
  --navy-2:#0a1428;
  --navy-3:#0f1e3d;
  --navy-4:#152a52;
  --accent-1:#64c8ff;
  --accent-2:#4a9eff;
  --accent-3:#8b5cf6;
  --accent-4:#ec4899;
  --gold:#ffd166;
  --green:#4ade80;
  --red:#f87171;
  --text-primary:#e8f1ff;
  --text-secondary:#aac8ff;
  --text-muted:#6688aa;
  --card-bg:rgba(255,255,255,0.05);
  --card-border:rgba(100,200,255,0.18);
  --card-hover:rgba(100,200,255,0.12);
  --glass:rgba(10,20,40,0.55);
  --glass-strong:rgba(5,10,25,0.85);
  --shadow:0 8px 40px rgba(0,0,0,0.5);
  --shadow-glow:0 0 30px rgba(100,200,255,0.3);
  --transition:all 0.35s cubic-bezier(0.4,0,0.2,1);
}
[data-theme="light"]{
  --navy-1:#f0f4ff;
  --navy-2:#e4ecff;
  --navy-3:#d6e2ff;
  --navy-4:#c8d8ff;
  --accent-1:#2563eb;
  --accent-2:#3b82f6;
  --accent-3:#7c3aed;
  --accent-4:#db2777;
  --text-primary:#0a1428;
  --text-secondary:#1e3a8a;
  --text-muted:#4b5563;
  --card-bg:rgba(255,255,255,0.75);
  --card-border:rgba(37,99,235,0.25);
  --card-hover:rgba(37,99,235,0.12);
  --glass:rgba(255,255,255,0.7);
  --glass-strong:rgba(255,255,255,0.92);
  --shadow:0 8px 40px rgba(37,99,235,0.15);
  --shadow-glow:0 0 30px rgba(37,99,235,0.25);
}
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{
  font-family:'Vazirmatn',sans-serif;
  background:var(--navy-1);
  color:var(--text-primary);
  min-height:100vh;
  overflow-x:hidden;
  position:relative;
  transition:background 0.5s ease,color 0.5s ease;
}
[dir="ltr"] body{font-family:'Vazirmatn','Orbitron',sans-serif}
#starfield{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:100%;
  z-index:0;
  pointer-events:none;
}
.bg-orbs{
  position:fixed;
  top:0;left:0;
  width:100%;height:100%;
  z-index:1;
  pointer-events:none;
  overflow:hidden;
}
.orb{
  position:absolute;
  border-radius:50%;
  filter:blur(80px);
  opacity:0.35;
  animation:float 20s ease-in-out infinite;
}
.orb-1{width:500px;height:500px;background:radial-gradient(circle,var(--accent-1),transparent 70%);top:-150px;left:-100px;animation-delay:0s}
.orb-2{width:400px;height:400px;background:radial-gradient(circle,var(--accent-3),transparent 70%);bottom:-100px;right:-100px;animation-delay:-7s}
.orb-3{width:350px;height:350px;background:radial-gradient(circle,var(--accent-4),transparent 70%);top:40%;left:60%;animation-delay:-14s}
@keyframes float{
  0%,100%{transform:translate(0,0) scale(1)}
  33%{transform:translate(50px,-30px) scale(1.1)}
  66%{transform:translate(-30px,40px) scale(0.95)}
}
.container{
  position:relative;
  z-index:10;
  max-width:1300px;
  margin:0 auto;
  padding:0 20px;
}
header.top-bar{
  position:fixed;
  top:0;
  left:0;
  right:0;
  z-index:100;
  backdrop-filter:blur(20px);
  -webkit-backdrop-filter:blur(20px);
  background:var(--glass);
  border-bottom:1px solid var(--card-border);
  transition:var(--transition);
}
.top-bar-inner{
  max-width:1300px;
  margin:0 auto;
  padding:14px 20px;
  display:flex;
  justify-content:space-between;
  align-items:center;
  gap:16px;
}
.brand{
  display:flex;
  align-items:center;
  gap:12px;
  text-decoration:none;
  color:var(--text-primary);
}
.brand-logo{
  width:44px;
  height:44px;
  border-radius:14px;
  background:linear-gradient(135deg,var(--accent-1),var(--accent-3));
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:24px;
  box-shadow:var(--shadow-glow);
  animation:pulse-glow 3s ease-in-out infinite;
}
@keyframes pulse-glow{
  0%,100%{box-shadow:0 0 20px rgba(100,200,255,0.4)}
  50%{box-shadow:0 0 40px rgba(100,200,255,0.8)}
}
.brand-text{display:flex;flex-direction:column;line-height:1.1}
.brand-title{font-weight:900;font-size:18px;letter-spacing:0.5px;background:linear-gradient(90deg,var(--accent-1),var(--accent-3));-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text}
.brand-sub{font-size:11px;color:var(--text-muted);font-weight:500}
.top-actions{display:flex;align-items:center;gap:10px}
.icon-btn{
  width:42px;height:42px;
  border-radius:12px;
  border:1px solid var(--card-border);
  background:var(--card-bg);
  color:var(--text-primary);
  cursor:pointer;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:18px;
  transition:var(--transition);
  position:relative;
  overflow:hidden;
}
.icon-btn:hover{
  background:var(--card-hover);
  transform:translateY(-2px);
  box-shadow:var(--shadow-glow);
}
.lang-btn{
  width:auto;
  padding:0 16px;
  font-weight:700;
  font-size:13px;
  gap:8px;
}
.lang-flag{font-size:16px}
.hero{
  padding:140px 0 60px;
  text-align:center;
  position:relative;
}
.hero-badge{
  display:inline-flex;
  align-items:center;
  gap:8px;
  padding:8px 18px;
  border-radius:50px;
  background:var(--card-bg);
  border:1px solid var(--card-border);
  font-size:13px;
  font-weight:600;
  color:var(--text-secondary);
  margin-bottom:24px;
  backdrop-filter:blur(10px);
  animation:fadeInDown 0.8s ease;
}
.hero-badge .dot{
  width:8px;height:8px;
  border-radius:50%;
  background:var(--green);
  box-shadow:0 0 10px var(--green);
  animation:blink 1.5s ease-in-out infinite;
}
@keyframes blink{0%,100%{opacity:1}50%{opacity:0.3}}
.hero-title{
  font-size:clamp(36px,6vw,72px);
  font-weight:900;
  line-height:1.15;
  margin-bottom:20px;
  background:linear-gradient(135deg,var(--text-primary) 0%,var(--accent-1) 50%,var(--accent-3) 100%);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
  background-clip:text;
  animation:fadeInDown 0.9s ease;
}
.hero-subtitle{
  font-size:clamp(15px,2vw,19px);
  color:var(--text-secondary);
  max-width:720px;
  margin:0 auto 36px;
  line-height:1.9;
  font-weight:400;
  animation:fadeInDown 1s ease;
}
.hero-buttons{
  display:flex;
  gap:14px;
  justify-content:center;
  flex-wrap:wrap;
  animation:fadeInUp 1.1s ease;
}
.btn{
  padding:14px 32px;
  border-radius:14px;
  border:none;
  font-family:inherit;
  font-size:15px;
  font-weight:700;
  cursor:pointer;
  transition:var(--transition);
  text-decoration:none;
  display:inline-flex;
  align-items:center;
  gap:10px;
  position:relative;
  overflow:hidden;
}
.btn-primary{
  background:linear-gradient(135deg,var(--accent-1),var(--accent-3));
  color:#fff;
  box-shadow:0 8px 30px rgba(100,200,255,0.35);
}
.btn-primary:hover{
  transform:translateY(-3px);
  box-shadow:0 15px 45px rgba(100,200,255,0.55);
}
.btn-ghost{
  background:var(--card-bg);
  color:var(--text-primary);
  border:1px solid var(--card-border);
  backdrop-filter:blur(10px);
}
.btn-ghost:hover{
  background:var(--card-hover);
  transform:translateY(-3px);
  box-shadow:var(--shadow-glow);
}
@keyframes fadeInDown{from{opacity:0;transform:translateY(-30px)}to{opacity:1;transform:translateY(0)}}
@keyframes fadeInUp{from{opacity:0;transform:translateY(30px)}to{opacity:1;transform:translateY(0)}}
.stats-row{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
  gap:20px;
  margin:70px 0 40px;
  animation:fadeInUp 1.2s ease;
}
.stat-card{
  background:var(--card-bg);
  border:1px solid var(--card-border);
  border-radius:20px;
  padding:28px 24px;
  backdrop-filter:blur(15px);
  -webkit-backdrop-filter:blur(15px);
  transition:var(--transition);
  position:relative;
  overflow:hidden;
}
.stat-card::before{
  content:'';
  position:absolute;
  top:0;left:0;
  width:100%;height:3px;
  background:linear-gradient(90deg,transparent,var(--accent-1),transparent);
  opacity:0;
  transition:var(--transition);
}
.stat-card:hover::before{opacity:1}
.stat-card:hover{
  transform:translateY(-6px);
  border-color:var(--accent-1);
  box-shadow:0 20px 50px rgba(100,200,255,0.25);
  background:var(--card-hover);
}
.stat-icon{font-size:32px;margin-bottom:12px;display:block}
.stat-value{font-size:32px;font-weight:900;color:var(--accent-1);margin-bottom:6px;font-family:'Orbitron','Vazirmatn',sans-serif}
.stat-label{font-size:13px;color:var(--text-muted);font-weight:600}
.section{
  padding:70px 0;
  position:relative;
}
.section-header{
  text-align:center;
  margin-bottom:50px;
}
.section-tag{
  display:inline-block;
  padding:6px 16px;
  border-radius:50px;
  background:var(--card-bg);
  border:1px solid var(--card-border);
  color:var(--accent-1);
  font-size:12px;
  font-weight:700;
  letter-spacing:1px;
  text-transform:uppercase;
  margin-bottom:16px;
}
.section-title{
  font-size:clamp(26px,4vw,42px);
  font-weight:900;
  margin-bottom:14px;
  background:linear-gradient(135deg,var(--text-primary),var(--accent-1));
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
  background-clip:text;
}
.section-desc{
  color:var(--text-secondary);
  font-size:16px;
  max-width:620px;
  margin:0 auto;
  line-height:1.9;
}
.search-wrap{
  max-width:600px;
  margin:0 auto 40px;
  position:relative;
}
.search-input{
  width:100%;
  padding:18px 56px 18px 24px;
  border-radius:16px;
  border:1px solid var(--card-border);
  background:var(--card-bg);
  color:var(--text-primary);
  font-family:inherit;
  font-size:15px;
  outline:none;
  transition:var(--transition);
  backdrop-filter:blur(15px);
}
[dir="ltr"] .search-input{padding:18px 24px 18px 56px}
.search-input:focus{
  border-color:var(--accent-1);
  box-shadow:0 0 0 4px rgba(100,200,255,0.15);
}
.search-input::placeholder{color:var(--text-muted)}
.search-icon{
  position:absolute;
  right:20px;
  top:50%;
  transform:translateY(-50%);
  font-size:20px;
  color:var(--text-muted);
  pointer-events:none;
}
[dir="ltr"] .search-icon{right:auto;left:20px}
.categories{
  display:flex;
  gap:10px;
  flex-wrap:wrap;
  justify-content:center;
  margin-bottom:40px;
}
.cat-btn{
  padding:10px 20px;
  border-radius:50px;
  border:1px solid var(--card-border);
  background:var(--card-bg);
  color:var(--text-secondary);
  font-family:inherit;
  font-size:13px;
  font-weight:600;
  cursor:pointer;
  transition:var(--transition);
  display:flex;
  align-items:center;
  gap:8px;
  backdrop-filter:blur(10px);
}
.cat-btn:hover{
  background:var(--card-hover);
  color:var(--text-primary);
  transform:translateY(-2px);
}
.cat-btn.active{
  background:linear-gradient(135deg,var(--accent-1),var(--accent-3));
  color:#fff;
  border-color:transparent;
  box-shadow:0 8px 25px rgba(100,200,255,0.4);
}
.help-grid{
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(340px,1fr));
  gap:22px;
}
.help-card{
  background:var(--card-bg);
  border:1px solid var(--card-border);
  border-radius:20px;
  padding:26px 24px;
  backdrop-filter:blur(15px);
  -webkit-backdrop-filter:blur(15px);
  transition:var(--transition);
  cursor:pointer;
  position:relative;
  overflow:hidden;
  animation:fadeInUp 0.5s ease backwards;
}
.help-card::after{
  content:'';
  position:absolute;
  top:0;left:-100%;
  width:100%;height:100%;
  background:linear-gradient(90deg,transparent,rgba(100,200,255,0.08),transparent);
  transition:left 0.6s ease;
  pointer-events:none;
}
.help-card:hover::after{left:100%}
.help-card:hover{
  transform:translateY(-6px);
  border-color:var(--accent-1);
  box-shadow:0 20px 50px rgba(100,200,255,0.2);
  background:var(--card-hover);
}
.help-card-head{
  display:flex;
  align-items:center;
  gap:14px;
  margin-bottom:14px;
}
.help-icon{
  width:48px;height:48px;
  border-radius:14px;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:24px;
  flex-shrink:0;
  background:linear-gradient(135deg,rgba(100,200,255,0.15),rgba(139,92,246,0.15));
  border:1px solid var(--card-border);
}
.help-card-title{
  font-size:17px;
  font-weight:800;
  color:var(--text-primary);
  line-height:1.3;
}
.help-card-desc{
  font-size:13.5px;
  color:var(--text-secondary);
  line-height:1.9;
  margin-bottom:16px;
}
.help-cmds{
  display:flex;
  flex-direction:column;
  gap:8px;
  padding-top:14px;
  border-top:1px dashed var(--card-border);
}
.cmd-line{
  display:flex;
  align-items:center;
  gap:10px;
  font-size:13px;
  color:var(--text-secondary);
  direction:ltr;
  text-align:left;
  font-family:'Orbitron','Vazirmatn',monospace;
}
.cmd-line .cm-key{
  color:var(--accent-1);
  font-weight:700;
}
.cmd-line .cm-arrow{color:var(--text-muted)}
.cmd-line .cm-val{color:var(--text-primary)}
.modal-overlay{
  position:fixed;
  inset:0;
  background:rgba(0,0,0,0.7);
  backdrop-filter:blur(8px);
  z-index:200;
  display:none;
  align-items:center;
  justify-content:center;
  padding:20px;
  opacity:0;
  transition:opacity 0.3s ease;
}
.modal-overlay.active{display:flex;opacity:1}
.modal{
  background:var(--glass-strong);
  border:1px solid var(--card-border);
  border-radius:24px;
  max-width:680px;
  width:100%;
  max-height:85vh;
  overflow-y:auto;
  padding:36px;
  position:relative;
  backdrop-filter:blur(30px);
  animation:modalIn 0.4s cubic-bezier(0.34,1.56,0.64,1);
  box-shadow:0 30px 80px rgba(0,0,0,0.6);
}
@keyframes modalIn{from{opacity:0;transform:scale(0.9) translateY(20px)}to{opacity:1;transform:scale(1) translateY(0)}}
.modal-close{
  position:absolute;
  top:18px;
  left:18px;
  width:38px;height:38px;
  border-radius:10px;
  border:1px solid var(--card-border);
  background:var(--card-bg);
  color:var(--text-primary);
  cursor:pointer;
  font-size:18px;
  transition:var(--transition);
  display:flex;
  align-items:center;
  justify-content:center;
}
[dir="ltr"] .modal-close{left:auto;right:18px}
.modal-close:hover{background:var(--red);color:#fff;border-color:var(--red)}
.modal-head{
  display:flex;
  align-items:center;
  gap:16px;
  margin-bottom:22px;
  padding-bottom:20px;
  border-bottom:1px solid var(--card-border);
}
.modal-icon{
  width:60px;height:60px;
  border-radius:18px;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:30px;
  background:linear-gradient(135deg,rgba(100,200,255,0.2),rgba(139,92,246,0.2));
  border:1px solid var(--card-border);
  flex-shrink:0;
}
.modal-title{font-size:22px;font-weight:900;color:var(--text-primary)}
.modal-body{
  font-size:15px;
  color:var(--text-secondary);
  line-height:2.2;
}
.modal-body h4{
  color:var(--accent-1);
  font-size:15px;
  margin:18px 0 10px;
  font-weight:800;
}
.modal-body p{margin-bottom:10px}
.modal-body code{
  background:rgba(100,200,255,0.12);
  color:var(--accent-1);
  padding:3px 10px;
  border-radius:8px;
  font-family:'Orbitron','Vazirmatn',monospace;
  font-size:13px;
  direction:ltr;
  display:inline-block;
  border:1px solid rgba(100,200,255,0.2);
}
.modal-body .cmd-block{
  background:rgba(0,0,0,0.25);
  border:1px solid var(--card-border);
  border-radius:12px;
  padding:14px 18px;
  margin:10px 0;
  direction:ltr;
  text-align:left;
  font-family:'Orbitron','Vazirmatn',monospace;
  font-size:13px;
  color:var(--text-primary);
  overflow-x:auto;
}
[data-theme="light"] .modal-body .cmd-block{background:rgba(0,0,0,0.05)}
.creator-section{
  background:linear-gradient(135deg,rgba(100,200,255,0.06),rgba(139,92,246,0.06));
  border:1px solid var(--card-border);
  border-radius:26px;
  padding:50px 40px;
  margin:40px 0;
  backdrop-filter:blur(15px);
  position:relative;
  overflow:hidden;
}
.creator-section::before{
  content:'';
  position:absolute;
  top:-50%;right:-10%;
  width:400px;height:400px;
  background:radial-gradient(circle,rgba(100,200,255,0.15),transparent 70%);
  pointer-events:none;
}
.creator-inner{
  display:grid;
  grid-template-columns:auto 1fr;
  gap:36px;
  align-items:center;
  position:relative;
  z-index:1;
}
.creator-avatar{
  width:130px;height:130px;
  border-radius:32px;
  background:linear-gradient(135deg,var(--accent-1),var(--accent-3),var(--accent-4));
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:64px;
  box-shadow:0 20px 60px rgba(100,200,255,0.4);
  animation:pulse-glow 4s ease-in-out infinite;
  position:relative;
}
.creator-avatar::after{
  content:'';
  position:absolute;
  inset:-4px;
  border-radius:36px;
  background:linear-gradient(135deg,var(--accent-1),var(--accent-3),var(--accent-4));
  z-index:-1;
  filter:blur(15px);
  opacity:0.6;
}
.creator-name{
  font-size:28px;
  font-weight:900;
  margin-bottom:8px;
  background:linear-gradient(135deg,var(--accent-1),var(--accent-3));
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
  background-clip:text;
}
.creator-role{
  color:var(--accent-1);
  font-size:14px;
  font-weight:700;
  margin-bottom:14px;
}
.creator-bio{
  color:var(--text-secondary);
  font-size:14.5px;
  line-height:2;
  margin-bottom:20px;
}
.creator-links{
  display:flex;
  gap:10px;
  flex-wrap:wrap;
}
.creator-link{
  display:inline-flex;
  align-items:center;
  gap:8px;
  padding:9px 18px;
  border-radius:12px;
  background:var(--card-bg);
  border:1px solid var(--card-border);
  color:var(--text-primary);
  text-decoration:none;
  font-size:13px;
  font-weight:600;
  transition:var(--transition);
}
.creator-link:hover{
  background:var(--card-hover);
  transform:translateY(-3px);
  box-shadow:var(--shadow-glow);
  border-color:var(--accent-1);
}
footer{
  padding:50px 0 30px;
  text-align:center;
  border-top:1px solid var(--card-border);
  margin-top:60px;
  position:relative;
  z-index:10;
}
.footer-text{
  color:var(--text-muted);
  font-size:13.5px;
  line-height:2;
}
.footer-heart{color:var(--accent-4);animation:heartbeat 1.5s ease-in-out infinite;display:inline-block}
@keyframes heartbeat{0%,100%{transform:scale(1)}50%{transform:scale(1.2)}}
.footer-version{
  display:inline-block;
  margin-top:12px;
  padding:6px 16px;
  border-radius:50px;
  background:var(--card-bg);
  border:1px solid var(--card-border);
  color:var(--accent-1);
  font-size:12px;
  font-weight:700;
  font-family:'Orbitron',sans-serif;
}
.no-results{
  text-align:center;
  padding:60px 20px;
  color:var(--text-muted);
  grid-column:1/-1;
}
.no-results-icon{font-size:60px;margin-bottom:16px;opacity:0.5}
.to-top{
  position:fixed;
  bottom:30px;
  left:30px;
  width:48px;height:48px;
  border-radius:14px;
  background:linear-gradient(135deg,var(--accent-1),var(--accent-3));
  color:#fff;
  border:none;
  cursor:pointer;
  font-size:20px;
  display:flex;
  align-items:center;
  justify-content:center;
  box-shadow:0 10px 30px rgba(100,200,255,0.4);
  opacity:0;
  pointer-events:none;
  transition:var(--transition);
  z-index:90;
}
[dir="ltr"] .to-top{left:auto;right:30px}
.to-top.show{opacity:1;pointer-events:auto}
.to-top:hover{transform:translateY(-4px) scale(1.05)}
@media (max-width:768px){
  .hero{padding:120px 0 40px}
  .creator-inner{grid-template-columns:1fr;text-align:center;gap:24px}
  .creator-avatar{margin:0 auto;width:110px;height:110px;font-size:54px}
  .creator-links{justify-content:center}
  .help-grid{grid-template-columns:1fr}
  .modal{padding:26px 20px}
  .brand-sub{display:none}
  .top-bar-inner{padding:12px 14px}
  .lang-btn{padding:0 12px;font-size:12px}
  .icon-btn{width:38px;height:38px;font-size:16px}
}
::-webkit-scrollbar{width:10px;height:10px}
::-webkit-scrollbar-track{background:var(--navy-2)}
::-webkit-scrollbar-thumb{background:linear-gradient(180deg,var(--accent-1),var(--accent-3));border-radius:10px;border:2px solid var(--navy-2)}
::-webkit-scrollbar-thumb:hover{background:var(--accent-1)}
.modal::-webkit-scrollbar{width:8px}
.modal::-webkit-scrollbar-thumb{background:var(--accent-1);border-radius:8px}
</style>
</head>
<body>

<canvas id="starfield"></canvas>
<div class="bg-orbs">
  <div class="orb orb-1"></div>
  <div class="orb orb-2"></div>
  <div class="orb orb-3"></div>
</div>

<header class="top-bar">
  <div class="top-bar-inner">
    <a href="#" class="brand">
      <div class="brand-logo">🤖</div>
      <div class="brand-text">
        <span class="brand-title">MAMPY Helper</span>
        <span class="brand-sub" data-i18n="brandSub">دستیار هوشمند مدیریت گروه</span>
      </div>
    </a>
    <div class="top-actions">
      <button class="icon-btn lang-btn" id="langToggle" title="Change Language">
        <span class="lang-flag" id="langFlag">🇮🇷</span>
        <span id="langLabel">FA</span>
      </button>
      <button class="icon-btn" id="themeToggle" title="Toggle Theme">
        <span id="themeIcon">🌙</span>
      </button>
    </div>
  </div>
</header>

<main class="container">

  <section class="hero">
    <div class="hero-badge">
      <span class="dot"></span>
      <span data-i18n="heroBadge">نسخه 1.7.0 — به‌روز و پایدار</span>
    </div>
    <h1 class="hero-title" data-i18n="heroTitle">MAMPY Helper</h1>
    <p class="hero-subtitle" data-i18n="heroSubtitle">
      ربات حرفه‌ای مدیریت گروه در پیام‌رسان بله. با قفل‌های پیشرفته، سیستم اخطار، مجازات هوشمند، بازی‌های سرگرم‌کننده و ده‌ها قابلیت دیگر، تجربه‌ای بی‌نظیر از مدیریت گروه را رقم بزنید.
    </p>
    <div class="hero-buttons">
      <a href="#help" class="btn btn-primary">
        <span>📚</span>
        <span data-i18n="btnGuide">مشاهده راهنمای کامل</span>
      </a>
      <a href="https://ble.ir/MAMPY_Helper_Bot" target="_blank" class="btn btn-ghost">
        <span>🚀</span>
        <span data-i18n="btnStart">شروع استفاده از ربات</span>
      </a>
    </div>
  </section>

  <section class="stats-row">
    <div class="stat-card">
      <span class="stat-icon">🔐</span>
      <div class="stat-value">25+</div>
      <div class="stat-label" data-i18n="statLocks">قفل پیشرفته</div>
    </div>
    <div class="stat-card">
      <span class="stat-icon">⚡</span>
      <div class="stat-value">80+</div>
      <div class="stat-label" data-i18n="statCommands">دستور کاربردی</div>
    </div>
    <div class="stat-card">
      <span class="stat-icon">🎮</span>
      <div class="stat-value">3</div>
      <div class="stat-label" data-i18n="statGames">بازی سرگرم‌کننده</div>
    </div>
    <div class="stat-card">
      <span class="stat-icon">💎</span>
      <div class="stat-value">7+</div>
      <div class="stat-label" data-i18n="statVip">قابلیت VIP</div>
    </div>
  </section>

  <section class="section" id="help">
    <div class="section-header">
      <span class="section-tag" data-i18n="tagHelp">راهنمای جامع</span>
      <h2 class="section-title" data-i18n="titleHelp">همه دستورات در یک نگاه</h2>
      <p class="section-desc" data-i18n="descHelp">دسته‌بندی شده، جستجوپذیر و کامل. کافیست بخش موردنظر خود را انتخاب کنید.</p>
    </div>
    <div class="search-wrap">
      <span class="search-icon">🔍</span>
      <input type="text" class="search-input" id="searchInput" placeholder="جستجو در راهنما..." data-i18n-placeholder="searchPlaceholder">
    </div>
    <div class="categories" id="categories"></div>
    <div class="help-grid" id="helpGrid"></div>
  </section>

  <section class="section" id="creator">
    <div class="creator-section">
      <div class="creator-inner">
        <div class="creator-avatar">👨‍💻</div>
        <div>
          <h3 class="creator-name">MAMAL / MAMPY</h3>
          <div class="creator-role" data-i18n="creatorRole">سازنده و توسعه‌دهنده اصلی MAMPY Helper</div>
          <p class="creator-bio" data-i18n="creatorBio">
            محمدحسین، معروف به MAMAL، توسعه‌دهنده و بنیان‌گذار تیم Xr Team. سازنده ربات‌های حرفه‌ای مدیریت گروه در پیام‌رسان بله. MAMPY Helper حاصل تلاش شبانه‌روزی این تیم برای ارائه بهترین تجربه مدیریت گروه است.
          </p>
          <div class="creator-links">
            <a href="https://ble.ir/MAMAL_WIN" target="_blank" class="creator-link"><span>💬</span> ble.ir/MAMAL_WIN</a>
            <a href="https://ble.ir/MAMPY_Group" target="_blank" class="creator-link"><span>🛠️</span> <span data-i18n="creatorSupport">گروه پشتیبانی</span></a>
            <a href="https://ble.ir/MAMPY_Channel" target="_blank" class="creator-link"><span>📢</span> <span data-i18n="creatorChannel">کانال رسمی</span></a>
          </div>
        </div>
      </div>
    </div>
  </section>

</main>

<footer>
  <div class="container">
    <p class="footer-text">
      <span data-i18n="footerMade">ساخته شده با</span>
      <span class="footer-heart">❤️</span>
      <span data-i18n="footerBy">توسط تیم</span>
      <strong style="color:var(--accent-1)">Xr Team</strong>
    </p>
    <p class="footer-text" style="margin-top:6px" data-i18n="footerCopy">© 2025 MAMPY Helper — تمامی حقوق محفوظ است.</p>
    <span class="footer-version">v1.7.0</span>
  </div>
</footer>

<button class="to-top" id="toTop">↑</button>

<div class="modal-overlay" id="modalOverlay">
  <div class="modal" id="modalContent"></div>
</div>

<script>
const I18N = {
  fa: {
    brandSub: "دستیار هوشمند مدیریت گروه",
    heroBadge: "نسخه 1.7.0 — به‌روز و پایدار",
    heroTitle: "MAMPY Helper",
    heroSubtitle: "ربات حرفه‌ای مدیریت گروه در پیام‌رسان بله. با قفل‌های پیشرفته، سیستم اخطار، مجازات هوشمند، بازی‌های سرگرم‌کننده و ده‌ها قابلیت دیگر، تجربه‌ای بی‌نظیر از مدیریت گروه را رقم بزنید.",
    btnGuide: "مشاهده راهنمای کامل",
    btnStart: "شروع استفاده از ربات",
    statLocks: "قفل پیشرفته",
    statCommands: "دستور کاربردی",
    statGames: "بازی سرگرم‌کننده",
    statVip: "قابلیت VIP",
    tagHelp: "راهنمای جامع",
    titleHelp: "همه دستورات در یک نگاه",
    descHelp: "دسته‌بندی شده، جستجوپذیر و کامل. کافیست بخش موردنظر خود را انتخاب کنید.",
    searchPlaceholder: "جستجو در راهنما...",
    creatorRole: "سازنده و توسعه‌دهنده اصلی MAMPY Helper",
    creatorBio: "محمدحسین، معروف به MAMAL، توسعه‌دهنده و بنیان‌گذار تیم Xr Team. سازنده ربات‌های حرفه‌ای مدیریت گروه در پیام‌رسان بله. MAMPY Helper حاصل تلاش شبانه‌روزی این تیم برای ارائه بهترین تجربه مدیریت گروه است.",
    creatorSupport: "گروه پشتیبانی",
    creatorChannel: "کانال رسمی",
    footerMade: "ساخته شده با",
    footerBy: "توسط تیم",
    footerCopy: "© 2025 MAMPY Helper — تمامی حقوق محفوظ است.",
    noResults: "نتیجه‌ای یافت نشد",
    noResultsDesc: "لطفاً عبارت دیگری را جستجو کنید",
    catAll: "همه",
    cmds: "دستورات"
  },
  en: {
    brandSub: "Smart Group Management Assistant",
    heroBadge: "Version 1.7.0 — Up to date & stable",
    heroTitle: "MAMPY Helper",
    heroSubtitle: "Professional group management bot on Bale messenger. With advanced locks, warning system, smart punishments, fun games and dozens of other features, experience unmatched group management.",
    btnGuide: "View Full Guide",
    btnStart: "Start Using Bot",
    statLocks: "Advanced Locks",
    statCommands: "Useful Commands",
    statGames: "Fun Games",
    statVip: "VIP Features",
    tagHelp: "Complete Guide",
    titleHelp: "All Commands at a Glance",
    descHelp: "Categorized, searchable and complete. Just pick the section you want.",
    searchPlaceholder: "Search in guide...",
    creatorRole: "Creator & Lead Developer of MAMPY Helper",
    creatorBio: "MohammadHossein, known as MAMAL, developer and founder of Xr Team. Creator of professional group management bots on Bale messenger. MAMPY Helper is the result of this team's round-the-clock efforts to provide the best group management experience.",
    creatorSupport: "Support Group",
    creatorChannel: "Official Channel",
    footerMade: "Made with",
    footerBy: "by team",
    footerCopy: "© 2025 MAMPY Helper — All rights reserved.",
    noResults: "No results found",
    noResultsDesc: "Please try another search term",
    catAll: "All",
    cmds: "Commands"
  }
};

const CATEGORIES = [
  { id: "locks", icon: "🔐", fa: "قفل‌ها", en: "Locks" },
  { id: "settings", icon: "⚙️", fa: "تنظیمات", en: "Settings" },
  { id: "punish", icon: "🚫", fa: "مجازات‌ها", en: "Punishments" },
  { id: "filters", icon: "📄", fa: "فیلترها", en: "Filters" },
  { id: "forcejoin", icon: "🚷", fa: "عضویت اجباری", en: "Force Join" },
  { id: "utility", icon: "🔰", fa: "کاربردی", en: "Utility" },
  { id: "games", icon: "🎮", fa: "بازی‌ها", en: "Games" },
  { id: "lists", icon: "📋", fa: "لیست‌ها", en: "Lists" },
  { id: "vip", icon: "💎", fa: "قابلیت‌های VIP", en: "VIP Features" }
];

const HELP_DATA = {
  fa: [
    {
      cat: "locks", icon: "🔞", title: "قفل فحش",
      desc: "این قفل به صورت خودکار پیام‌های حاوی کلمات رکیک و نامناسب را تشخیص داده و سریعاً از گروه حذف می‌کند.",
      cmds: [["قفل فحش", "فعال‌سازی"], ["باز کردن فحش", "غیرفعال‌سازی"], ["lock badword", "English"], ["unlock badword", "English"]]
    },
    {
      cat: "locks", icon: "🔗", title: "قفل لینک",
      desc: "با فعال کردن این قفل، ارسال هرگونه لینک (شامل http، https، t.me و ...) برای کاربران عادی ممنوع شده و پیام حذف می‌شود.",
      cmds: [["قفل لینک", "فعال‌سازی"], ["باز کردن لینک", "غیرفعال‌سازی"], ["قفل لینک عمومی", "فعال‌سازی لینک گروه"], ["باز کردن لینک عمومی", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "⚡", title: "قفل اسپم",
      desc: "این سیستم کاربرانی را که پیام‌های تکراری و پشت سر هم ارسال می‌کنند شناسایی کرده و از ارسال پیام مسدود می‌کند.",
      cmds: [["قفل اسپم", "فعال‌سازی"], ["باز کردن اسپم", "غیرفعال‌سازی"], ["lock spam", "English"], ["unlock spam", "English"]]
    },
    {
      cat: "locks", icon: "🎞️", title: "قفل گیف",
      desc: "زمانی که کاربر در گروه گیفی را ارسال می‌کند، ربات سریعاً آن را حذف می‌کند.",
      cmds: [["قفل گیف", "فعال‌سازی"], ["باز کردن گیف", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "👾", title: "قفل استیکر",
      desc: "زمانی که کاربر در گروه استیکری را ارسال می‌کند، ربات سریعاً آن را حذف می‌کند.",
      cmds: [["قفل استیکر", "فعال‌سازی"], ["باز کردن استیکر", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "⛔", title: "قفل کاراکتر",
      desc: "با فعال کردن این قفل و تنظیم کاراکتر مجاز، پیام هر کاربری که تعداد کاراکترهایش بیشتر از حد مجاز باشد حذف می‌شود.",
      cmds: [["قفل کاراکتر [عدد]", "فعال‌سازی"], ["باز کردن کاراکتر", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🔢", title: "قفل کدهنگی",
      desc: "این قفل برای جلوگیری از ارسال کدهای زبان برنامه‌نویسی یا متون خاص طراحی شده است.",
      cmds: [["قفل کدهنگی", "فعال‌سازی"], ["باز کردن کدهنگی", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "✉️", title: "قفل فوروارد",
      desc: "جلوگیری از ارسال پیام‌های فوروارد شده از سایر کانال‌ها یا گروه‌ها. این قفل برای جلوگیری از تبلیغات بسیار کاربردی است.",
      cmds: [["قفل فوروارد", "فعال‌سازی"], ["باز کردن فوروارد", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "↩️", title: "قفل ریپلای",
      desc: "با فعال‌سازی این قفل، کاربران عادی نمی‌توانند روی پیام‌های دیگران پاسخ دهند و فقط ادمین‌ها این امکان را دارند.",
      cmds: [["قفل ریپلای", "فعال‌سازی"], ["باز کردن ریپلای", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "#️⃣", title: "قفل هشتگ",
      desc: "جلوگیری از ارسال متنی که شامل هشتگ (#) می‌باشد. این قفل برای مدیریت چت‌های شلوغ مفید است.",
      cmds: [["قفل هشتگ", "فعال‌سازی"], ["باز کردن هشتگ", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "⌨️", title: "قفل کامند",
      desc: "ممانعت از ارسال دستورات که با علامت / شروع می‌شوند. این قفل دسترسی به ربات‌های دیگر را محدود می‌کند.",
      cmds: [["قفل کامند", "فعال‌سازی"], ["باز کردن کامند", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🔡", title: "قفل انگلیسی",
      desc: "این قفل ارسال هرگونه متنی که حروف انگلیسی یا اعداد انگلیسی داشته باشد را ممنوع می‌کند.",
      cmds: [["قفل انگلیسی", "فعال‌سازی"], ["باز کردن انگلیسی", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🛡️", title: "قفل فارسی",
      desc: "برعکس قفل انگلیسی، این قفل فقط اجازه ارسال متن انگلیسی را می‌دهد و ارسال حروف فارسی را ممنوع می‌کند.",
      cmds: [["قفل فارسی", "فعال‌سازی"], ["باز کردن فارسی", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🔒", title: "قفل گروه",
      desc: "با فعال کردن این قفل، تمامی پیام‌های کاربران عادی به محض ارسال حذف می‌شوند و فقط ادمین‌ها می‌توانند پیام ارسال کنند.",
      cmds: [["قفل گروه", "فعال‌سازی"], ["باز کردن گروه", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🖼️", title: "قفل عکس",
      desc: "جلوگیری از ارسال تصاویر در گروه. برای گروه‌های متنی که تمایل به ارسال عکس ندارند مناسب است.",
      cmds: [["قفل عکس", "فعال‌سازی"], ["باز کردن عکس", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🎥", title: "قفل فیلم",
      desc: "ممانعت از ارسال ویدیو و کلیپ در گروه. این قفل حجم مصرفی اینترنت گروه را کاهش می‌دهد.",
      cmds: [["قفل فیلم", "فعال‌سازی"], ["باز کردن فیلم", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🎵", title: "قفل موسیقی",
      desc: "جلوگیری از ارسال فایل‌های موسیقی در گروه. اگر گروه شما متنی است، این قفل باعث نظم بیشتر می‌شود.",
      cmds: [["قفل موسیقی", "فعال‌سازی"], ["باز کردن موسیقی", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🎤", title: "قفل ویس",
      desc: "منع ارسال پیام‌های صوتی. این قفل کاربران را مجبور به تایپ متن می‌کند.",
      cmds: [["قفل ویس", "فعال‌سازی"], ["باز کردن ویس", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "📍", title: "قفل مکان",
      desc: "جلوگیری از ارسال موقعیت مکانی و نقشه در گروه. برای حفظ حریم خصوصی کاربرد دارد.",
      cmds: [["قفل مکان", "فعال‌سازی"], ["باز کردن مکان", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "📁", title: "قفل فایل",
      desc: "ممانعت از ارسال هرگونه فایل مستند مانند PDF، ZIP و ... در گروه.",
      cmds: [["قفل فایل", "فعال‌سازی"], ["باز کردن فایل", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "👤", title: "قفل مخاطب",
      desc: "جلوگیری از ارسال شماره تماس و اطلاعات مخاطبین در گروه. از انتشار شماره‌های شخصی جلوگیری می‌کند.",
      cmds: [["قفل مخاطب", "فعال‌سازی"], ["باز کردن مخاطب", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🔗", title: "قفل یوزرنیم",
      desc: "با فعال کردن این قفل، زمانی که کاربر در گروه پیامی حاوی یوزرنیم ارسال کند، ربات پیام را حذف می‌کند.",
      cmds: [["قفل یوزرنیم", "فعال‌سازی"], ["باز کردن یوزرنیم", "غیرفعال‌سازی"]]
    },
    {
      cat: "locks", icon: "🫡", title: "قفل حکومت نظامی",
      desc: "با فعال کردن این قفل، تمامی قفل‌های مهم فعال می‌شوند. مناسب برای شرایط بحرانی.",
      cmds: [["قفل حکومت نظامی", "فعال‌سازی همه قفل‌ها"], ["باز کردن حکومت نظامی", "غیرفعال‌سازی همه"]]
    },
    {
      cat: "settings", icon: "💾", title: "بکاپ تنظیمات",
      desc: "با این دستور می‌توانید یک فایل متنی حاوی تمام تنظیمات، قفل‌ها، مجازات‌ها، لیست‌ها و آمار گروه دریافت کنید.",
      cmds: [["بکاپ", "دریافت فایل بکاپ"], ["backup", "English"]]
    },
    {
      cat: "settings", icon: "📝", title: "تنظیم گروه گزارش",
      desc: "با تنظیم گروه گزارش، فعالیت‌های ادمین‌های گروه اصلی مانند ریم، بن، سکوت و ... به صورت خلاصه به گروه موردنظر ارسال می‌شود.",
      cmds: [["ارسال گزارش [شناسه]", "تنظیم گروه گزارش"], ["حذف گروه گزارش", "حذف تنظیم"]]
    },
    {
      cat: "settings", icon: "🔐", title: "قفل خودکار گروه",
      desc: "با این قفل می‌توانید گروه را در یک زمان مشخص قفل و در زمان مشخص باز کنید. در زمان قفل، کاربران عادی اجازه ارسال پیام ندارند.",
      cmds: [["قفل خودکار گروه 23:30-7:00", "تنظیم زمان"], ["بازکردن قفل خودکار گروه", "غیرفعال‌سازی"]]
    },
    {
      cat: "settings", icon: "⚠️", title: "تنظیم حداکثر اخطار",
      desc: "با تنظیم کردن حداکثر اخطار مجاز، زمانی که کاربر به سقف مجازات می‌رسد، مجازات تنظیم شده روی کاربر اعمال می‌شود.",
      cmds: [["تنظیم [عدد] اخطار [مجازات]", "مثال: تنظیم 5 اخطار بن"]]
    },
    {
      cat: "settings", icon: "🚫", title: "تنظیم مجازات کاربران",
      desc: "با تنظیم کردن مجازات در گروه، می‌توانید تعیین کنید که اگر کاربری پیام ممنوعه فرستاد، چه مجازاتی داشته باشد.",
      cmds: [["مجازات [نوع] [مجازات]", "مثال: مجازات فحش اخطار"]]
    },
    {
      cat: "settings", icon: "😊", title: "تنظیم خوش‌آمد",
      desc: "زمانی که متن خوش‌آمد را تنظیم می‌کنید، هر کاربری که به گروه عضو شود، متن خوش‌آمد ارسال می‌شود.",
      cmds: [["تنظیم خوش آمد [متن]", "متغیرها: {name} {time} {title}"]]
    },
    {
      cat: "settings", icon: "🔰", title: "تنظیم قوانین",
      desc: "زمانی که قوانین را تنظیم می‌کنید، کاربران می‌توانند قوانین را با ارسال دستور مشاهده کنند.",
      cmds: [["تنظیم قوانین (ریپلای)", "ثبت قوانین"], ["حذف قوانین", "حذف قوانین"]]
    },
    {
      cat: "settings", icon: "👤", title: "ثبت اصل",
      desc: "ثبت کردن اصل کاربر موردنظر در اطلاعات گروه. این دستورات با ریپلای زدن روی کاربر موردنظر انجام می‌شود.",
      cmds: [["ثبت اصل (ریپلای)", "ثبت اصل"], ["حذف اصل (ریپلای)", "حذف اصل"]]
    },
    {
      cat: "settings", icon: "🚫", title: "ثبت فحش",
      desc: "با ثبت کردن فحش موردنظر، ارسال آن فحش در گروه ممنوع می‌شود.",
      cmds: [["ثبت فحش [کلمه]", "افزودن به لیست"], ["حذف فحش [کلمه]", "حذف از لیست"]]
    },
    {
      cat: "settings", icon: "💬", title: "ثبت پیام تکراری",
      desc: "با ثبت پیام تکراری، پیام موردنظر با توجه به فاصله زمانی در گروه ارسال می‌شود.",
      cmds: [["پیام تکراری [زمان] (ریپلای)", "زمان به دقیقه"], ["حذف پیام تکراری", "حذف"]]
    },
    {
      cat: "punish", icon: "⭕", title: "بن",
      desc: "زمانی که یک کاربر بن می‌شود، امکان ورود دوباره به گروه را ندارد.",
      cmds: [["بن (ریپلای)", "بن کردن"], ["بن [آیدی]", "بن با آیدی"], ["حذف بن [آیدی]", "رفع بن"]]
    },
    {
      cat: "punish", icon: "⚠️", title: "ریم",
      desc: "زمانی که یک کاربر ریم می‌شود، امکان بازگشت دوباره کاربر در گروه وجود دارد.",
      cmds: [["ریم (ریپلای)", "ریم کردن"], ["ریم [آیدی]", "ریم با آیدی"], ["kick", "English"]]
    },
    {
      cat: "punish", icon: "⭕", title: "بن پلاس",
      desc: "زمانی که یک کاربر بن پلاس می‌شود، پیام موفقیت بن ارسال نمی‌شود و پیام ادمین پاک می‌شود.",
      cmds: [["بن پلاس (ریپلای)", "بن بدون پیام"], ["banplus", "English"]]
    },
    {
      cat: "punish", icon: "⚠️", title: "ریم پلاس",
      desc: "زمانی که یک کاربر ریم پلاس می‌شود، پیام موفقیت ریم ارسال نمی‌شود و پیام ادمین پاک می‌شود.",
      cmds: [["ریم پلاس (ریپلای)", "ریم بدون پیام"], ["kickplus", "English"]]
    },
    {
      cat: "punish", icon: "⚠️", title: "اخطار",
      desc: "ادمین می‌تواند به صورت دستی به کاربر اخطار دهد. با رسیدن به سقف، مجازات اعمال می‌شود.",
      cmds: [["اخطار (ریپلای)", "دادن اخطار"], ["حذف اخطار (ریپلای)", "کم کردن اخطار"], ["حذف اخطارها (ریپلای)", "حذف همه"]]
    },
    {
      cat: "punish", icon: "🔇", title: "سکوت",
      desc: "زمانی که یک کاربر سکوت می‌شود، امکان ارسال پیام در گروه را ندارد.",
      cmds: [["سکوت (ریپلای)", "سکوت دائم"], ["حذف سکوت (ریپلای)", "رفع سکوت"], ["سکوت کاربر [آیدی]", "با آیدی"]]
    },
    {
      cat: "punish", icon: "🔇", title: "سکوت زمان‌دار",
      desc: "زمانی که ادمین یک نفر را برای زمان مشخصی سکوت می‌کند، فرد موردنظر تا پایان زمان تعیین شده سکوت می‌ماند.",
      cmds: [["سکوت [دقیقه] (ریپلای)", "مثال: سکوت 10"], ["حذف سکوت (ریپلای)", "رفع سکوت"]]
    },
    {
      cat: "punish", icon: "⭕", title: "تغییر مجوز کاربران",
      desc: "با این دستور می‌توانید مجوزهای کاربر را از طریق ربات تغییر دهید.",
      cmds: [["دسترسی (ریپلای)", "مدیریت دسترسی"], ["دسترسی [آیدی]", "با آیدی"]]
    },
    {
      cat: "punish", icon: "⚠️", title: "گزارش به ادمین",
      desc: "با این دستور می‌توانید پیام یک کاربر را به ادمین‌های گروه گزارش دهید.",
      cmds: [["گزارش (ریپلای)", "ارسال گزارش"]]
    },
    {
      cat: "filters", icon: "💬", title: "قفل پاسخ خودکار",
      desc: "با این قابلیت می‌توانید کنترل کنید که ربات به کلمات فیلترشده پاسخ خودکار بدهد یا نه.",
      cmds: [["قفل پاسخ خودکار", "فعال‌سازی"], ["باز کردن پاسخ خودکار", "غیرفعال‌سازی"]]
    },
    {
      cat: "filters", icon: "📋", title: "افزودن فیلتر",
      desc: "با افزودن فیلتر بر یک کلمه یا جمله، می‌توانید برای آن جمله یک جواب مشخص قرار دهید.",
      cmds: [["ثبت فیلتر [جواب] (ریپلای)", "افزودن فیلتر"]]
    },
    {
      cat: "filters", icon: "📋", title: "حذف فیلتر",
      desc: "با حذف کردن یک فیلتر، می‌توانید جواب آن فیلتر را از اطلاعات گروه حذف کنید.",
      cmds: [["حذف فیلتر [کلمه]", "حذف فیلتر"]]
    },
    {
      cat: "filters", icon: "📋", title: "مشاهده لیست فیلتر",
      desc: "با این دستور می‌توانید تمام فیلترهای ثبت شده را مشاهده کنید.",
      cmds: [["لیست فیلترها", "مشاهده لیست"]]
    },
    {
      cat: "forcejoin", icon: "🚷", title: "افزودن عضویت اجباری",
      desc: "با این دستور می‌توانید برای کاربران عضویت اجباری بگذارید.",
      cmds: [["عضویت اجباری [آیدی]", "افزودن"], ["forcejoin [id]", "English"]]
    },
    {
      cat: "forcejoin", icon: "🚷", title: "حذف عضویت اجباری",
      desc: "با این دستور می‌توانید گفتگوی موردنظر را از لیست عضویت اجباری حذف کنید.",
      cmds: [["حذف عضویت اجباری [آیدی]", "حذف"]]
    },
    {
      cat: "forcejoin", icon: "📋", title: "مشاهده لیست عضویت اجباری",
      desc: "با این دستور می‌توانید لیست کانال‌هایی که جوین در آنها اجباری است را مشاهده کنید.",
      cmds: [["لیست عضویت اجباری", "مشاهده لیست"]]
    },
    {
      cat: "utility", icon: "💸", title: "نرخ ارز",
      desc: "با این دستور می‌توانید از آخرین قیمت ارزهای موجود مطلع شوید.",
      cmds: [["نرخ ارز", "مشاهده قیمت‌ها"], ["currency", "English"]]
    },
    {
      cat: "utility", icon: "🌤️", title: "آب و هوا",
      desc: "با این دستور می‌توانید وضعیت آب و هوای هر شهر را مشاهده کنید.",
      cmds: [["هوا [شهر]", "مشاهده آب و هوا"], ["weather [city]", "English"]]
    },
    {
      cat: "utility", icon: "📰", title: "اخبار",
      desc: "با این دستور می‌توانید آخرین اخبار روز را دریافت کنید.",
      cmds: [["اخبار", "دریافت اخبار"], ["news", "English"]]
    },
    {
      cat: "utility", icon: "🌐", title: "ترجمه",
      desc: "با این دستور می‌توانید متن‌های فارسی را به انگلیسی و بالعکس ترجمه کنید.",
      cmds: [["ترجمه [متن]", "ترجمه متن"], ["translate [text]", "English"]]
    },
    {
      cat: "utility", icon: "🎬", title: "ساخت گیف",
      desc: "با این دستور می‌توانید روی عکس یا گیف ریپلای کنید و آن را به گیف تبدیل کنید.",
      cmds: [["ساخت گیف (ریپلای)", "تبدیل به گیف"], ["ساخت گیف [متن]", "با متن دلخواه"]]
    },
    {
      cat: "utility", icon: "🎲", title: "تاس",
      desc: "با این دستور ربات یک تاس تصادفی برای شما پرتاب می‌کند.",
      cmds: [["تاس", "پرتاب تاس"], ["dice", "English"]]
    },
    {
      cat: "utility", icon: "🔍", title: "استخراج متن مخفی",
      desc: "با این دستور می‌توانید متن‌های مخفی داخل پرانتز را از پیام‌های ریپلای شده استخراج کنید.",
      cmds: [["حقیقت (ریپلای)", "استخراج"], ["واقعیت (ریپلای)", "استخراج"]]
    },
    {
      cat: "utility", icon: "🔊", title: "سیستم اکو",
      desc: "با این دستور، ربات پیام شما را پاک کرده و متن را همراه با منشن مخفی فرستنده ارسال می‌کند.",
      cmds: [["اکو [متن]", "ارسال اکو"], ["echo [text]", "English"]]
    },
    {
      cat: "utility", icon: "🔢", title: "ماشین حساب",
      desc: "با این قابلیت می‌توانید عملیات‌های مختلف ریاضی را انجام دهید.",
      cmds: [["حساب [عملیات]", "مثال: حساب 2 + 9 × 5"], ["calc [op]", "English"]]
    },
    {
      cat: "utility", icon: "📜", title: "غزل حافظ",
      desc: "با این دستور می‌توانید یک غزل تصادفی از دیوان حضرت حافظ دریافت کنید.",
      cmds: [["حافظ", "دریافت غزل"], ["hafez", "English"]]
    },
    {
      cat: "utility", icon: "📖", title: "ویکی‌پدیا",
      desc: "با این دستور می‌توانید هر موضوعی را در ویکی‌پدیا جستجو کنید.",
      cmds: [["ویکی [عبارت]", "جستجو"], ["wikipedia [query]", "English"]]
    },
    {
      cat: "utility", icon: "🧹", title: "پاک کردن پیام",
      desc: "با این دستور می‌توانید تعداد مشخصی از پیام‌های گروه را پاک کنید.",
      cmds: [["پاک کردن [عدد] پیام", "حداکثر 100 پیام"], ["purge [num]", "English"]]
    },
    {
      cat: "utility", icon: "😶‍🌫️", title: "ارسال پیام ناشناس",
      desc: "با این دستور می‌توانید برای کاربر موردنظر خود در گروه پیام ناشناس ارسال کنید.",
      cmds: [["پیام ناشناس (ریپلای)", "ارسال ناشناس"], ["anonymous (reply)", "English"]]
    },
    {
      cat: "utility", icon: "🔰", title: "ارسال درخواست کمک",
      desc: "با ارسال این دستور، تیم پشتیبانی برای کمک به شما به گروه مراجعه می‌کنند.",
      cmds: [["کمک", "درخواست پشتیبانی"], ["support", "English"]]
    },
    {
      cat: "utility", icon: "📊", title: "آمار گروه",
      desc: "با این دستور می‌توانید آمار کاربران گروه را مشاهده کنید.",
      cmds: [["آمار", "مشاهده آمار"], ["گزارش روزانه", "گزارش روز"], ["stats", "English"]]
    },
    {
      cat: "utility", icon: "📿", title: "صلوات",
      desc: "با این دستور ربات در گروه صلوات ارسال می‌کند.",
      cmds: [["صلوات", "ارسال صلوات"], ["salavat", "English"]]
    },
    {
      cat: "utility", icon: "📜", title: "حدیث",
      desc: "با این دستور، ربات به صورت تصادفی یک حدیث ارسال می‌کند.",
      cmds: [["حدیث", "ارسال حدیث"], ["hadith", "English"]]
    },
    {
      cat: "utility", icon: "🎭", title: "جوک",
      desc: "با این دستور، ربات به صورت تصادفی یک جوک ارسال می‌کند.",
      cmds: [["جوک", "ارسال جوک"], ["joke", "English"]]
    },
    {
      cat: "utility", icon: "🤖", title: "هوش مصنوعی",
      desc: "با این دستور می‌توانید هر سوالی را از هوش مصنوعی بات بپرسید.",
      cmds: [["هوش [سوال]", "پرسش از AI"], ["ai [question]", "English"]]
    },
    {
      cat: "utility", icon: "📌", title: "لینک",
      desc: "با این دستور می‌توانید لینک خصوصی گروه را دریافت کنید.",
      cmds: [["لینک", "دریافت لینک"], ["link", "English"]]
    },
    {
      cat: "utility", icon: "🏓", title: "پینگ",
      desc: "با این دستور می‌توانید سرعت پاسخگویی ربات را مشاهده کنید.",
      cmds: [["پینگ", "بررسی سرعت"], ["ping", "English"]]
    },
    {
      cat: "utility", icon: "👾", title: "تغییر نام گروه",
      desc: "با این دستور می‌توانید نام گروه را تغییر دهید.",
      cmds: [["تغییر نام [نام جدید]", "تغییر نام"], ["set title [name]", "English"]]
    },
    {
      cat: "utility", icon: "🔹", title: "تغییر توضیحات",
      desc: "با این دستور می‌توانید توضیحات گروه را تغییر دهید.",
      cmds: [["تغییر توضیحات [متن]", "تغییر توضیحات"]]
    },
    {
      cat: "utility", icon: "🙎‍♂️", title: "دستورات ادمین",
      desc: "دستورات مدیریت ادمین‌های گروه توسط مالک.",
      cmds: [["ترفیع (ریپلای)", "اضافه کردن ادمین"], ["عزل (ریپلای)", "حذف ادمین"], ["لیست ادمین", "مشاهده لیست"]]
    },
    {
      cat: "utility", icon: "📌", title: "پین کردن",
      desc: "با این دستورات می‌توانید پیام‌های سنجاق شده را مدیریت کنید.",
      cmds: [["پین (ریپلای)", "سنجاق پیام"], ["حذف پین (ریپلای)", "برداشتن سنجاق"], ["حذف پین‌ها", "حذف همه"]]
    },
    {
      cat: "utility", icon: "⚙️", title: "تنظیمات (پنل)",
      desc: "با این دستور می‌توانید پنل مختصر تنظیمات و قفل‌های گروه را مشاهده کنید.",
      cmds: [["تنظیمات", "نمایش پنل"], ["پنل", "نمایش پنل"]]
    },
    {
      cat: "utility", icon: "👤", title: "اطلاعات کاربر",
      desc: "با این دستور می‌توانید اطلاعات شخص موردنظر را مشاهده کنید.",
      cmds: [["اطلاعات (ریپلای)", "اطلاعات کاربر"], ["پروفایل (ریپلای)", "پروفایل"]]
    },
    {
      cat: "utility", icon: "👤", title: "اطلاعات من",
      desc: "با این دستور می‌توانید اطلاعات پروفایل خود را مشاهده کنید.",
      cmds: [["پروفایل", "پروفایل من"], ["اطلاعات", "اطلاعات من"], ["من", "اطلاعات من"]]
    },
    {
      cat: "utility", icon: "⏰", title: "تاریخ",
      desc: "با ارسال این دستور، از زمان و تاریخ مطلع شوید.",
      cmds: [["تاریخ", "مشاهده تاریخ"], ["تایم", "مشاهده زمان"], ["زمان", "مشاهده زمان"]]
    },
    {
      cat: "utility", icon: "🍂", title: "خروج ربات از گروه",
      desc: "با این دستورات، ربات گروه را ترک می‌کند (فقط مالک).",
      cmds: [["مامپای خداحافظ", "خروج ربات"], ["مامپای برو", "خروج ربات"], ["bye", "English"]]
    },
    {
      cat: "utility", icon: "👤", title: "ارسال پیام ترک گروه",
      desc: "زمانی که کاربری گروه را ترک می‌کند، ربات اعلان ترک گروه را ارسال می‌کند.",
      cmds: [["ترک گروه روشن", "فعال‌سازی"], ["ترک گروه خاموش", "غیرفعال‌سازی"]]
    },
    {
      cat: "utility", icon: "🌱", title: "ارسال پیام خوش‌آمد",
      desc: "زمانی که خوش‌آمدگویی فعال است، پیام خوش‌آمد به کاربر جدید ارسال می‌شود.",
      cmds: [["خوش آمد روشن", "فعال‌سازی"], ["خوش آمد خاموش", "غیرفعال‌سازی"]]
    },
    {
      cat: "utility", icon: "🎮", title: "سیستم امتیازگیری",
      desc: "با فعالیت در گروه امتیاز جمع کنید، سطح خود را بالا ببرید و با بقیه رقابت کنید.",
      cmds: [["امتیاز", "دریافت امتیاز"], ["امتیازام", "مشاهده امتیاز"], ["قمار امتیاز [عدد]", "شرکت در قمار"], ["لیدربرد امتیاز", "برترین‌ها"]]
    },
    {
      cat: "games", icon: "👾", title: "بازی دوز",
      desc: "با این دستور ادمین‌ها می‌توانند بازی دوز را استارت کنند.",
      cmds: [["دوز", "شروع بازی"], ["tic", "English"], ["بستن بازی‌ها", "بستن بازی‌ها"]]
    },
    {
      cat: "games", icon: "👾", title: "بازی گل یا پوچ",
      desc: "با این دستور، ادمین‌ها می‌توانند بازی گل یا پوچ را استارت کنند.",
      cmds: [["گل یا پوچ", "شروع بازی"], ["guess", "English"]]
    },
    {
      cat: "games", icon: "💣", title: "بازی مین‌روب",
      desc: "یک بازی فکری، کلاسیک و تک‌نفره پرطرفدار. تمام خانه‌های خالی زمین 5×5 را بدون برخورد با مین‌ها پیدا کنید.",
      cmds: [["بازی مینروب", "شروع بازی"], ["مین‌روب", "شروع بازی"], ["mines", "English"]]
    },
    {
      cat: "lists", icon: "📋", title: "مشاهده لیست‌ها",
      desc: "با دستورات زیر می‌توانید انواع لیست‌ها را مشاهده کنید.",
      cmds: [["لیست سکوت", "کاربران سکوت"], ["لیست اخطار", "کاربران اخطار"], ["لیست ادمین", "ادمین‌ها"], ["لیست فحش ها", "فحش‌ها"], ["لیست معاف", "معاف‌ها"]]
    },
    {
      cat: "lists", icon: "🧹", title: "پاکسازی لیست‌ها",
      desc: "با این دستورات می‌توانید لیست‌های موردنظر را پاکسازی کنید.",
      cmds: [["پاکسازی لیست فیلتر", "پاک کردن فیلترها"], ["پاکسازی لیست فحش", "پاک کردن فحش‌ها"], ["پاکسازی لیست معاف", "پاک کردن معاف‌ها"]]
    },
    {
      cat: "vip", icon: "💎", title: "اشتراک VIP",
      desc: "با تهیه اشتراک VIP می‌توانید از قابلیت‌های ویژه ربات مانند قفل‌های بیو، قفل نام ناپسند، قفل ویرایش و محدودیت ارسال پیام استفاده کنید.",
      cmds: [["خرید اشتراک", "مشاهده پلن‌ها"], ["اشتراک", "مشاهده اشتراک فعلی"], ["buy subscription", "English"]]
    },
    {
      cat: "vip", icon: "🔗", title: "قفل لینک در بیو",
      desc: "اگر در بیوگرافی کاربر، لینک وجود داشته باشد، ربات پیام کاربر را حذف می‌کند. (ویژه VIP)",
      cmds: [["قفل لینک در بیو", "فعال‌سازی"], ["باز کردن لینک در بیو", "غیرفعال‌سازی"]]
    },
    {
      cat: "vip", icon: "🔗", title: "قفل آیدی در بیو",
      desc: "اگر در بیوگرافی کاربر، شناسه کاربری وجود داشته باشد، ربات پیام کاربر را حذف می‌کند. (ویژه VIP)",
      cmds: [["قفل آیدی در بیو", "فعال‌سازی"], ["باز کردن آیدی در بیو", "غیرفعال‌سازی"]]
    },
    {
      cat: "vip", icon: "🔗", title: "قفل یوزرنیم در بیو",
      desc: "اگر در بیوگرافی کاربر، یوزرنیم وجود داشته باشد، ربات پیام کاربر را حذف می‌کند. (ویژه VIP)",
      cmds: [["قفل یوزرنیم در بیو", "فعال‌سازی"], ["باز کردن یوزرنیم در بیو", "غیرفعال‌سازی"]]
    },
    {
      cat: "vip", icon: "🔞", title: "قفل فحش در بیو",
      desc: "اگر در بیوگرافی کاربر، فحش وجود داشته باشد، ربات پیام کاربر را حذف می‌کند. (ویژه VIP)",
      cmds: [["قفل فحش در بیو", "فعال‌سازی"], ["باز کردن فحش در بیو", "غیرفعال‌سازی"]]
    },
    {
      cat: "vip", icon: "📛", title: "قفل نام ناپسند",
      desc: "پیام کاربرانی که نام آنها حاوی کلمات ناپسند است را پاک می‌کند. (ویژه VIP)",
      cmds: [["قفل نام", "فعال‌سازی"], ["باز کردن نام", "غیرفعال‌سازی"]]
    },
    {
      cat: "vip", icon: "✍️", title: "قفل ویرایش پیام",
      desc: "از ویرایش پیام از سوی کاربران جلوگیری می‌کند و پیام‌های ویرایش شده را پاک می‌کند. (ویژه VIP)",
      cmds: [["قفل ویرایش", "فعال‌سازی"], ["باز کردن ویرایش", "غیرفعال‌سازی"]]
    },
    {
      cat: "vip", icon: "📊", title: "قفل محدودیت ارسال",
      desc: "برای هر نوع پیام محدودیت روزانه تعیین کنید. اگر کاربر عبور کند، پیام‌هایش حذف می‌شود. (ویژه VIP)",
      cmds: [["قفل محدودیت [نوع]", "فعال‌سازی"], ["تنظیم محدودیت ارسال [نوع] [عدد]", "تنظیم تعداد"], ["باز کردن محدودیت ها", "غیرفعال‌سازی همه"]]
    }
  ],
  en: []
};

HELP_DATA.en = [
  {
    cat: "locks", icon: "🔞", title: "Badword Lock",
    desc: "This lock automatically detects messages containing badwords and deletes them to maintain group order.",
    cmds: [["lock badword", "Enable"], ["unlock badword", "Disable"], ["قفل فحش", "Persian"], ["باز کردن فحش", "Persian"]]
  },
  {
    cat: "locks", icon: "🔗", title: "Link Lock",
    desc: "When this lock is active, sending any link (http, https, t.me, etc.) is prohibited for regular users and the message will be deleted.",
    cmds: [["lock link", "Enable"], ["unlock link", "Disable"], ["lock publiclink", "Group link only"], ["unlock publiclink", "Disable"]]
  },
  {
    cat: "locks", icon: "⚡", title: "Spam Lock",
    desc: "This system detects users who send repeated messages and prevents them from sending messages.",
    cmds: [["lock spam", "Enable"], ["unlock spam", "Disable"]]
  },
  {
    cat: "locks", icon: "🎞️", title: "GIF Lock",
    desc: "When a user sends a GIF in the group, the bot immediately deletes it!",
    cmds: [["lock gif", "Enable"], ["unlock gif", "Disable"]]
  },
  {
    cat: "locks", icon: "👾", title: "Sticker Lock",
    desc: "When a user sends a sticker in the group, the bot immediately deletes it!",
    cmds: [["lock sticker", "Enable"], ["unlock sticker", "Disable"]]
  },
  {
    cat: "locks", icon: "⛔", title: "Character Lock",
    desc: "When active and you set a character limit, any message with more characters than the limit will be deleted.",
    cmds: [["lock char [number]", "Enable"], ["unlock char", "Disable"]]
  },
  {
    cat: "locks", icon: "🔢", title: "Code Lock",
    desc: "This lock prevents sending programming code or special texts.",
    cmds: [["lock code", "Enable"], ["unlock code", "Disable"]]
  },
  {
    cat: "locks", icon: "✉️", title: "Forward Lock",
    desc: "Prevents forwarding messages from other channels or groups. Very useful for preventing advertising.",
    cmds: [["lock forward", "Enable"], ["unlock forward", "Disable"]]
  },
  {
    cat: "locks", icon: "↩️", title: "Reply Lock",
    desc: "When active, regular users cannot reply to others' messages, only admins can.",
    cmds: [["lock reply", "Enable"], ["unlock reply", "Disable"]]
  },
  {
    cat: "locks", icon: "#️⃣", title: "Hashtag Lock",
    desc: "Prevents sending text containing hashtags (#). Useful for managing busy chats.",
    cmds: [["lock hashtag", "Enable"], ["unlock hashtag", "Disable"]]
  },
  {
    cat: "locks", icon: "⌨️", title: "Command Lock",
    desc: "Prevents sending commands that start with /. This lock restricts access to other bots.",
    cmds: [["lock command", "Enable"], ["unlock command", "Disable"]]
  },
  {
    cat: "locks", icon: "🔡", title: "English Lock",
    desc: "This lock prohibits sending any text containing English letters or numbers.",
    cmds: [["lock english", "Enable"], ["unlock english", "Disable"]]
  },
  {
    cat: "locks", icon: "🛡️", title: "Persian Lock",
    desc: "Opposite of English lock, this only allows sending English text and prohibits Persian letters.",
    cmds: [["lock persian", "Enable"], ["unlock persian", "Disable"]]
  },
  {
    cat: "locks", icon: "🔒", title: "Group Lock",
    desc: "When active, all messages from regular users are deleted upon sending, and only admins can send messages.",
    cmds: [["lock group", "Enable"], ["unlock group", "Disable"]]
  },
  {
    cat: "locks", icon: "🖼️", title: "Photo Lock",
    desc: "Prevents sending images in the group. Suitable for text-based groups.",
    cmds: [["lock photo", "Enable"], ["unlock photo", "Disable"]]
  },
  {
    cat: "locks", icon: "🎥", title: "Video Lock",
    desc: "Prevents sending videos and clips in the group. Reduces internet usage.",
    cmds: [["lock video", "Enable"], ["unlock video", "Disable"]]
  },
  {
    cat: "locks", icon: "🎵", title: "Music Lock",
    desc: "Prevents sending music files in the group. Brings more order to text-based groups.",
    cmds: [["lock music", "Enable"], ["unlock music", "Disable"]]
  },
  {
    cat: "locks", icon: "🎤", title: "Voice Lock",
    desc: "Prevents sending voice messages. Forces users to type text.",
    cmds: [["lock voice", "Enable"], ["unlock voice", "Disable"]]
  },
  {
    cat: "locks", icon: "📍", title: "Location Lock",
    desc: "Prevents sending location and maps in the group. Useful for privacy protection.",
    cmds: [["lock location", "Enable"], ["unlock location", "Disable"]]
  },
  {
    cat: "locks", icon: "📁", title: "File Lock",
    desc: "Prevents sending document files (PDF, ZIP, etc.) in the group.",
    cmds: [["lock file", "Enable"], ["unlock file", "Disable"]]
  },
  {
    cat: "locks", icon: "👤", title: "Contact Lock",
    desc: "Prevents sending contact information in the group. Prevents sharing personal numbers.",
    cmds: [["lock contact", "Enable"], ["unlock contact", "Disable"]]
  },
  {
    cat: "locks", icon: "🔗", title: "Username Lock",
    desc: "When active, if a user's message contains a username, the bot deletes the message.",
    cmds: [["lock username", "Enable"], ["unlock username", "Disable"]]
  },
  {
    cat: "locks", icon: "🫡", title: "Martial Law Lock",
    desc: "When activated, all important locks are activated simultaneously!",
    cmds: [["lock martial", "Enable all"], ["unlock martial", "Disable all"]]
  },
  {
    cat: "settings", icon: "💾", title: "Backup Settings",
    desc: "This command gives you a text file containing all settings, locks, punishments, lists, and group statistics.",
    cmds: [["backup", "Download backup"], ["بکاپ", "Persian"]]
  },
  {
    cat: "settings", icon: "📝", title: "Set Log Group",
    desc: "By setting a log group, admin activities from your main group will be sent as a summary to the target group.",
    cmds: [["setlog [id]", "Set log group"], ["remove log", "Remove setting"]]
  },
  {
    cat: "settings", icon: "🔐", title: "Auto Group Lock",
    desc: "With this lock, you can lock the group at a specific time and unlock at a specific time.",
    cmds: [["lock auto 23:30-7:00", "Set time"], ["unlock autolock", "Disable"]]
  },
  {
    cat: "settings", icon: "⚠️", title: "Set Max Warnings",
    desc: "By setting the maximum warnings, when a user reaches the limit, the set punishment will be applied.",
    cmds: [["set [num] warn [punish]", "Example: set 5 warn ban"]]
  },
  {
    cat: "settings", icon: "🚫", title: "Set User Punishments",
    desc: "By setting punishments, you can determine what punishment a user gets if they send a restricted message.",
    cmds: [["punish [type] [punish]", "Example: punish badword warning"]]
  },
  {
    cat: "settings", icon: "😊", title: "Set Welcome Message",
    desc: "When you set a welcome message, any new member who joins will receive it.",
    cmds: [["set welcome [text]", "Variables: {name} {time} {title}"]]
  },
  {
    cat: "settings", icon: "🔰", title: "Set Rules",
    desc: "When you set rules, users can view them by sending a command.",
    cmds: [["set rules (reply)", "Set rules"], ["remove rules", "Remove rules"]]
  },
  {
    cat: "settings", icon: "👤", title: "Register Bio",
    desc: "Register a bio for a user in the group info. Works by replying to the target user.",
    cmds: [["add bio (reply)", "Add bio"], ["remove bio (reply)", "Remove bio"]]
  },
  {
    cat: "settings", icon: "🚫", title: "Register Badword",
    desc: "By registering a badword, sending that word in the group will be prohibited.",
    cmds: [["add badword [word]", "Add to list"], ["remove badword [word]", "Remove from list"]]
  },
  {
    cat: "settings", icon: "💬", title: "Register Repeating Message",
    desc: "By registering a repeating message, the message will be sent in the group according to the time interval.",
    cmds: [["repeat [min] (reply)", "Time in minutes"], ["remove repeat", "Remove"]]
  },
  {
    cat: "punish", icon: "⭕", title: "Ban",
    desc: "When a user is banned, they cannot re-enter the group!",
    cmds: [["ban (reply)", "Ban user"], ["ban [id]", "Ban by ID"], ["remove ban [id]", "Unban"]]
  },
  {
    cat: "punish", icon: "⚠️", title: "Kick",
    desc: "When a user is kicked, they can re-join the group!",
    cmds: [["kick (reply)", "Kick user"], ["kick [id]", "Kick by ID"], ["ریم", "Persian"]]
  },
  {
    cat: "punish", icon: "⭕", title: "Ban Plus",
    desc: "When a user is ban plus, no success message is sent and the admin's message is deleted!",
    cmds: [["banplus (reply)", "Ban without message"]]
  },
  {
    cat: "punish", icon: "⚠️", title: "Kick Plus",
    desc: "When a user is kick plus, no success message is sent and the admin's message is deleted!",
    cmds: [["kickplus (reply)", "Kick without message"]]
  },
  {
    cat: "punish", icon: "⚠️", title: "Warning",
    desc: "Admins can manually warn users. When limit is reached, punishment is applied.",
    cmds: [["warn (reply)", "Give warning"], ["remove warn (reply)", "Remove one"], ["remove warns (reply)", "Remove all"]]
  },
  {
    cat: "punish", icon: "🔇", title: "Mute",
    desc: "When a user is muted, they cannot send messages in the group!",
    cmds: [["mute (reply)", "Permanent mute"], ["remove mute (reply)", "Unmute"], ["muteuser [id]", "By ID"]]
  },
  {
    cat: "punish", icon: "🔇", title: "Timed Mute",
    desc: "When an admin mutes a user for a specific time, the user remains muted until the time ends!",
    cmds: [["mutetime [min] (reply)", "Example: mutetime 10"], ["remove mute (reply)", "Unmute"]]
  },
  {
    cat: "punish", icon: "⭕", title: "Change User Permissions",
    desc: "This command lets you change user permissions through the bot!",
    cmds: [["permission (reply)", "Manage permissions"], ["permission [id]", "By ID"]]
  },
  {
    cat: "punish", icon: "⚠️", title: "Report to Admin",
    desc: "This command reports a user's message to the group admins.",
    cmds: [["report (reply)", "Send report"]]
  },
  {
    cat: "filters", icon: "💬", title: "Auto Reply Lock",
    desc: "With this feature, you can control whether the bot automatically replies to filtered words or not.",
    cmds: [["lock autofilter", "Enable"], ["unlock autofilter", "Disable"]]
  },
  {
    cat: "filters", icon: "📋", title: "Add Filter",
    desc: "By adding a filter to a word or phrase, you can set a specific reply for it!",
    cmds: [["add filter [reply] (reply)", "Add filter"]]
  },
  {
    cat: "filters", icon: "📋", title: "Remove Filter",
    desc: "By removing a filter, you can delete its reply from the group data!",
    cmds: [["remove filter [word]", "Remove filter"]]
  },
  {
    cat: "filters", icon: "📋", title: "View Filter List",
    desc: "This command shows all registered filters!",
    cmds: [["list filters", "View list"]]
  },
  {
    cat: "forcejoin", icon: "🚷", title: "Add Mandatory Membership",
    desc: "This command lets you set mandatory membership for users!",
    cmds: [["forcejoin [id]", "Add"], ["عضویت اجباری [آیدی]", "Persian"]]
  },
  {
    cat: "forcejoin", icon: "🚷", title: "Remove Mandatory Membership",
    desc: "This command lets you remove a chat from the mandatory membership list!",
    cmds: [["remove forcejoin [id]", "Remove"]]
  },
  {
    cat: "forcejoin", icon: "📋", title: "View Mandatory Membership List",
    desc: "This command shows the list of channels where membership is mandatory!",
    cmds: [["list forcejoin", "View list"]]
  },
  {
    cat: "utility", icon: "💸", title: "Currency Rates",
    desc: "This command shows the latest currency prices!",
    cmds: [["currency", "View rates"], ["نرخ ارز", "Persian"]]
  },
  {
    cat: "utility", icon: "🌤️", title: "Weather",
    desc: "With this command, you can view the weather status of any city.",
    cmds: [["weather [city]", "View weather"], ["هوا [شهر]", "Persian"]]
  },
  {
    cat: "utility", icon: "📰", title: "News",
    desc: "With this command, you can get the latest daily news.",
    cmds: [["news", "Get news"], ["اخبار", "Persian"]]
  },
  {
    cat: "utility", icon: "🌐", title: "Translate",
    desc: "With this command, you can translate Persian text to English and vice versa.",
    cmds: [["translate [text]", "Translate"], ["ترجمه [متن]", "Persian"]]
  },
  {
    cat: "utility", icon: "🎬", title: "Create GIF",
    desc: "Reply to a photo or GIF to convert it into a GIF. You can also add custom text.",
    cmds: [["make gif (reply)", "Convert to GIF"], ["make gif [text] (reply)", "With custom text"]]
  },
  {
    cat: "utility", icon: "🎲", title: "Dice",
    desc: "This command makes the bot roll a random dice for you.",
    cmds: [["dice", "Roll dice"], ["تاس", "Persian"]]
  },
  {
    cat: "utility", icon: "🔍", title: "Extract Hidden Text",
    desc: "This command extracts hidden text inside parentheses from replied messages.",
    cmds: [["extract (reply)", "Extract text"]]
  },
  {
    cat: "utility", icon: "🔊", title: "Echo System",
    desc: "Using this command, the bot deletes your message and resends it with a hidden mention.",
    cmds: [["echo [text]", "Send echo"]]
  },
  {
    cat: "utility", icon: "🔢", title: "Calculator",
    desc: "This feature lets you perform various mathematical operations!",
    cmds: [["calc [operation]", "Example: calc 2 + 9 × 5"]]
  },
  {
    cat: "utility", icon: "📜", title: "Hafez Poem",
    desc: "With this command, you can get a random Ghazal from Hafez's Divan.",
    cmds: [["hafez", "Get poem"], ["حافظ", "Persian"]]
  },
  {
    cat: "utility", icon: "📖", title: "Wikipedia",
    desc: "With this command, you can search any topic in Wikipedia.",
    cmds: [["wikipedia [query]", "Search"], ["ویکی [عبارت]", "Persian"]]
  },
  {
    cat: "utility", icon: "🧹", title: "Delete Messages",
    desc: "This command lets you delete a specific number of messages from the group!",
    cmds: [["purge [num]", "Max 100 messages"], ["پاک کردن [عدد] پیام", "Persian"]]
  },
  {
    cat: "utility", icon: "😶‍🌫️", title: "Send Anonymous Message",
    desc: "This command lets you send an anonymous message to a user in the group!",
    cmds: [["anonymous (reply)", "Send anonymous"], ["پیام ناشناس (ریپلای)", "Persian"]]
  },
  {
    cat: "utility", icon: "🔰", title: "Send Help Request",
    desc: "By sending this command, the support team will join your group to help you!",
    cmds: [["support", "Request support"], ["کمک", "Persian"]]
  },
  {
    cat: "utility", icon: "📊", title: "Group Statistics",
    desc: "This command shows the group user statistics!",
    cmds: [["stats", "View stats"], ["daily report", "Daily report"]]
  },
  {
    cat: "utility", icon: "📿", title: "Salavat",
    desc: "This command makes the bot send Salavat in the group!",
    cmds: [["salavat", "Send Salavat"], ["صلوات", "Persian"]]
  },
  {
    cat: "utility", icon: "📜", title: "Hadith",
    desc: "This command makes the bot send a random Hadith!",
    cmds: [["hadith", "Send hadith"], ["حدیث", "Persian"]]
  },
  {
    cat: "utility", icon: "🎭", title: "Joke",
    desc: "This command makes the bot send a random joke!",
    cmds: [["joke", "Send joke"], ["جوک", "Persian"]]
  },
  {
    cat: "utility", icon: "🤖", title: "Artificial Intelligence",
    desc: "You can ask any question to the bot's AI for free!",
    cmds: [["ai [question]", "Ask AI"], ["هوش [سوال]", "Persian"]]
  },
  {
    cat: "utility", icon: "📌", title: "Link",
    desc: "This command gives you the private link of the group!",
    cmds: [["link", "Get link"], ["لینک", "Persian"]]
  },
  {
    cat: "utility", icon: "🏓", title: "Ping",
    desc: "This command checks the bot response speed!",
    cmds: [["ping", "Check speed"], ["پینگ", "Persian"]]
  },
  {
    cat: "utility", icon: "👾", title: "Change Group Title",
    desc: "This command lets you change the group name!",
    cmds: [["set title [name]", "Change title"], ["تغییر نام [نام]", "Persian"]]
  },
  {
    cat: "utility", icon: "🔹", title: "Change Description",
    desc: "This command lets you change the group description!",
    cmds: [["set description [text]", "Change description"]]
  },
  {
    cat: "utility", icon: "🙎‍♂️", title: "Admin Commands",
    desc: "These commands are for managing group admins by the owner!",
    cmds: [["promote (reply)", "Add admin"], ["demote (reply)", "Remove admin"], ["list admin", "View list"]]
  },
  {
    cat: "utility", icon: "📌", title: "Pin",
    desc: "These commands let you manage pinned messages!",
    cmds: [["pin (reply)", "Pin message"], ["remove pin (reply)", "Unpin"], ["remove pins", "Unpin all"]]
  },
  {
    cat: "utility", icon: "⚙️", title: "Settings (Panel)",
    desc: "This command shows a brief panel of settings and locks in the group!",
    cmds: [["panel", "Show panel"], ["تنظیمات", "Persian"]]
  },
  {
    cat: "utility", icon: "👤", title: "User Info",
    desc: "This command shows the information of a specific user!",
    cmds: [["info (reply)", "User info"]]
  },
  {
    cat: "utility", icon: "👤", title: "My Info",
    desc: "This command shows your profile information!",
    cmds: [["info", "My info"], ["me", "My info"]]
  },
  {
    cat: "utility", icon: "⏰", title: "Date & Time",
    desc: "This command shows the current date and time!",
    cmds: [["date", "Show date"], ["time", "Show time"]]
  },
  {
    cat: "utility", icon: "🍂", title: "Bot Leave Group",
    desc: "These commands make the bot leave the group (owner only)!",
    cmds: [["bye", "Leave group"], ["مامپای برو", "Persian"]]
  },
  {
    cat: "utility", icon: "👤", title: "Leave Group Message",
    desc: "When a user leaves the group, the bot sends a notification!",
    cmds: [["leave on", "Enable"], ["leave off", "Disable"]]
  },
  {
    cat: "utility", icon: "🌱", title: "Welcome Message",
    desc: "When a new member joins, a welcome message is sent!",
    cmds: [["welcome on", "Enable"], ["welcome off", "Disable"]]
  },
  {
    cat: "utility", icon: "🎮", title: "Points System",
    desc: "Earn points by being active in the group, level up, and compete with others!",
    cmds: [["point", "Get points"], ["mypoints", "View points"], ["gamble [num]", "Gamble"], ["leaderboard", "Top users"]]
  },
  {
    cat: "games", icon: "👾", title: "Tic Tac Toe",
    desc: "Admins can start a Tic Tac Toe game!",
    cmds: [["tic", "Start game"], ["closegames", "Close games"]]
  },
  {
    cat: "games", icon: "👾", title: "Heads or Tails",
    desc: "Admins can start a Heads or Tails game!",
    cmds: [["guess", "Start game"], ["closegames", "Close games"]]
  },
  {
    cat: "games", icon: "💣", title: "Minesweeper",
    desc: "A classic single-player puzzle game. Find all empty cells in a 5x5 grid without hitting mines.",
    cmds: [["mines", "Start game"], ["minerob", "Start game"]]
  },
  {
    cat: "lists", icon: "📋", title: "View All Lists",
    desc: "These commands let you view various lists!",
    cmds: [["list mute", "Muted users"], ["list warn", "Warned users"], ["list admin", "Admins"], ["list badword", "Badwords"], ["list exempt", "Exempt users"]]
  },
  {
    cat: "lists", icon: "🧹", title: "Clear Lists",
    desc: "These commands let you clear specific lists!",
    cmds: [["clear filter", "Clear filters"], ["clear badword", "Clear badwords"], ["clear exempt", "Clear exempt"]]
  },
  {
    cat: "vip", icon: "💎", title: "VIP Subscription",
    desc: "By purchasing a VIP subscription, you can use special bot features such as bio locks, inappropriate name lock, edit lock, and message sending limits.",
    cmds: [["buy subscription", "View plans"], ["subscription", "Current subscription"]]
  },
  {
    cat: "vip", icon: "🔗", title: "Link in Bio Lock",
    desc: "If there is a link in the user's bio, the bot deletes the message. (VIP only)",
    cmds: [["lock link in bio", "Enable"], ["unlock link in bio", "Disable"]]
  },
  {
    cat: "vip", icon: "🔗", title: "ID in Bio Lock",
    desc: "If there is an ID in the user's bio, the bot deletes the message. (VIP only)",
    cmds: [["lock id in bio", "Enable"], ["unlock id in bio", "Disable"]]
  },
  {
    cat: "vip", icon: "🔗", title: "Username in Bio Lock",
    desc: "If there is a username in the user's bio, the bot deletes the message. (VIP only)",
    cmds: [["lock username in bio", "Enable"], ["unlock username in bio", "Disable"]]
  },
  {
    cat: "vip", icon: "🔞", title: "Badword in Bio Lock",
    desc: "If there are badwords in the user's bio, the bot deletes the message. (VIP only)",
    cmds: [["lock badword in bio", "Enable"], ["unlock badword in bio", "Disable"]]
  },
  {
    cat: "vip", icon: "📛", title: "Inappropriate Name Lock",
    desc: "Deletes messages from users whose names contain inappropriate words. (VIP only)",
    cmds: [["lock name", "Enable"], ["unlock name", "Disable"]]
  },
  {
    cat: "vip", icon: "✍️", title: "Edit Message Lock",
    desc: "Prevents users from editing messages and deletes edited messages. (VIP only)",
    cmds: [["lock edit", "Enable"], ["unlock edit", "Disable"]]
  },
  {
    cat: "vip", icon: "📊", title: "Message Sending Limit Lock",
    desc: "Set a daily limit for each message type. If exceeded, messages will be deleted. (VIP only)",
    cmds: [["lock limit [type]", "Enable"], ["set limit [type] [count]", "Set count"], ["unlock all limits", "Disable all"]]
  }
];

let currentLang = localStorage.getItem('mampy_lang') || 'fa';
let currentTheme = localStorage.getItem('mampy_theme') || 'dark';
let currentCat = 'all';
let searchQuery = '';

const $ = (s) => document.querySelector(s);
const $$ = (s) => document.querySelectorAll(s);

function applyTheme(theme) {
  document.documentElement.setAttribute('data-theme', theme);
  $('#themeIcon').textContent = theme === 'dark' ? '🌙' : '☀️';
  currentTheme = theme;
  localStorage.setItem('mampy_theme', theme);
}

function applyLang(lang) {
  currentLang = lang;
  localStorage.setItem('mampy_lang', lang);
  document.documentElement.lang = lang;
  document.documentElement.dir = lang === 'fa' ? 'rtl' : 'ltr';
  $('#langFlag').textContent = lang === 'fa' ? '🇮🇷' : '🇬🇧';
  $('#langLabel').textContent = lang === 'fa' ? 'FA' : 'EN';
  const t = I18N[lang];
  $$('[data-i18n]').forEach(el => {
    const key = el.getAttribute('data-i18n');
    if (t[key]) el.textContent = t[key];
  });
  $$('[data-i18n-placeholder]').forEach(el => {
    const key = el.getAttribute('data-i18n-placeholder');
    if (t[key]) el.placeholder = t[key];
  });
  renderCategories();
  renderHelp();
}

function renderCategories() {
  const wrap = $('#categories');
  wrap.innerHTML = '';
  const t = I18N[currentLang];
  const allBtn = document.createElement('button');
  allBtn.className = 'cat-btn' + (currentCat === 'all' ? ' active' : '');
  allBtn.innerHTML = `<span>✨</span><span>${t.catAll}</span>`;
  allBtn.onclick = () => { currentCat = 'all'; renderCategories(); renderHelp(); };
  wrap.appendChild(allBtn);
  CATEGORIES.forEach(cat => {
    const btn = document.createElement('button');
    btn.className = 'cat-btn' + (currentCat === cat.id ? ' active' : '');
    btn.innerHTML = `<span>${cat.icon}</span><span>${currentLang === 'fa' ? cat.fa : cat.en}</span>`;
    btn.onclick = () => { currentCat = cat.id; renderCategories(); renderHelp(); };
    wrap.appendChild(btn);
  });
}

function renderHelp() {
  const grid = $('#helpGrid');
  const t = I18N[currentLang];
  const data = HELP_DATA[currentLang] || [];
  let filtered = data;
  if (currentCat !== 'all') filtered = filtered.filter(h => h.cat === currentCat);
  if (searchQuery) {
    const q = searchQuery.toLowerCase();
    filtered = filtered.filter(h =>
      h.title.toLowerCase().includes(q) ||
      h.desc.toLowerCase().includes(q) ||
      h.cmds.some(c => c[0].toLowerCase().includes(q) || c[1].toLowerCase().includes(q))
    );
  }
  if (!filtered.length) {
    grid.innerHTML = `<div class="no-results"><div class="no-results-icon">🔍</div><h3>${t.noResults}</h3><p style="margin-top:8px;color:var(--text-muted)">${t.noResultsDesc}</p></div>`;
    return;
  }
  grid.innerHTML = '';
  filtered.forEach((item, idx) => {
    const card = document.createElement('div');
    card.className = 'help-card';
    card.style.animationDelay = (idx * 0.03) + 's';
    card.innerHTML = `
      <div class="help-card-head">
        <div class="help-icon">${item.icon}</div>
        <div class="help-card-title">${item.title}</div>
      </div>
      <div class="help-card-desc">${item.desc}</div>
      <div class="help-cmds">
        ${item.cmds.slice(0, 3).map(c => `<div class="cmd-line"><span class="cm-key">${c[0]}</span><span class="cm-arrow">←</span><span class="cm-val">${c[1]}</span></div>`).join('')}
      </div>
    `;
    card.onclick = () => openModal(item);
    grid.appendChild(card);
  });
}

function openModal(item) {
  const t = I18N[currentLang];
  const content = $('#modalContent');
  content.innerHTML = `
    <button class="modal-close" onclick="closeModal()">✕</button>
    <div class="modal-head">
      <div class="modal-icon">${item.icon}</div>
      <div class="modal-title">${item.title}</div>
    </div>
    <div class="modal-body">
      <p>${item.desc}</p>
      <h4>${t.cmds}:</h4>
      ${item.cmds.map(c => `<div class="cmd-block"><strong style="color:var(--accent-1)">${c[0]}</strong>  →  ${c[1]}</div>`).join('')}
    </div>
  `;
  $('#modalOverlay').classList.add('active');
  document.body.style.overflow = 'hidden';
}

function closeModal() {
  $('#modalOverlay').classList.remove('active');
  document.body.style.overflow = '';
}

$('#modalOverlay').addEventListener('click', (e) => {
  if (e.target.id === 'modalOverlay') closeModal();
});

document.addEventListener('keydown', (e) => {
  if (e.key === 'Escape') closeModal();
});

$('#themeToggle').onclick = () => applyTheme(currentTheme === 'dark' ? 'light' : 'dark');

$('#langToggle').onclick = () => applyLang(currentLang === 'fa' ? 'en' : 'fa');

$('#searchInput').addEventListener('input', (e) => {
  searchQuery = e.target.value.trim();
  renderHelp();
});

$('#toTop').onclick = () => window.scrollTo({ top: 0, behavior: 'smooth' });

window.addEventListener('scroll', () => {
  $('#toTop').classList.toggle('show', window.scrollY > 500);
});

const canvas = $('#starfield');
const ctx = canvas.getContext('2d');
let stars = [];
let shootingStars = [];

function resizeCanvas() {
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;
  initStars();
}

function initStars() {
  stars = [];
  const count = Math.floor((canvas.width * canvas.height) / 9000);
  for (let i = 0; i < count; i++) {
    stars.push({
      x: Math.random() * canvas.width,
      y: Math.random() * canvas.height,
      r: Math.random() * 1.6 + 0.3,
      a: Math.random() * 0.7 + 0.3,
      da: (Math.random() * 0.015 + 0.005) * (Math.random() > 0.5 ? 1 : -1),
      vx: (Math.random() - 0.5) * 0.15,
      vy: (Math.random() - 0.5) * 0.15
    });
  }
}

function spawnShootingStar() {
  if (Math.random() < 0.008 && shootingStars.length < 2) {
    shootingStars.push({
      x: Math.random() * canvas.width,
      y: Math.random() * canvas.height * 0.5,
      len: Math.random() * 120 + 60,
      speed: Math.random() * 8 + 6,
      angle: Math.PI / 4 + (Math.random() - 0.5) * 0.5,
      life: 1
    });
  }
}

function drawStars() {
  ctx.clearRect(0, 0, canvas.width, canvas.height);
  const isLight = currentTheme === 'light';
  stars.forEach(s => {
    s.a += s.da;
    if (s.a > 1 || s.a < 0.2) s.da *= -1;
    s.x += s.vx;
    s.y += s.vy;
    if (s.x < 0) s.x = canvas.width;
    if (s.x > canvas.width) s.x = 0;
    if (s.y < 0) s.y = canvas.height;
    if (s.y > canvas.height) s.y = 0;
    ctx.beginPath();
    ctx.arc(s.x, s.y, s.r, 0, Math.PI * 2);
    ctx.fillStyle = isLight
      ? `rgba(37,99,235,${s.a * 0.5})`
      : `rgba(200,230,255,${s.a})`;
    ctx.shadowBlur = isLight ? 4 : 8;
    ctx.shadowColor = isLight ? 'rgba(37,99,235,0.5)' : 'rgba(100,200,255,0.8)';
    ctx.fill();
  });
  ctx.shadowBlur = 0;
  spawnShootingStar();
  shootingStars = shootingStars.filter(ss => ss.life > 0);
  shootingStars.forEach(ss => {
    ss.x += Math.cos(ss.angle) * ss.speed;
    ss.y += Math.sin(ss.angle) * ss.speed;
    ss.life -= 0.012;
    const grad = ctx.createLinearGradient(
      ss.x, ss.y,
      ss.x - Math.cos(ss.angle) * ss.len,
      ss.y - Math.sin(ss.angle) * ss.len
    );
    if (isLight) {
      grad.addColorStop(0, `rgba(37,99,235,${ss.life})`);
      grad.addColorStop(1, 'rgba(37,99,235,0)');
    } else {
      grad.addColorStop(0, `rgba(150,220,255,${ss.life})`);
      grad.addColorStop(1, 'rgba(150,220,255,0)');
    }
    ctx.strokeStyle = grad;
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.moveTo(ss.x, ss.y);
    ctx.lineTo(
      ss.x - Math.cos(ss.angle) * ss.len,
      ss.y - Math.sin(ss.angle) * ss.len
    );
    ctx.stroke();
  });
  requestAnimationFrame(drawStars);
}

window.addEventListener('resize', resizeCanvas);
resizeCanvas();
drawStars();

applyTheme(currentTheme);
applyLang(currentLang);
</script>
</body>
</html>
