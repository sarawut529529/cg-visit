<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ระบบเยี่ยมบ้านผู้มีภาวะพึ่งพิง | ตำบลหนองแปน</title>
<link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>🏡</text></svg>">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Taviraj:wght@400;500;600;700&family=Sarabun:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<!-- ============================================================
     FIREBASE (compat SDK) — ต้องตั้งค่า firebaseConfig ด้านล่างก่อนใช้งาน
     ดูวิธีตั้งค่าใน README.md
     ============================================================ -->
<script src="https://www.gstatic.com/firebasejs/10.13.0/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.13.0/firebase-auth-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.13.0/firebase-firestore-compat.js"></script>

<!-- PDF export -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>

<style>
/* ===================== DESIGN TOKENS ===================== */
:root{
  --bg:#FAF6ED;
  --surface:#FFFFFF;
  --surface-soft:#FFFCF6;
  --ink:#2A2620;
  --muted:#8A8070;
  --border:#E6DCC4;
  --primary:#1F3D2B;
  --primary-light:#2F5940;
  --primary-dark:#142A1D;
  --gold:#B8874F;
  --gold-light:#E7C88F;
  --gold-soft:#F3E4C8;
  --wine:#7A2E3B;
  --wine-soft:#F4E1E3;
  --amber:#96631C;
  --amber-soft:#F6E7CE;
  --green-ok:#2F6B4F;
  --green-ok-soft:#E1EEE4;
  --radius-lg:18px;
  --radius-md:12px;
  --radius-sm:8px;
  --shadow-card:0 1px 0 rgba(31,61,43,0.06), 0 8px 24px -16px rgba(31,61,43,0.25);
  --font-display:'Taviraj',serif;
  --font-body:'Sarabun','Noto Sans Thai',sans-serif;
}
*{box-sizing:border-box;}
html,body{margin:0;padding:0;}
body{
  font-family:var(--font-body);
  background:var(--bg);
  color:var(--ink);
  min-height:100vh;
  -webkit-font-smoothing:antialiased;
}
h1,h2,h3,h4,.display{font-family:var(--font-display);font-weight:600;color:var(--primary-dark);}
a{color:inherit;}
button{font-family:inherit;cursor:pointer;}
input,select,textarea{font-family:inherit;font-size:15px;}
::selection{background:var(--gold-light);}

/* ===================== LAYOUT ===================== */
#app{display:flex;min-height:100vh;}
.sidebar{
  width:252px;flex-shrink:0;background:linear-gradient(180deg,var(--primary) 0%, var(--primary-dark) 100%);
  color:#EFE8D8;display:flex;flex-direction:column;position:sticky;top:0;height:100vh;overflow-y:auto;
}
.sidebar-brand{padding:26px 22px 18px;border-bottom:1px solid rgba(231,200,143,0.18);}
.sidebar-brand .emblem{font-size:30px;line-height:1;margin-bottom:8px;display:block;}
.sidebar-brand .name{font-family:var(--font-display);font-size:19px;font-weight:600;color:#F4E9CF;line-height:1.35;}
.sidebar-brand .sub{font-size:12px;color:#B9C9BB;margin-top:4px;letter-spacing:.02em;}
.nav{flex:1;padding:16px 14px;display:flex;flex-direction:column;gap:4px;}
.nav a{
  display:flex;align-items:center;gap:11px;padding:11px 14px;border-radius:999px;
  color:#DCE6DB;text-decoration:none;font-size:14.5px;transition:background .15s, color .15s;
}
.nav a svg{width:18px;height:18px;flex-shrink:0;opacity:.85;}
.nav a:hover{background:rgba(231,200,143,0.1);color:#F4E9CF;}
.nav a.active{background:var(--gold);color:#2A1F0E;font-weight:600;}
.nav a.active svg{opacity:1;}
.nav .section-label{font-size:11px;text-transform:uppercase;letter-spacing:.08em;color:#8FA491;margin:14px 14px 4px;}
.sidebar-foot{padding:16px 22px 20px;border-top:1px solid rgba(231,200,143,0.18);font-size:12.5px;color:#A9BCA9;}
.sidebar-user{padding:14px 18px;margin:0 14px 6px;background:rgba(0,0,0,0.16);border-radius:var(--radius-md);}
.sidebar-user .role-badge{display:inline-block;font-size:11px;padding:2px 9px;border-radius:99px;background:var(--gold-soft);color:#5A3E17;font-weight:600;margin-top:4px;}
.sidebar-user .uname{font-size:14px;font-weight:600;color:#F4E9CF;}

.main{flex:1;min-width:0;display:flex;flex-direction:column;}
.topbar{
  display:flex;align-items:center;justify-content:space-between;padding:16px 32px;
  background:rgba(250,246,237,0.9);backdrop-filter:blur(6px);position:sticky;top:0;z-index:20;
  border-bottom:1px solid var(--border);
}
.topbar .page-title{font-size:22px;}
.topbar .page-title .eyebrow{display:block;font-family:var(--font-body);font-size:12.5px;color:var(--gold);letter-spacing:.04em;margin-bottom:2px;}
.topbar-actions{display:flex;align-items:center;gap:10px;}
.view-container{padding:28px 32px 60px;max-width:1280px;width:100%;margin:0 auto;}

/* mobile nav toggle */
.menu-toggle{display:none;background:none;border:none;font-size:24px;color:var(--primary);}
@media (max-width:980px){
  .sidebar{position:fixed;left:0;top:0;bottom:0;z-index:50;transform:translateX(-100%);transition:transform .2s;width:264px;}
  .sidebar.open{transform:translateX(0);box-shadow:0 0 40px rgba(0,0,0,.35);}
  .menu-toggle{display:inline-flex;}
  .view-container{padding:20px 16px 48px;}
  .topbar{padding:14px 16px;}
  .sidebar-backdrop{display:none;position:fixed;inset:0;background:rgba(0,0,0,.35);z-index:40;}
  .sidebar-backdrop.show{display:block;}
}

/* ===================== BUTTONS ===================== */
.btn{display:inline-flex;align-items:center;gap:8px;padding:10px 18px;border-radius:999px;border:1px solid transparent;font-size:14.5px;font-weight:600;transition:filter .15s, transform .05s;}
.btn:active{transform:scale(.98);}
.btn-primary{background:var(--primary);color:#F4E9CF;}
.btn-primary:hover{filter:brightness(1.12);}
.btn-gold{background:var(--gold);color:#2A1F0E;}
.btn-gold:hover{filter:brightness(1.07);}
.btn-outline{background:transparent;color:var(--primary);border-color:var(--border);}
.btn-outline:hover{background:var(--surface-soft);border-color:var(--primary);}
.btn-ghost{background:transparent;color:var(--muted);}
.btn-ghost:hover{color:var(--ink);}
.btn-danger{background:var(--wine-soft);color:var(--wine);}
.btn-danger:hover{background:var(--wine);color:#fff;}
.btn-sm{padding:6px 13px;font-size:13px;}
.btn:disabled{opacity:.5;cursor:not-allowed;}

/* ===================== CARDS ===================== */
.card{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius-lg);box-shadow:var(--shadow-card);}
.card-pad{padding:22px 24px;}
.divider{height:1px;background:var(--border);border:none;margin:18px 0;}

/* ===================== DASHBOARD ===================== */
.hero{
  background:linear-gradient(120deg,var(--primary-dark) 0%, var(--primary) 60%, var(--primary-light) 100%);
  border-radius:var(--radius-lg);padding:38px 36px;color:#F4E9CF;position:relative;overflow:hidden;margin-bottom:26px;
}
.hero::after{content:"";position:absolute;right:-60px;top:-60px;width:260px;height:260px;border-radius:50%;background:radial-gradient(circle,rgba(231,200,143,0.18),transparent 70%);}
.hero .eyebrow{color:var(--gold-light);font-size:13px;letter-spacing:.06em;margin-bottom:8px;}
.hero h1{color:#FBF3E1;font-size:28px;margin:0 0 8px;}
.hero p{color:#C9D6CA;font-size:14.5px;max-width:640px;line-height:1.7;margin:0;}

.stat-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px;margin-bottom:26px;}
.stat-card{background:var(--surface);border:1px solid var(--border);border-left:4px solid var(--gold);border-radius:var(--radius-md);padding:18px 20px;}
.stat-card .num{font-family:var(--font-display);font-size:32px;color:var(--primary-dark);line-height:1;}
.stat-card .lbl{font-size:13px;color:var(--muted);margin-top:8px;}
.stat-card.wine{border-left-color:var(--wine);}
.stat-card.green{border-left-color:var(--green-ok);}

.section-heading{display:flex;align-items:center;justify-content:space-between;margin:30px 0 14px;}
.section-heading h2{font-size:19px;margin:0;}
.section-heading .hint{font-size:13px;color:var(--muted);}

.progress-row{display:flex;align-items:center;gap:12px;padding:12px 0;border-bottom:1px solid var(--border);}
.progress-row:last-child{border-bottom:none;}
.progress-row .name{flex:0 0 200px;font-size:14px;font-weight:600;}
.progress-row .meta{flex:0 0 90px;font-size:12px;color:var(--muted);}
.progress-track{flex:1;height:9px;border-radius:99px;background:var(--gold-soft);overflow:hidden;}
.progress-fill{height:100%;border-radius:99px;background:var(--green-ok);transition:width .3s;}
.progress-fill.under{background:var(--wine);}
.progress-count{flex:0 0 56px;text-align:right;font-size:13px;font-weight:600;}

.badge{display:inline-flex;align-items:center;padding:3px 11px;border-radius:99px;font-size:12px;font-weight:600;}
.badge-g1{background:var(--green-ok-soft);color:var(--green-ok);}
.badge-g2{background:var(--amber-soft);color:var(--amber);}
.badge-g3{background:var(--wine-soft);color:var(--wine);}
.badge-pending{background:var(--amber-soft);color:var(--amber);}
.badge-approved{background:var(--green-ok-soft);color:var(--green-ok);}
.badge-rejected{background:var(--wine-soft);color:var(--wine);}

/* ===================== FORMS ===================== */
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px;}
.form-grid.cols-1{grid-template-columns:1fr;}
@media (max-width:700px){.form-grid{grid-template-columns:1fr;}}
.field{display:flex;flex-direction:column;gap:6px;}
.field label{font-size:13.5px;font-weight:600;color:var(--primary-dark);}
.field .req{color:var(--wine);}
.field input[type=text],.field input[type=date],.field input[type=tel],.field input[type=password],.field input[type=number],.field input[type=file],.field select,.field textarea{
  padding:10px 13px;border:1px solid var(--border);border-radius:var(--radius-sm);background:var(--surface-soft);color:var(--ink);outline:none;
}
.field input:focus,.field select:focus,.field textarea:focus{border-color:var(--gold);box-shadow:0 0 0 3px var(--gold-soft);}
.field textarea{resize:vertical;min-height:80px;}
.field .helptext{font-size:12px;color:var(--muted);}
.checkline{display:flex;align-items:flex-start;gap:9px;padding:8px 0;font-size:14px;}
.checkline input{margin-top:3px;}

/* ===================== TABLE ===================== */
.table-wrap{overflow-x:auto;}
table.data{width:100%;border-collapse:collapse;font-size:14px;}
table.data th{text-align:left;font-size:12.5px;text-transform:uppercase;letter-spacing:.03em;color:var(--muted);padding:10px 12px;border-bottom:2px solid var(--border);}
table.data td{padding:11px 12px;border-bottom:1px solid var(--border);vertical-align:middle;}
table.data tr:hover td{background:var(--surface-soft);}
.avatar{width:38px;height:38px;border-radius:50%;object-fit:cover;background:var(--gold-soft);border:1px solid var(--border);}
.avatar-lg{width:100px;height:100px;border-radius:14px;object-fit:cover;background:var(--gold-soft);border:1px solid var(--border);}

/* ===================== MISC ===================== */
.empty-state{text-align:center;padding:50px 20px;color:var(--muted);}
.empty-state .ic{font-size:38px;margin-bottom:10px;}
.tabs{display:flex;gap:6px;border-bottom:1px solid var(--border);margin-bottom:20px;flex-wrap:wrap;}
.tab{padding:10px 16px;font-size:14px;font-weight:600;color:var(--muted);border-bottom:2px solid transparent;background:none;border-top:none;border-left:none;border-right:none;}
.tab.active{color:var(--primary-dark);border-bottom-color:var(--gold);}
.modal-backdrop{position:fixed;inset:0;background:rgba(20,15,5,.42);display:flex;align-items:center;justify-content:center;z-index:100;padding:20px;}
.modal{background:var(--surface);border-radius:var(--radius-lg);max-width:480px;width:100%;padding:28px;max-height:90vh;overflow-y:auto;}
.modal.wide{max-width:760px;}
.modal h3{margin-top:0;}
.toast-wrap{position:fixed;bottom:22px;right:22px;z-index:200;display:flex;flex-direction:column;gap:10px;}
.toast{padding:13px 18px;border-radius:var(--radius-md);background:var(--primary-dark);color:#F4E9CF;font-size:14px;box-shadow:0 10px 30px rgba(0,0,0,.25);min-width:240px;}
.toast.err{background:var(--wine);}
.toast.ok{background:var(--green-ok);}
.center-page{min-height:100vh;display:flex;align-items:center;justify-content:center;padding:20px;}
.auth-card{max-width:420px;width:100%;}
.auth-card .emblem{font-size:36px;}
.link-btn{background:none;border:none;color:var(--primary);text-decoration:underline;font-size:13.5px;padding:0;}
.photo-preview{width:100%;max-width:220px;border-radius:var(--radius-md);border:1px solid var(--border);object-fit:cover;}
.pill-select{display:flex;gap:8px;flex-wrap:wrap;}
.pill-opt{padding:9px 16px;border-radius:999px;border:1px solid var(--border);background:var(--surface-soft);font-size:13.5px;cursor:pointer;font-weight:600;color:var(--muted);}
.pill-opt.sel{background:var(--primary);color:#F4E9CF;border-color:var(--primary);}
.adl-item{padding:12px 0;border-bottom:1px dashed var(--border);}
.adl-item:last-child{border-bottom:none;}
.adl-item .q{font-size:13.5px;font-weight:600;margin-bottom:8px;}
.adl-opts{display:flex;flex-wrap:wrap;gap:7px;}
.adl-opt{padding:6px 12px;border:1px solid var(--border);border-radius:999px;font-size:12.5px;cursor:pointer;color:var(--muted);background:var(--surface-soft);}
.adl-opt.sel{background:var(--gold);border-color:var(--gold);color:#2A1F0E;font-weight:700;}
.adl-total{margin-top:14px;padding:12px 16px;background:var(--gold-soft);border-radius:var(--radius-sm);font-weight:700;color:#5A3E17;}
.loader{width:38px;height:38px;border:4px solid var(--gold-soft);border-top-color:var(--gold);border-radius:50%;animation:spin 0.8s linear infinite;}
@keyframes spin{to{transform:rotate(360deg);}}
.kicker{font-size:12px;letter-spacing:.06em;color:var(--gold);font-weight:700;text-transform:uppercase;margin-bottom:4px;}

/* ===================== PDF / PRINT TEMPLATE ===================== */
.pdf-root{position:fixed;left:-9999px;top:0;}
.report-page{
  width:210mm;min-height:297mm;background:#fff;padding:16mm 15mm;font-family:'Sarabun',sans-serif;color:#1a1a1a;
  page-break-after:always;position:relative;box-sizing:border-box;
}
.report-page:last-child{page-break-after:auto;}
.rp-header{text-align:center;border-bottom:3px double #1F3D2B;padding-bottom:10px;margin-bottom:16px;}
.rp-header .org{font-size:13px;color:#555;}
.rp-header h2{font-family:'Sarabun',sans-serif;font-size:19px;margin:4px 0 2px;color:#1F3D2B;}
.rp-header .sub{font-size:13px;color:#555;}
.rp-grid{display:grid;grid-template-columns:100px 1fr;gap:6px 14px;font-size:13.5px;margin-bottom:14px;}
.rp-grid .k{color:#666;}
.rp-photo-row{display:flex;gap:14px;margin-bottom:14px;}
.rp-photo-row img{width:110px;height:110px;object-fit:cover;border-radius:8px;border:1px solid #ddd;}
.rp-table{width:100%;border-collapse:collapse;font-size:12.5px;margin-top:6px;}
.rp-table th,.rp-table td{border:1px solid #ccc;padding:6px 8px;text-align:left;}
.rp-table th{background:#F3E4C8;color:#5A3E17;}
.rp-section-title{font-size:14.5px;font-weight:700;color:#1F3D2B;margin:16px 0 8px;border-left:4px solid #B8874F;padding-left:8px;}
.rp-signature{margin-top:40px;display:flex;justify-content:flex-end;font-size:13px;text-align:center;}
.rp-signature .line{margin-top:36px;border-top:1px solid #999;padding-top:4px;width:200px;}
.rp-bar-row{display:flex;align-items:center;gap:10px;font-size:12.5px;margin-bottom:6px;}
.rp-bar-row .m{width:80px;color:#555;}
.rp-bar-track{flex:1;height:14px;background:#eee;border-radius:4px;overflow:hidden;}
.rp-bar-fill{height:100%;background:#1F3D2B;}
.rp-bar-val{width:34px;text-align:right;font-weight:700;}
</style>
</head>
<body>

<div id="loading-screen" class="center-page">
  <div style="text-align:center;">
    <div class="loader" style="margin:0 auto 14px;"></div>
    <div style="color:var(--muted);font-size:14px;">กำลังโหลดระบบ...</div>
  </div>
</div>

<div id="app" style="display:none;">
  <div class="sidebar-backdrop" id="sidebarBackdrop"></div>
  <aside class="sidebar" id="sidebar">
    <div class="sidebar-brand">
      <span class="emblem">🏡</span>
      <div class="name">ระบบเยี่ยมบ้าน<br>ผู้มีภาวะพึ่งพิง</div>
      <div class="sub">ตำบลหนองแปน อำเภอเจริญศิลป์ จังหวัดสกลนคร</div>
    </div>
    <div id="sidebarUserBox"></div>
    <nav class="nav" id="navMenu"></nav>
    <div class="sidebar-foot">© CG Home Visit System</div>
  </aside>

  <div class="main">
    <div class="topbar">
      <div style="display:flex;align-items:center;gap:10px;">
        <button class="menu-toggle" id="menuToggle">☰</button>
        <div class="page-title">
          <span class="eyebrow" id="pageEyebrow">ภาพรวม</span>
          <span id="pageTitle">แดชบอร์ด</span>
        </div>
      </div>
      <div class="topbar-actions" id="topbarActions"></div>
    </div>
    <div class="view-container" id="view"></div>
  </div>
</div>

<div class="toast-wrap" id="toastWrap"></div>
<div id="modalRoot"></div>
<div class="pdf-root" id="pdfRoot"></div>

<script>
/* ======================================================================
   FIREBASE CONFIG — แก้ค่าด้านล่างนี้เป็นของโปรเจกต์ Firebase ของคุณเอง
   (Firebase Console > Project settings > General > Your apps > SDK setup)
   ====================================================================== */
const firebaseConfig = {
  apiKey: "AIzaSyDwmk2wi_aeV0K1bO1PAkGYSOjA7gQOKBE",
  authDomain: "ltc-nongpan.firebaseapp.com",
  databaseURL: "https://ltc-nongpan-default-rtdb.asia-southeast1.firebasedatabase.app",
  projectId: "ltc-nongpan",
  storageBucket: "ltc-nongpan.firebasestorage.app",
  messagingSenderId: "1024118162465",
  appId: "1:1024118162465:web:4f0bbd1e005f6542924f6"
};

firebase.initializeApp(firebaseConfig);
const auth = firebase.auth();
const db = firebase.firestore();
const FAKE_EMAIL_DOMAIN = "@cgvisit.local";

// ImgBB — ใช้เก็บรูปภาพจริงบนอินเทอร์เน็ต (เก็บเฉพาะลิงก์ URL ไว้ใน Firestore แทน base64
// เพื่อไม่ให้ชนขีดจำกัดขนาดเอกสาร 1MB ของ Firestore และโหลดข้อมูลได้เร็วขึ้น)
const IMGBB_API_KEY = "8eb385d52c3d5019be8763d5074e9026";
async function uploadToImgbb(dataUrl){
  if(!dataUrl) return null;
  if(/^https?:\/\//.test(dataUrl)) return dataUrl; // already an uploaded URL, no need to re-upload
  const base64 = dataUrl.split(",")[1];
  const form = new FormData();
  form.append("image", base64);
  const res = await fetch(`https://api.imgbb.com/1/upload?key=${IMGBB_API_KEY}`, { method:"POST", body: form });
  const json = await res.json();
  if(!json.success) throw new Error("อัปโหลดรูปภาพไม่สำเร็จ กรุณาลองใหม่");
  return json.data.url;
}

/* ======================================================================
   CONSTANTS
   ====================================================================== */
const ORG_LINE1 = "ตำบลหนองแปน อำเภอเจริญศิลป์ จังหวัดสกลนคร";
const REPORT_TITLE = "รายงานการเยี่ยมผู้มีภาวะพึ่งพิงตำบลหนองแปน อำเภอเจริญศิลป์ จังหวัดสกลนคร";

const GROUP_INFO = {
  "1": { label: "กลุ่มที่ 1 (ติดบ้าน)", target: 1, unit: "เดือน", badge:"badge-g1",
    desc:"เคลื่อนไหวเองได้บ้าง มีปัญหาการกิน/ขับถ่าย (ไม่สับสน) — เยี่ยมอย่างน้อย 1 ครั้ง/เดือน" },
  "2": { label: "กลุ่มที่ 2 (ติดบ้าน/เริ่มติดเตียง)", target: 2, unit: "เดือน", badge:"badge-g2",
    desc:"เคลื่อนไหวได้บ้าง มีภาวะสับสน มีปัญหาการกิน/ขับถ่าย — เยี่ยมอย่างน้อย 2 ครั้ง/เดือน" },
  "3": { label: "กลุ่มที่ 3 (ติดเตียง)", target: 4, unit: "เดือน", badge:"badge-g3",
    desc:"เคลื่อนไหวเองไม่ได้ นอนติดเตียง อาการรุนแรง — เยี่ยมอย่างน้อยสัปดาห์ละ 1 ครั้ง (4 ครั้ง/เดือน) ประเมิน ADL ทุกครั้ง" }
};
const ACTIVITIES = [
  "ให้ความรู้ผู้ป่วยและญาติ",
  "กายภาพบำบัด/ออกกำลังกาย",
  "อาบน้ำ/สระผม/ตัดเล็บ/ทำความสะอาดร่างกาย",
  "ทำความสะอาดบ้าน พัฒนาสิ่งแวดล้อมรอบบ้าน",
  "ป้อนอาหาร/ดูแลโภชนาการ",
  "วัดความดันโลหิต/เจาะน้ำตาลในเลือด",
  "เยี่ยมให้กำลังใจ"
];
// Barthel ADL Index (Thai LTC standard, 10 items, total 0-20)
const ADL_ITEMS = [
  { key:"feeding", q:"1. รับประทานอาหาร", opts:[[0,"ทำเองไม่ได้"],[5,"ช่วยเหลือบางส่วน"],[10,"ทำเองได้"]] },
  { key:"grooming", q:"2. ล้างหน้า หวีผม แปรงฟัน โกนหนวด", opts:[[0,"ทำเองไม่ได้/ต้องช่วย"],[5,"ทำเองได้"]] },
  { key:"transfer", q:"3. ลุกนั่งจากที่นอน/เตียง", opts:[[0,"ทำเองไม่ได้เลย"],[5,"ต้องช่วยเหลือมาก"],[10,"ช่วยเหลือเล็กน้อย"],[15,"ทำเองได้"]] },
  { key:"toilet", q:"4. การใช้ห้องน้ำ", opts:[[0,"ช่วยเหลือทั้งหมด"],[5,"ช่วยเหลือบางส่วน"],[10,"ทำเองได้"]] },
  { key:"mobility", q:"5. การเคลื่อนที่ภายในบ้าน/ห้อง", opts:[[0,"เคลื่อนที่ไม่ได้"],[5,"ใช้รถเข็นเอง"],[10,"เดินโดยมีคนช่วย"],[15,"เดินได้เอง"]] },
  { key:"dressing", q:"6. การสวมใส่เสื้อผ้า", opts:[[0,"ทำเองไม่ได้"],[5,"ช่วยเหลือบางส่วน"],[10,"ทำเองได้"]] },
  { key:"stairs", q:"7. การขึ้นลงบันได 1 ชั้น", opts:[[0,"ทำเองไม่ได้"],[5,"ต้องช่วยเหลือ"],[10,"ทำเองได้"]] },
  { key:"bathing", q:"8. การอาบน้ำ", opts:[[0,"ต้องช่วยเหลือ"],[5,"ทำเองได้"]] },
  { key:"bowel", q:"9. การกลั้นการถ่ายอุจจาระ", opts:[[0,"กลั้นไม่ได้"],[5,"กลั้นไม่ได้เป็นบางครั้ง"],[10,"กลั้นได้ปกติ"]] },
  { key:"bladder", q:"10. การกลั้นปัสสาวะ", opts:[[0,"กลั้นไม่ได้"],[5,"กลั้นไม่ได้เป็นบางครั้ง"],[10,"กลั้นได้ปกติ"]] }
];

/* ======================================================================
   APP STATE
   ====================================================================== */
let state = {
  user: null,        // { uid, username, fullName, role, status }
  myCg: null,        // linked cgs doc {id,...} if role CG
  cgs: [],
  dependents: [],
  route: "dashboard"
};

/* ======================================================================
   UTILITIES
   ====================================================================== */
function $(sel, root){ return (root||document).querySelector(sel); }
function $all(sel, root){ return Array.from((root||document).querySelectorAll(sel)); }
function esc(str){ if(str===undefined||str===null) return ""; return String(str).replace(/[&<>"']/g, c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c])); }
function toast(msg, type){
  const wrap = $("#toastWrap");
  const el = document.createElement("div");
  el.className = "toast" + (type?(" "+type):"");
  el.textContent = msg;
  wrap.appendChild(el);
  setTimeout(()=>{ el.style.opacity="0"; el.style.transition="opacity .3s"; setTimeout(()=>el.remove(),300); }, 3400);
}
function fmtDate(d){
  if(!d) return "-";
  const dt = (d instanceof Date) ? d : new Date(d);
  if(isNaN(dt)) return "-";
  const thMonths=["ม.ค.","ก.พ.","มี.ค.","เม.ย.","พ.ค.","มิ.ย.","ก.ค.","ส.ค.","ก.ย.","ต.ค.","พ.ย.","ธ.ค."];
  return `${dt.getDate()} ${thMonths[dt.getMonth()]} ${dt.getFullYear()+543}`;
}
function fmtMonthLabel(ym){ // "2026-09" -> "กันยายน 2569"
  const thMonthsFull=["มกราคม","กุมภาพันธ์","มีนาคม","เมษายน","พฤษภาคม","มิถุนายน","กรกฎาคม","สิงหาคม","กันยายน","ตุลาคม","พฤศจิกายน","ธันวาคม"];
  const [y,m]=ym.split("-").map(Number);
  return `${thMonthsFull[m-1]} ${y+543}`;
}
function todayStr(){ return new Date().toISOString().slice(0,10); }
function curYm(){ return new Date().toISOString().slice(0,7); }
function ymOf(dateStr){ return (dateStr||"").slice(0,7); }
function uid(){ return Math.random().toString(36).slice(2,10)+Date.now().toString(36); }

function compressImage(file, maxW){
  return new Promise((resolve,reject)=>{
    if(!file) return resolve(null);
    const reader = new FileReader();
    reader.onload = e=>{
      const img = new Image();
      img.onload = ()=>{
        const scale = Math.min(1, (maxW||900)/img.width);
        const w = Math.round(img.width*scale), h = Math.round(img.height*scale);
        const canvas = document.createElement("canvas");
        canvas.width=w; canvas.height=h;
        canvas.getContext("2d").drawImage(img,0,0,w,h);
        resolve(canvas.toDataURL("image/jpeg",0.62));
      };
      img.onerror = reject;
      img.src = e.target.result;
    };
    reader.onerror = reject;
    reader.readAsDataURL(file);
  });
}

function iconSvg(name){
  const icons = {
    dashboard:'<path d="M3 13h8V3H3v10zm0 8h8v-6H3v6zm10 0h8V11h-8v10zm0-18v6h8V3h-8z"/>',
    report:'<path d="M14 2H6a2 2 0 00-2 2v16a2 2 0 002 2h12a2 2 0 002-2V8l-6-6z"/><path d="M14 2v6h6M9 13h6M9 17h6M9 9h1" stroke="currentColor" fill="none" stroke-width="1.6"/>',
    cg:'<circle cx="12" cy="8" r="4"/><path d="M4 21c0-4 3.6-7 8-7s8 3 8 7"/>',
    dependent:'<path d="M12 21s-7-4.5-9.5-9A5.5 5.5 0 0112 6a5.5 5.5 0 019.5 6c-2.5 4.5-9.5 9-9.5 9z"/>',
    export:'<path d="M12 3v12m0 0l-4-4m4 4l4-4M4 21h16" stroke="currentColor" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>',
    admin:'<path d="M12 2l8 4v6c0 5-3.4 8.4-8 10-4.6-1.6-8-5-8-10V6l8-4z"/>',
    logout:'<path d="M9 21H5a2 2 0 01-2-2V5a2 2 0 012-2h4M16 17l5-5-5-5M21 12H9" stroke="currentColor" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>',
    login:'<path d="M15 3h4a2 2 0 012 2v14a2 2 0 01-2 2h-4M10 17l-5-5 5-5M3 12h12" stroke="currentColor" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>'
  };
  return `<svg viewBox="0 0 24 24" fill="currentColor">${icons[name]||""}</svg>`;
}

/* ======================================================================
   AUTH
   ====================================================================== */
async function doRegister(data){
  const email = data.username.trim().toLowerCase() + FAKE_EMAIL_DOMAIN;
  const isAdminBootstrap = data.username.trim().toLowerCase() === "admin";
  if(isAdminBootstrap && data.password !== "05579"){
    throw new Error("บัญชี admin ต้องใช้รหัสผ่านที่กำหนดไว้เท่านั้น");
  }
  const cred = await auth.createUserWithEmailAndPassword(email, data.password);
  const profile = {
    username: data.username.trim().toLowerCase(),
    fullName: data.fullName.trim(),
    role: isAdminBootstrap ? "admin" : data.role,
    status: isAdminBootstrap ? "approved" : "pending",
    createdAt: firebase.firestore.FieldValue.serverTimestamp()
  };
  await db.collection("users").doc(cred.user.uid).set(profile);
  await auth.signOut();
  return profile;
}

async function doLogin(username, password){
  const email = username.trim().toLowerCase() + FAKE_EMAIL_DOMAIN;
  const cred = await auth.signInWithEmailAndPassword(email, password);
  const snap = await db.collection("users").doc(cred.user.uid).get();
  if(!snap.exists){ await auth.signOut(); throw new Error("ไม่พบข้อมูลผู้ใช้งาน"); }
  const profile = snap.data();
  if(profile.status === "pending"){ await auth.signOut(); throw new Error("บัญชีของคุณกำลังรออนุมัติจากผู้ดูแลระบบ"); }
  if(profile.status === "rejected"){ await auth.signOut(); throw new Error("บัญชีนี้ไม่ได้รับอนุมัติให้เข้าใช้งาน"); }
  return profile;
}

function doLogout(){ auth.signOut(); }

/* ======================================================================
   FIRESTORE DATA HELPERS
   ====================================================================== */
async function loadCgs(){
  const snap = await db.collection("cgs").orderBy("fullName").get();
  state.cgs = snap.docs.map(d=>({id:d.id, ...d.data()}));
}
async function loadDependents(){
  const snap = await db.collection("dependents").orderBy("fullName").get();
  state.dependents = snap.docs.map(d=>({id:d.id, ...d.data()}));
}
async function resolveMyCg(){
  state.myCg = null;
  if(state.user && state.user.role === "CG"){
    const snap = await db.collection("cgs").where("linkedUsername","==",state.user.username).limit(1).get();
    if(!snap.empty) state.myCg = {id:snap.docs[0].id, ...snap.docs[0].data()};
  }
}
async function bumpStats(patch){
  const ref = db.collection("meta").doc("stats");
  await db.runTransaction(async tx=>{
    const doc = await tx.get(ref);
    const cur = doc.exists ? doc.data() : {};
    const next = {...cur};
    for(const k in patch){
      next[k] = (cur[k]||0) + patch[k];
    }
    tx.set(ref, next, {merge:true});
  });
}
async function bumpMonthlyStat(ym, group){
  const ref = db.collection("meta").doc("stats");
  const field = `visits_${ym}`;
  const fieldG = `visits_${ym}_g${group}`;
  await ref.set({
    [field]: firebase.firestore.FieldValue.increment(1),
    [fieldG]: firebase.firestore.FieldValue.increment(1),
    totalVisits: firebase.firestore.FieldValue.increment(1)
  }, {merge:true});
}

/* ======================================================================
   ROUTER
   ====================================================================== */
const ROUTES = {
  dashboard: { title:"แดชบอร์ด", eyebrow:"ภาพรวมระบบ", auth:false, render: viewDashboard },
  login: { title:"เข้าสู่ระบบ", eyebrow:"สมาชิก", auth:false, render: viewLogin },
  register: { title:"สมัครสมาชิก", eyebrow:"สมาชิกใหม่", auth:false, render: viewRegister },
  report: { title:"ส่งรายงานการเยี่ยมบ้าน", eyebrow:"CG / CM / Admin", auth:true, roles:["CG","CM","admin"], render: viewReport },
  cgs: { title:"จัดการข้อมูล CG", eyebrow:"CM / Admin", auth:true, roles:["CM","admin"], render: viewCgs },
  dependents: { title:"จัดการข้อมูลผู้มีภาวะพึ่งพิง", eyebrow:"ข้อมูลหลัก", auth:true, roles:["CG","CM","admin"], render: viewDependents },
  reports: { title:"ออกรายงาน (PDF)", eyebrow:"สรุปและเอกสาร", auth:true, roles:["CG","CM","admin"], render: viewReportsExport },
  admin: { title:"จัดการผู้ใช้งาน", eyebrow:"Admin", auth:true, roles:["admin"], render: viewAdmin }
};

function navigate(route){
  if(!ROUTES[route]) route = "dashboard";
  const def = ROUTES[route];
  if(def.auth && !state.user){ route="login"; }
  else if(def.roles && state.user && !def.roles.includes(state.user.role)){
    toast("คุณไม่มีสิทธิ์เข้าถึงเมนูนี้","err"); route="dashboard";
  }
  state.route = route;
  window.location.hash = route;
  renderShell();
}
window.addEventListener("hashchange", ()=>{
  const r = window.location.hash.replace("#","") || "dashboard";
  state.route = r;
  renderShell();
});

/* ======================================================================
   SHELL (sidebar / topbar / view render)
   ====================================================================== */
function menuItem(route, icon, label){
  return `<a href="#${route}" class="${state.route===route?'active':''}" onclick="event.preventDefault();navigate('${route}');closeSidebarMobile();">${iconSvg(icon)}<span>${label}</span></a>`;
}
function renderSidebar(){
  let html = "";
  html += menuItem("dashboard","dashboard","แดชบอร์ด");
  if(state.user){
    html += `<div class="section-label">งานเยี่ยมบ้าน</div>`;
    html += menuItem("report","report","ส่งรายงานการเยี่ยม");
    html += menuItem("dependents","dependent","ข้อมูลผู้มีภาวะพึ่งพิง");
    if(state.user.role==="CM"||state.user.role==="admin"){
      html += menuItem("cgs","cg","จัดการข้อมูล CG");
    }
    html += menuItem("reports","export","ออกรายงาน (PDF)");
    if(state.user.role==="admin"){
      html += `<div class="section-label">ระบบ</div>`;
      html += menuItem("admin","admin","อนุมัติผู้ใช้งาน");
    }
  }
  $("#navMenu").innerHTML = html;

  const box = $("#sidebarUserBox");
  if(state.user){
    const roleLabel = {CG:"อาสาสมัคร CG", CM:"ผู้จัดการรายกรณี (CM)", admin:"ผู้ดูแลระบบ"}[state.user.role]||state.user.role;
    box.innerHTML = `<div class="sidebar-user">
      <div class="uname">${esc(state.user.fullName)}</div>
      <div style="font-size:12.5px;color:#B9C9BB;">@${esc(state.user.username)}</div>
      <span class="role-badge">${roleLabel}</span>
    </div>`;
  } else {
    box.innerHTML = "";
  }
}
function renderTopbarActions(){
  const el = $("#topbarActions");
  if(state.user){
    el.innerHTML = `<button class="btn btn-outline btn-sm" onclick="doLogout()">${iconSvg("logout")} ออกจากระบบ</button>`;
  } else {
    el.innerHTML = `
      <button class="btn btn-outline btn-sm" onclick="navigate('login')">${iconSvg("login")} เข้าสู่ระบบ</button>
      <button class="btn btn-gold btn-sm" onclick="navigate('register')">สมัครสมาชิก</button>`;
  }
}
function closeSidebarMobile(){ $("#sidebar").classList.remove("open"); $("#sidebarBackdrop").classList.remove("show"); }

async function renderShell(){
  const def = ROUTES[state.route] || ROUTES.dashboard;
  $("#pageTitle").textContent = def.title;
  $("#pageEyebrow").textContent = def.eyebrow;
  renderSidebar();
  renderTopbarActions();
  const viewEl = $("#view");
  viewEl.innerHTML = `<div style="display:flex;justify-content:center;padding:60px;"><div class="loader"></div></div>`;
  try{
    await def.render(viewEl);
  }catch(err){
    console.error(err);
    viewEl.innerHTML = `<div class="card card-pad"><b style="color:var(--wine)">เกิดข้อผิดพลาด:</b> ${esc(err.message||String(err))}</div>`;
  }
}

/* ======================================================================
   VIEW: DASHBOARD  (public)
   ====================================================================== */
async function viewDashboard(root){
  const statsSnap = await db.collection("meta").doc("stats").get();
  const stats = statsSnap.exists ? statsSnap.data() : {};
  await loadDependents().catch(()=>{ state.dependents = state.dependents||[]; });
  await loadCgs().catch(()=>{ state.cgs = state.cgs||[]; });

  const ym = curYm();
  const totalDep = state.dependents.length;
  const byGroupCount = {1:0,2:0,3:0};
  state.dependents.forEach(d=> byGroupCount[d.group] = (byGroupCount[d.group]||0)+1 );
  const visitsThisMonth = stats[`visits_${ym}`] || 0;
  const totalVisits = stats.totalVisits || 0;
  const totalCg = state.cgs.length;

  root.innerHTML = `
    <div class="hero">
      <div class="eyebrow">${esc(ORG_LINE1)}</div>
      <h1>ระบบติดตามงานเยี่ยมบ้านผู้มีภาวะพึ่งพิง</h1>
      <p>แดชบอร์ดนี้แสดงภาพรวมจำนวนการส่งรายงานและการออกเยี่ยมบ้านของอาสาสมัคร CG ทุกคน — เปิดให้ทุกคนในชุมชนติดตามความคืบหน้าได้อย่างโปร่งใส</p>
    </div>

    <div class="stat-grid">
      <div class="stat-card"><div class="num">${totalDep}</div><div class="lbl">ผู้มีภาวะพึ่งพิงทั้งหมด</div></div>
      <div class="stat-card green"><div class="num">${totalCg}</div><div class="lbl">อาสาสมัคร CG ทั้งหมด</div></div>
      <div class="stat-card"><div class="num">${visitsThisMonth}</div><div class="lbl">การเยี่ยมบ้านเดือนนี้ (${fmtMonthLabel(ym)})</div></div>
      <div class="stat-card wine"><div class="num">${totalVisits}</div><div class="lbl">การเยี่ยมบ้านสะสมทั้งหมด</div></div>
    </div>

    <div class="card card-pad">
      <div class="section-heading" style="margin-top:0;">
        <h2>สัดส่วนผู้มีภาวะพึ่งพิงตาม Care Plan</h2>
      </div>
      ${[1,2,3].map(g=>{
        const info = GROUP_INFO[g];
        const count = byGroupCount[g]||0;
        const pct = totalDep? Math.round(count/totalDep*100):0;
        return `<div class="progress-row">
          <div class="name"><span class="badge ${info.badge}">${info.label}</span></div>
          <div class="progress-track"><div class="progress-fill" style="width:${pct}%;"></div></div>
          <div class="progress-count">${count} คน</div>
        </div>`;
      }).join("")}
    </div>

    <div class="section-heading"><h2>ความคืบหน้าการเยี่ยมบ้านเดือนนี้ต่อผู้มีภาวะพึ่งพิง</h2><span class="hint">${fmtMonthLabel(ym)}</span></div>
    <div class="card card-pad" id="dashProgressCard">
      <div style="text-align:center;color:var(--muted);padding:20px;">กำลังคำนวณ...</div>
    </div>
  `;
  renderDashboardProgress();
}

async function renderDashboardProgress(){
  const el = $("#dashProgressCard");
  if(!el) return;
  const ym = curYm();
  const start = ym+"-01", end = ym+"-31";
  let visits = [];
  try{
    const snap = await db.collection("visits").where("visitDate",">=",start).where("visitDate","<=",end).get();
    visits = snap.docs.map(d=>d.data());
  }catch(e){ /* likely not logged in / restricted read - okay for public dashboard */ }
  const countByDep = {};
  visits.forEach(v=> countByDep[v.dependentId] = (countByDep[v.dependentId]||0)+1 );

  if(!state.dependents.length){
    el.innerHTML = `<div class="empty-state"><div class="ic">📋</div>ยังไม่มีข้อมูลผู้มีภาวะพึ่งพิง</div>`;
    return;
  }
  el.innerHTML = state.dependents.map(d=>{
    const target = (GROUP_INFO[d.group]||{}).target || 1;
    const c = countByDep[d.id]||0;
    const pct = Math.min(100, Math.round(c/target*100));
    return `<div class="progress-row">
      <div class="name">${esc(d.fullName)} <span class="badge ${GROUP_INFO[d.group]?.badge||''}" style="margin-left:4px;">กลุ่ม ${esc(d.group)}</span></div>
      <div class="meta">หมู่ ${esc(d.moo||'-')}</div>
      <div class="progress-track"><div class="progress-fill ${c<target?'under':''}" style="width:${pct}%;"></div></div>
      <div class="progress-count">${c}/${target} ครั้ง</div>
    </div>`;
  }).join("");
}

/* ======================================================================
   VIEW: LOGIN / REGISTER
   ====================================================================== */
function viewLogin(root){
  root.innerHTML = `
    <div style="display:flex;justify-content:center;padding-top:20px;">
      <div class="card card-pad auth-card">
        <div class="emblem">🏡</div>
        <h2 style="margin:10px 0 4px;">เข้าสู่ระบบ</h2>
        <p style="color:var(--muted);font-size:14px;margin-top:0;">สำหรับ CG / CM / ผู้ดูแลระบบ</p>
        <form id="loginForm">
          <div class="field" style="margin-bottom:14px;">
            <label>ชื่อผู้ใช้ <span class="req">*</span></label>
            <input type="text" id="li_username" required autocomplete="username">
          </div>
          <div class="field" style="margin-bottom:18px;">
            <label>รหัสผ่าน <span class="req">*</span></label>
            <input type="password" id="li_password" required autocomplete="current-password">
          </div>
          <button class="btn btn-primary" style="width:100%;justify-content:center;" type="submit">เข้าสู่ระบบ</button>
        </form>
        <div style="text-align:center;margin-top:16px;">
          <button class="link-btn" onclick="navigate('register')">ยังไม่มีบัญชี? สมัครสมาชิก</button>
        </div>
      </div>
    </div>`;
  $("#loginForm").addEventListener("submit", async e=>{
    e.preventDefault();
    const btn = e.target.querySelector("button");
    btn.disabled = true; btn.textContent = "กำลังเข้าสู่ระบบ...";
    try{
      await doLogin($("#li_username").value, $("#li_password").value);
      toast("เข้าสู่ระบบสำเร็จ","ok");
      navigate("dashboard");
    }catch(err){
      toast(err.message || "เข้าสู่ระบบไม่สำเร็จ", "err");
      btn.disabled=false; btn.textContent="เข้าสู่ระบบ";
    }
  });
}

function viewRegister(root){
  root.innerHTML = `
    <div style="display:flex;justify-content:center;padding-top:20px;">
      <div class="card card-pad auth-card">
        <div class="emblem">🌿</div>
        <h2 style="margin:10px 0 4px;">สมัครสมาชิก</h2>
        <p style="color:var(--muted);font-size:14px;margin-top:0;">บัญชีของคุณจะต้องรอผู้ดูแลระบบอนุมัติก่อนใช้งาน</p>
        <form id="regForm">
          <div class="field" style="margin-bottom:14px;">
            <label>ชื่อ-สกุล <span class="req">*</span></label>
            <input type="text" id="rg_fullname" required>
          </div>
          <div class="field" style="margin-bottom:14px;">
            <label>สิทธิ์การใช้งาน <span class="req">*</span></label>
            <select id="rg_role" required>
              <option value="CG">CG (อาสาสมัครผู้เยี่ยมบ้าน)</option>
              <option value="CM">CM (ผู้จัดการรายกรณี)</option>
            </select>
          </div>
          <div class="field" style="margin-bottom:14px;">
            <label>ชื่อผู้ใช้ <span class="req">*</span></label>
            <input type="text" id="rg_username" required placeholder="ห้ามใช้ admin">
          </div>
          <div class="field" style="margin-bottom:18px;">
            <label>รหัสผ่าน <span class="req">*</span></label>
            <input type="password" id="rg_password" required minlength="6">
          </div>
          <button class="btn btn-gold" style="width:100%;justify-content:center;" type="submit">สมัครสมาชิก</button>
        </form>
        <div style="text-align:center;margin-top:16px;">
          <button class="link-btn" onclick="navigate('login')">มีบัญชีแล้ว? เข้าสู่ระบบ</button>
        </div>
      </div>
    </div>`;
  $("#regForm").addEventListener("submit", async e=>{
    e.preventDefault();
    const btn = e.target.querySelector("button");
    btn.disabled = true; btn.textContent="กำลังสมัคร...";
    try{
      const data = {
        fullName: $("#rg_fullname").value,
        role: $("#rg_role").value,
        username: $("#rg_username").value,
        password: $("#rg_password").value
      };
      const profile = await doRegister(data);
      if(profile.status === "approved"){
        toast("สร้างบัญชีผู้ดูแลระบบสำเร็จ กรุณาเข้าสู่ระบบ","ok");
      } else {
        toast("สมัครสมาชิกสำเร็จ กรุณารอการอนุมัติจากผู้ดูแลระบบ","ok");
      }
      navigate("login");
    }catch(err){
      let msg = err.message || "สมัครสมาชิกไม่สำเร็จ";
      if(err.code === "auth/email-already-in-use") msg = "ชื่อผู้ใช้นี้ถูกใช้แล้ว";
      if(err.code === "auth/weak-password") msg = "รหัสผ่านต้องมีอย่างน้อย 6 ตัวอักษร";
      toast(msg,"err");
      btn.disabled=false; btn.textContent="สมัครสมาชิก";
    }
  });
}

/* ======================================================================
   VIEW: ส่วนที่ 2 — ส่งรายงานการเยี่ยมบ้าน
   ====================================================================== */
async function viewReport(root){
  await loadCgs(); await loadDependents(); await resolveMyCg();
  const isCG = state.user.role === "CG";

  let myDependents = state.dependents;
  if(isCG){
    if(!state.myCg){
      root.innerHTML = `<div class="card card-pad"><div class="empty-state"><div class="ic">⚠️</div>
        บัญชีของคุณยังไม่ถูกเชื่อมโยงกับข้อมูล CG กรุณาแจ้ง CM/Admin ให้เพิ่มชื่อผู้ใช้ <b>${esc(state.user.username)}</b> ในข้อมูล CG (ส่วนจัดการข้อมูล CG)</div></div>`;
      return;
    }
    myDependents = state.dependents.filter(d=>d.cgId === state.myCg.id);
  }

  root.innerHTML = `
    ${isCG ? `
    <div class="card card-pad" style="margin-bottom:24px;">
      <div class="section-heading" style="margin-top:0;"><h2>บันทึกการเยี่ยมบ้านใหม่</h2></div>
      <form id="visitForm">
        <div class="form-grid">
          <div class="field"><label>ชื่อ CG</label><input type="text" value="${esc(state.myCg.fullName)}" disabled></div>
          <div class="field"><label>ผู้มีภาวะพึ่งพิง <span class="req">*</span></label>
            <select id="v_dep" required>
              <option value="">-- เลือก --</option>
              ${myDependents.map(d=>`<option value="${d.id}">${esc(d.fullName)} (กลุ่ม ${esc(d.group)})</option>`).join("")}
            </select>
          </div>
          <div class="field"><label>หมู่</label><input type="text" id="v_moo" disabled></div>
          <div class="field"><label>ชื่อบ้าน</label><input type="text" id="v_house" disabled></div>
          <div class="field"><label>วันที่เยี่ยม <span class="req">*</span></label><input type="date" id="v_date" required value="${todayStr()}"></div>
          <div class="field"><label>รูปการเยี่ยม (1 รูป) <span class="req">*</span></label><input type="file" id="v_photo" accept="image/*" required></div>
        </div>
        <div id="v_photoPreviewWrap"></div>
        <div id="v_adlWrap" style="margin-top:10px;"></div>
        <div id="v_actWrap" style="margin-top:10px;"></div>
        <div class="field" style="margin-top:14px;">
          <label>บันทึกเพิ่มเติม</label>
          <textarea id="v_notes" placeholder="รายละเอียดการเยี่ยม อาการ ข้อสังเกต ฯลฯ"></textarea>
        </div>
        <div style="margin-top:18px;"><button class="btn btn-primary" type="submit">บันทึกรายงานการเยี่ยม</button></div>
      </form>
    </div>` : ``}

    <div class="section-heading"><h2>ประวัติการเยี่ยมบ้าน</h2></div>
    <div class="card card-pad">
      <div style="display:flex;gap:10px;flex-wrap:wrap;margin-bottom:14px;">
        ${!isCG ? `<select id="f_cg" class="field-inline">
          <option value="">-- ทุก CG --</option>
          ${state.cgs.map(c=>`<option value="${c.id}">${esc(c.fullName)}</option>`).join("")}
        </select>` : ``}
        <input type="month" id="f_month" value="${curYm()}">
        <button class="btn btn-outline btn-sm" onclick="loadVisitHistory()">กรองข้อมูล</button>
      </div>
      <div id="visitHistoryTable"></div>
    </div>
  `;

  if(isCG){
    const depSel = $("#v_dep");
    const adlWrap = $("#v_adlWrap");
    const actWrap = $("#v_actWrap");
    let adlState = {};
    depSel.addEventListener("change", ()=>{
      const dep = myDependents.find(d=>d.id===depSel.value);
      $("#v_moo").value = dep? (dep.moo||"") : "";
      $("#v_house").value = dep? (dep.houseName||"") : "";
      adlState = {};
      if(dep && dep.group === "3"){
        adlWrap.innerHTML = renderAdlForm("v_adl", true);
        actWrap.innerHTML = `<div class="field"><label>กิจกรรมที่ทำ (เลือกอย่างน้อย 1) <span class="req">*</span></label>
          ${ACTIVITIES.map((a,i)=>`<div class="checkline"><input type="checkbox" name="v_act" value="${i}" id="act${i}"><label for="act${i}" style="font-weight:400;">${esc(a)}</label></div>`).join("")}
        </div>`;
        bindAdlForm("v_adl");
      } else if(dep){
        adlWrap.innerHTML = `<details><summary style="cursor:pointer;font-weight:600;color:var(--primary);padding:8px 0;">ประเมิน ADL (ถ้ามี)</summary>${renderAdlForm("v_adl", false)}</details>`;
        actWrap.innerHTML = `<details><summary style="cursor:pointer;font-weight:600;color:var(--primary);padding:8px 0;">กิจกรรมที่ทำ (ถ้ามี)</summary>
          ${ACTIVITIES.map((a,i)=>`<div class="checkline"><input type="checkbox" name="v_act" value="${i}" id="act${i}"><label for="act${i}" style="font-weight:400;">${esc(a)}</label></div>`).join("")}
        </details>`;
        bindAdlForm("v_adl");
      } else {
        adlWrap.innerHTML = ""; actWrap.innerHTML = "";
      }
    });

    $("#v_photo").addEventListener("change", async e=>{
      const f = e.target.files[0];
      if(!f) return;
      const dataUrl = await compressImage(f, 900);
      $("#v_photoPreviewWrap").innerHTML = `<img src="${dataUrl}" class="photo-preview" style="margin-top:10px;">`;
      $("#v_photo").dataset.compressed = dataUrl;
    });

    $("#visitForm").addEventListener("submit", async e=>{
      e.preventDefault();
      const dep = myDependents.find(d=>d.id===depSel.value);
      if(!dep){ toast("กรุณาเลือกผู้มีภาวะพึ่งพิง","err"); return; }
      const photo = $("#v_photo").dataset.compressed;
      if(!photo){ toast("กรุณาแนบรูปการเยี่ยม","err"); return; }
      const activities = $all('input[name="v_act"]:checked').map(c=>Number(c.value));
      let adl = collectAdlForm("v_adl");
      if(dep.group === "3"){
        if(activities.length===0){ toast("กรุณาเลือกกิจกรรมอย่างน้อย 1 รายการ (กลุ่ม 3)","err"); return; }
        if(!adl){ toast("กรุณาประเมิน ADL ให้ครบทุกข้อ (บังคับสำหรับกลุ่ม 3)","err"); return; }
      }
      const btn = e.target.querySelector('button[type=submit]');
      btn.disabled = true; btn.textContent = "กำลังอัปโหลดรูป...";
      try{
        const visitDate = $("#v_date").value;
        const photoUrl = await uploadToImgbb(photo);
        btn.textContent = "กำลังบันทึก...";
        await db.collection("visits").add({
          dependentId: dep.id, dependentName: dep.fullName, group: dep.group,
          cgId: state.myCg.id, cgUsername: state.user.username, cgName: state.myCg.fullName,
          moo: dep.moo||"", houseName: dep.houseName||"",
          visitDate, photo: photoUrl, adl: adl||null, activities: activities.map(i=>ACTIVITIES[i]),
          notes: $("#v_notes").value.trim(),
          createdAt: firebase.firestore.FieldValue.serverTimestamp()
        });
        await bumpMonthlyStat(ymOf(visitDate), dep.group);
        toast("บันทึกรายงานการเยี่ยมสำเร็จ","ok");
        e.target.reset();
        $("#v_photoPreviewWrap").innerHTML=""; adlWrap.innerHTML=""; actWrap.innerHTML="";
        loadVisitHistory();
      }catch(err){
        toast(err.message,"err");
      }finally{
        btn.disabled=false; btn.textContent="บันทึกรายงานการเยี่ยม";
      }
    });
  }

  window.loadVisitHistory = async function(){
    const box = $("#visitHistoryTable");
    box.innerHTML = `<div style="text-align:center;padding:20px;"><div class="loader" style="margin:0 auto;"></div></div>`;
    let q = db.collection("visits");
    const cgFilterId = isCG ? state.myCg.id : ($("#f_cg")?$("#f_cg").value:"");
    if(cgFilterId) q = q.where("cgId","==",cgFilterId);
    const month = $("#f_month") ? $("#f_month").value : curYm();
    if(month) q = q.where("visitDate",">=",month+"-01").where("visitDate","<=",month+"-31");
    q = q.orderBy("visitDate","desc").limit(200);
    const snap = await q.get();
    const rows = snap.docs.map(d=>({id:d.id,...d.data()}));
    if(!rows.length){ box.innerHTML = `<div class="empty-state"><div class="ic">📭</div>ไม่พบข้อมูลการเยี่ยมในช่วงที่เลือก</div>`; return; }
    box.innerHTML = `<div class="table-wrap"><table class="data"><thead><tr>
      <th>วันที่</th><th>ผู้มีภาวะพึ่งพิง</th><th>กลุ่ม</th><th>CG</th><th>หมู่/บ้าน</th><th>ADL</th><th>รูป</th>
      </tr></thead><tbody>
      ${rows.map(v=>`<tr>
        <td>${fmtDate(v.visitDate)}</td>
        <td>${esc(v.dependentName)}</td>
        <td><span class="badge ${GROUP_INFO[v.group]?.badge||''}">กลุ่ม ${esc(v.group)}</span></td>
        <td>${esc(v.cgName)}</td>
        <td>หมู่ ${esc(v.moo||'-')} / ${esc(v.houseName||'-')}</td>
        <td>${v.adl? v.adl.total+"/20" : "-"}</td>
        <td>${v.photo?`<img src="${v.photo}" class="avatar" style="border-radius:6px;">`:"-"}</td>
      </tr>`).join("")}
      </tbody></table></div>`;
  };
  loadVisitHistory();
}

function renderAdlForm(prefix, required){
  return `<div class="card" style="background:var(--surface-soft);padding:16px 18px;border-radius:var(--radius-md);margin-top:6px;">
    <div style="font-weight:700;color:var(--primary-dark);margin-bottom:4px;">แบบประเมิน ADL (Barthel Index)</div>
    ${ADL_ITEMS.map(item=>`
      <div class="adl-item">
        <div class="q">${esc(item.q)}</div>
        <div class="adl-opts" data-key="${item.key}" id="${prefix}_${item.key}">
          ${item.opts.map(([score,label])=>`<div class="adl-opt" data-score="${score}">${score} - ${esc(label)}</div>`).join("")}
        </div>
      </div>
    `).join("")}
    <div class="adl-total" id="${prefix}_total">คะแนนรวม: 0 / 20</div>
  </div>`;
}
function bindAdlForm(prefix){
  ADL_ITEMS.forEach(item=>{
    const wrap = $(`#${prefix}_${item.key}`);
    if(!wrap) return;
    $all(".adl-opt", wrap).forEach(opt=>{
      opt.addEventListener("click", ()=>{
        $all(".adl-opt", wrap).forEach(o=>o.classList.remove("sel"));
        opt.classList.add("sel");
        updateAdlTotal(prefix);
      });
    });
  });
}
function updateAdlTotal(prefix){
  let total = 0, answered = 0;
  ADL_ITEMS.forEach(item=>{
    const wrap = $(`#${prefix}_${item.key}`);
    const sel = wrap ? wrap.querySelector(".adl-opt.sel") : null;
    if(sel){ total += Number(sel.dataset.score); answered++; }
  });
  const totalEl = $(`#${prefix}_total`);
  if(totalEl) totalEl.textContent = `คะแนนรวม: ${total} / 20 (ตอบแล้ว ${answered}/${ADL_ITEMS.length} ข้อ)`;
  return {total, answered};
}
function collectAdlForm(prefix){
  const details = {};
  let total = 0, answered = 0;
  ADL_ITEMS.forEach(item=>{
    const wrap = $(`#${prefix}_${item.key}`);
    const sel = wrap ? wrap.querySelector(".adl-opt.sel") : null;
    if(sel){ details[item.key] = Number(sel.dataset.score); total += Number(sel.dataset.score); answered++; }
  });
  if(answered === 0) return null;
  return { total, answered, details, date: todayStr() };
}

/* ======================================================================
   VIEW: ส่วนที่ 3 — จัดการข้อมูล CG (CM/admin)
   ====================================================================== */
async function viewCgs(root){
  await loadCgs();
  root.innerHTML = `
    <div class="section-heading" style="margin-top:0;">
      <h2>รายชื่อ CG (${state.cgs.length})</h2>
      <button class="btn btn-gold btn-sm" onclick="openCgModal()">+ เพิ่ม CG</button>
    </div>
    <div class="card card-pad">
      ${state.cgs.length ? `<div class="table-wrap"><table class="data"><thead><tr>
        <th></th><th>ชื่อ-สกุล</th><th>เบอร์โทร</th><th>Username เชื่อมโยง</th><th>ที่อยู่</th><th></th>
        </tr></thead><tbody>
        ${state.cgs.map(c=>`<tr>
          <td>${c.photo?`<img src="${c.photo}" class="avatar">`:`<div class="avatar" style="display:flex;align-items:center;justify-content:center;">👤</div>`}</td>
          <td><b>${esc(c.fullName)}</b><div style="font-size:12px;color:var(--muted);">${esc(c.nationalId||'')}</div></td>
          <td>${esc(c.phone||'-')}</td>
          <td>${c.linkedUsername?`<span class="badge badge-approved">@${esc(c.linkedUsername)}</span>`:`<span class="badge badge-pending">ยังไม่เชื่อมโยง</span>`}</td>
          <td>${esc(c.address||'-')}</td>
          <td style="white-space:nowrap;">
            <button class="btn btn-outline btn-sm" onclick='openCgModal(${JSON.stringify(c).replace(/'/g,"&#39;")})'>แก้ไข</button>
            <button class="btn btn-danger btn-sm" onclick="deleteCg('${c.id}')">ลบ</button>
          </td>
        </tr>`).join("")}
        </tbody></table></div>` : `<div class="empty-state"><div class="ic">👥</div>ยังไม่มีข้อมูล CG — เริ่มเพิ่มข้อมูลได้เลย</div>`}
    </div>
  `;
}
function openCgModal(cg){
  cg = cg || {};
  const html = `
    <div class="modal-backdrop" onclick="if(event.target===this)closeModal()">
      <div class="modal">
        <h3>${cg.id?"แก้ไขข้อมูล CG":"เพิ่ม CG ใหม่"}</h3>
        <form id="cgForm">
          <div class="field" style="margin-bottom:12px;"><label>รูปภาพ CG</label>
            <input type="file" id="cg_photo" accept="image/*">
            <img id="cg_photoPrev" class="photo-preview" style="margin-top:8px;${cg.photo?'':'display:none;'}" src="${cg.photo||''}">
          </div>
          <div class="field" style="margin-bottom:12px;"><label>ชื่อ-สกุล <span class="req">*</span></label>
            <input type="text" id="cg_name" required value="${esc(cg.fullName||'')}"></div>
          <div class="form-grid" style="margin-bottom:12px;">
            <div class="field"><label>วันเดือนปีเกิด</label><input type="date" id="cg_dob" value="${esc(cg.birthDate||'')}"></div>
            <div class="field"><label>เลขบัตรประชาชน</label><input type="text" id="cg_nid" value="${esc(cg.nationalId||'')}" maxlength="13"></div>
          </div>
          <div class="field" style="margin-bottom:12px;"><label>ที่อยู่</label><textarea id="cg_addr">${esc(cg.address||'')}</textarea></div>
          <div class="form-grid" style="margin-bottom:12px;">
            <div class="field"><label>เบอร์โทร</label><input type="tel" id="cg_phone" value="${esc(cg.phone||'')}"></div>
            <div class="field"><label>Username เชื่อมโยงบัญชีเข้าระบบ</label><input type="text" id="cg_link" value="${esc(cg.linkedUsername||'')}" placeholder="ต้องตรงกับ username ที่ CG ใช้สมัคร">
              <div class="helptext">ใช้จับคู่บัญชี login ของ CG กับข้อมูลนี้ เพื่อให้ CG เห็นผู้ป่วยของตัวเองตอนส่งรายงาน</div>
            </div>
          </div>
          <div style="display:flex;gap:10px;margin-top:16px;">
            <button class="btn btn-primary" type="submit">บันทึก</button>
            <button class="btn btn-ghost" type="button" onclick="closeModal()">ยกเลิก</button>
          </div>
        </form>
      </div>
    </div>`;
  $("#modalRoot").innerHTML = html;
  let photoData = cg.photo || null;
  $("#cg_photo").addEventListener("change", async e=>{
    const f = e.target.files[0]; if(!f) return;
    photoData = await compressImage(f, 500);
    $("#cg_photoPrev").src = photoData; $("#cg_photoPrev").style.display="block";
  });
  $("#cgForm").addEventListener("submit", async e=>{
    e.preventDefault();
    const btn = e.target.querySelector('button[type=submit]');
    btn.disabled = true; btn.textContent = "กำลังอัปโหลดรูป...";
    try{
      const photoUrl = await uploadToImgbb(photoData);
      btn.textContent = "กำลังบันทึก...";
      const payload = {
        fullName: $("#cg_name").value.trim(),
        birthDate: $("#cg_dob").value,
        nationalId: $("#cg_nid").value.trim(),
        address: $("#cg_addr").value.trim(),
        phone: $("#cg_phone").value.trim(),
        linkedUsername: $("#cg_link").value.trim().toLowerCase(),
        photo: photoUrl
      };
      if(cg.id){ await db.collection("cgs").doc(cg.id).update(payload); toast("แก้ไขข้อมูล CG สำเร็จ","ok"); }
      else { payload.createdAt = firebase.firestore.FieldValue.serverTimestamp(); await db.collection("cgs").add(payload); await bumpStats({totalCg:1}); toast("เพิ่ม CG สำเร็จ","ok"); }
      closeModal();
      renderShell();
    }catch(err){
      toast(err.message,"err");
      btn.disabled=false; btn.textContent="บันทึก";
    }
  });
}
async function deleteCg(id){
  if(!confirm("ยืนยันการลบข้อมูล CG นี้?")) return;
  await db.collection("cgs").doc(id).delete();
  await bumpStats({totalCg:-1});
  toast("ลบข้อมูลแล้ว","ok");
  renderShell();
}
function closeModal(){ $("#modalRoot").innerHTML = ""; }

/* ======================================================================
   VIEW: ส่วนที่ 4 — จัดการข้อมูลผู้มีภาวะพึ่งพิง
   ====================================================================== */
async function viewDependents(root){
  await loadCgs(); await loadDependents(); await resolveMyCg();
  const canEdit = state.user.role === "CM" || state.user.role === "admin";
  let list = state.dependents;
  if(state.user.role === "CG"){
    list = state.myCg ? state.dependents.filter(d=>d.cgId===state.myCg.id) : [];
  }
  root.innerHTML = `
    <div class="section-heading" style="margin-top:0;">
      <h2>ผู้มีภาวะพึ่งพิง (${list.length})</h2>
      ${canEdit?`<button class="btn btn-gold btn-sm" onclick="openDepModal()">+ เพิ่มผู้มีภาวะพึ่งพิง</button>`:''}
    </div>
    <div class="card card-pad">
      ${list.length? `<div class="table-wrap"><table class="data"><thead><tr>
        <th></th><th>ชื่อ-สกุล</th><th>กลุ่ม</th><th>หมู่/บ้าน</th><th>CG ผู้ดูแล</th><th>ADL ล่าสุด</th><th></th>
      </tr></thead><tbody>
        ${list.map(d=>`<tr>
          <td>${d.photo?`<img src="${d.photo}" class="avatar">`:`<div class="avatar" style="display:flex;align-items:center;justify-content:center;">👤</div>`}</td>
          <td><b>${esc(d.fullName)}</b><div style="font-size:12px;color:var(--muted);">${esc(d.chronicDisease||'-')}</div></td>
          <td><span class="badge ${GROUP_INFO[d.group]?.badge||''}">กลุ่ม ${esc(d.group)}</span></td>
          <td>หมู่ ${esc(d.moo||'-')} / ${esc(d.houseName||'-')}</td>
          <td>${esc((state.cgs.find(c=>c.id===d.cgId)||{}).fullName || '-')}</td>
          <td>${d.adlBaseline? d.adlBaseline.total+"/20" : "-"}</td>
          <td style="white-space:nowrap;">
            <button class="btn btn-outline btn-sm" onclick="viewDepDetail('${d.id}')">ดูข้อมูล</button>
            ${canEdit?`<button class="btn btn-outline btn-sm" onclick='openDepModal(${JSON.stringify(d).replace(/'/g,"&#39;")})'>แก้ไข</button>
            <button class="btn btn-danger btn-sm" onclick="deleteDep('${d.id}')">ลบ</button>`:''}
          </td>
        </tr>`).join("")}
      </tbody></table></div>` : `<div class="empty-state"><div class="ic">🧑‍🦽</div>ยังไม่มีข้อมูลผู้มีภาวะพึ่งพิง</div>`}
    </div>
  `;
}
function viewDepDetail(id){
  const d = state.dependents.find(x=>x.id===id);
  if(!d) return;
  const cg = state.cgs.find(c=>c.id===d.cgId);
  $("#modalRoot").innerHTML = `<div class="modal-backdrop" onclick="if(event.target===this)closeModal()">
    <div class="modal wide">
      <h3>${esc(d.fullName)}</h3>
      <div style="display:flex;gap:16px;flex-wrap:wrap;margin-bottom:16px;">
        ${d.photo?`<img src="${d.photo}" class="avatar-lg">`:''}
        ${d.housePhoto?`<img src="${d.housePhoto}" class="avatar-lg">`:''}
      </div>
      <div class="form-grid">
        <div><b>กลุ่ม Care Plan:</b> <span class="badge ${GROUP_INFO[d.group]?.badge||''}">${GROUP_INFO[d.group]?.label||''}</span></div>
        <div><b>วันเกิด:</b> ${fmtDate(d.birthDate)}</div>
        <div><b>เลขบัตรประชาชน:</b> ${esc(d.nationalId||'-')}</div>
        <div><b>เบอร์โทร:</b> ${esc(d.phone||'-')}</div>
        <div><b>ที่อยู่:</b> ${esc(d.address||'-')}</div>
        <div><b>หมู่/บ้าน:</b> หมู่ ${esc(d.moo||'-')} / ${esc(d.houseName||'-')}</div>
        <div><b>โรคประจำตัว:</b> ${esc(d.chronicDisease||'-')}</div>
        <div><b>CG ผู้ดูแล:</b> ${esc(cg?cg.fullName:'-')}</div>
      </div>
      <hr class="divider">
      <b>ผล ADL ก่อนดูแล (Baseline):</b> ${d.adlBaseline? `${d.adlBaseline.total}/20 คะแนน (ประเมินเมื่อ ${fmtDate(d.adlBaseline.date)})` : 'ยังไม่ได้ประเมิน'}
      <div style="margin-top:18px;text-align:right;"><button class="btn btn-outline" onclick="closeModal()">ปิด</button></div>
    </div>
  </div>`;
}
function openDepModal(d){
  d = d || {};
  const modalHtml = `
    <div class="modal-backdrop" onclick="if(event.target===this)closeModal()">
      <div class="modal wide">
        <h3>${d.id?"แก้ไขข้อมูลผู้มีภาวะพึ่งพิง":"เพิ่มผู้มีภาวะพึ่งพิง"}</h3>
        <form id="depForm">
          <div class="form-grid" style="margin-bottom:12px;">
            <div class="field"><label>รูปผู้มีภาวะพึ่งพิง</label><input type="file" id="d_photo" accept="image/*">
              <img id="d_photoPrev" class="photo-preview" style="margin-top:8px;${d.photo?'':'display:none;'}" src="${d.photo||''}"></div>
            <div class="field"><label>รูปบ้าน</label><input type="file" id="d_housePhoto" accept="image/*">
              <img id="d_housePhotoPrev" class="photo-preview" style="margin-top:8px;${d.housePhoto?'':'display:none;'}" src="${d.housePhoto||''}"></div>
          </div>
          <div class="field" style="margin-bottom:12px;"><label>ชื่อ-สกุล <span class="req">*</span></label>
            <input type="text" id="d_name" required value="${esc(d.fullName||'')}"></div>
          <div class="form-grid" style="margin-bottom:12px;">
            <div class="field"><label>วันเดือนปีเกิด</label><input type="date" id="d_dob" value="${esc(d.birthDate||'')}"></div>
            <div class="field"><label>เลขบัตรประชาชน</label><input type="text" id="d_nid" value="${esc(d.nationalId||'')}" maxlength="13"></div>
          </div>
          <div class="field" style="margin-bottom:12px;"><label>ที่อยู่</label><textarea id="d_addr">${esc(d.address||'')}</textarea></div>
          <div class="form-grid" style="margin-bottom:12px;">
            <div class="field"><label>เบอร์โทร</label><input type="tel" id="d_phone" value="${esc(d.phone||'')}"></div>
            <div class="field"><label>โรคประจำตัว</label><input type="text" id="d_disease" value="${esc(d.chronicDisease||'')}"></div>
          </div>
          <div class="form-grid" style="margin-bottom:12px;">
            <div class="field"><label>หมู่ <span class="req">*</span></label><input type="text" id="d_moo" required value="${esc(d.moo||'')}"></div>
            <div class="field"><label>ชื่อบ้าน</label><input type="text" id="d_house" value="${esc(d.houseName||'')}"></div>
          </div>
          <div class="form-grid" style="margin-bottom:12px;">
            <div class="field"><label>กลุ่ม Care Plan <span class="req">*</span></label>
              <select id="d_group" required>
                <option value="">-- เลือก --</option>
                ${[1,2,3].map(g=>`<option value="${g}" ${String(d.group)===String(g)?'selected':''}>${GROUP_INFO[g].label}</option>`).join("")}
              </select>
            </div>
            <div class="field"><label>CG ผู้รับผิดชอบ <span class="req">*</span></label>
              <select id="d_cg" required>
                <option value="">-- เลือก --</option>
                ${state.cgs.map(c=>`<option value="${c.id}" ${d.cgId===c.id?'selected':''}>${esc(c.fullName)}</option>`).join("")}
              </select>
            </div>
          </div>
          <details ${d.adlBaseline?'open':''}>
            <summary style="cursor:pointer;font-weight:700;color:var(--primary);padding:10px 0;">ผลการประเมิน ADL ก่อนดูแล (Baseline)</summary>
            ${renderAdlForm("d_adl", false)}
          </details>
          <div style="display:flex;gap:10px;margin-top:16px;">
            <button class="btn btn-primary" type="submit">บันทึก</button>
            <button class="btn btn-ghost" type="button" onclick="closeModal()">ยกเลิก</button>
          </div>
        </form>
      </div>
    </div>`;
  $("#modalRoot").innerHTML = modalHtml;
  bindAdlForm("d_adl");
  if(d.adlBaseline && d.adlBaseline.details){
    ADL_ITEMS.forEach(item=>{
      const score = d.adlBaseline.details[item.key];
      if(score===undefined) return;
      const wrap = $(`#d_adl_${item.key}`);
      if(!wrap) return;
      const opt = wrap.querySelector(`.adl-opt[data-score="${score}"]`);
      if(opt) opt.classList.add("sel");
    });
    updateAdlTotal("d_adl");
  }
  let photoData = d.photo || null, houseData = d.housePhoto || null;
  $("#d_photo").addEventListener("change", async e=>{
    const f=e.target.files[0]; if(!f) return;
    photoData = await compressImage(f,600);
    $("#d_photoPrev").src=photoData; $("#d_photoPrev").style.display="block";
  });
  $("#d_housePhoto").addEventListener("change", async e=>{
    const f=e.target.files[0]; if(!f) return;
    houseData = await compressImage(f,700);
    $("#d_housePhotoPrev").src=houseData; $("#d_housePhotoPrev").style.display="block";
  });
  $("#depForm").addEventListener("submit", async e=>{
    e.preventDefault();
    const btn = e.target.querySelector('button[type=submit]');
    btn.disabled = true; btn.textContent = "กำลังอัปโหลดรูป...";
    try{
      const adl = collectAdlForm("d_adl");
      const cgObj = state.cgs.find(c=>c.id===$("#d_cg").value);
      const [photoUrl, houseUrl] = await Promise.all([uploadToImgbb(photoData), uploadToImgbb(houseData)]);
      btn.textContent = "กำลังบันทึก...";
      const payload = {
        fullName: $("#d_name").value.trim(),
        birthDate: $("#d_dob").value,
        nationalId: $("#d_nid").value.trim(),
        address: $("#d_addr").value.trim(),
        phone: $("#d_phone").value.trim(),
        chronicDisease: $("#d_disease").value.trim(),
        moo: $("#d_moo").value.trim(),
        houseName: $("#d_house").value.trim(),
        group: $("#d_group").value,
        cgId: $("#d_cg").value,
        cgName: cgObj?cgObj.fullName:"",
        photo: photoUrl,
        housePhoto: houseUrl,
        adlBaseline: adl
      };
      if(d.id){ await db.collection("dependents").doc(d.id).update(payload); toast("แก้ไขข้อมูลสำเร็จ","ok"); }
      else{ payload.createdAt = firebase.firestore.FieldValue.serverTimestamp(); await db.collection("dependents").add(payload); await bumpStats({totalDependents:1}); toast("เพิ่มข้อมูลสำเร็จ","ok"); }
      closeModal(); renderShell();
    }catch(err){
      toast(err.message,"err");
      btn.disabled=false; btn.textContent="บันทึก";
    }
  });
}
async function deleteDep(id){
  if(!confirm("ยืนยันการลบข้อมูลนี้?")) return;
  await db.collection("dependents").doc(id).delete();
  await bumpStats({totalDependents:-1});
  toast("ลบข้อมูลแล้ว","ok");
  renderShell();
}

/* ======================================================================
   VIEW: ส่วนที่ 5 — ออกรายงาน PDF
   ====================================================================== */
async function viewReportsExport(root){
  await loadCgs(); await loadDependents(); await resolveMyCg();
  const isCG = state.user.role === "CG";
  const cgOptions = isCG ? (state.myCg?[state.myCg]:[]) : state.cgs;

  root.innerHTML = `
    <div class="tabs">
      <button class="tab active" data-tab="t1">5.1 รายงานการเยี่ยมบ้านรายเดือน</button>
      <button class="tab" data-tab="t2">5.2 รายงานข้อมูลผู้มีภาวะพึ่งพิง</button>
      <button class="tab" data-tab="t3">5.3 สรุปผลการดำเนินงาน</button>
    </div>

    <div id="tab_t1" class="card card-pad">
      <div class="form-grid">
        <div class="field"><label>เลือก CG</label>
          <select id="r1_cg">${cgOptions.map(c=>`<option value="${c.id}">${esc(c.fullName)}</option>`).join("")}</select></div>
        <div class="field"><label>เดือน</label><input type="month" id="r1_month" value="${curYm()}"></div>
        <div class="field"><label>ผู้มีภาวะพึ่งพิง</label><select id="r1_dep"><option value="">-- ทั้งหมดของ CG นี้ --</option></select></div>
      </div>
      <button class="btn btn-primary" style="margin-top:14px;" onclick="exportVisitReport()">${iconSvg('export')} ส่งออก PDF</button>
    </div>

    <div id="tab_t2" class="card card-pad" style="display:none;">
      <div class="field" style="max-width:420px;"><label>เลือกผู้มีภาวะพึ่งพิง</label>
        <select id="r2_dep" multiple size="8">${state.dependents.map(d=>`<option value="${d.id}">${esc(d.fullName)}</option>`).join("")}</select>
        <div class="helptext">กด Ctrl/Cmd ค้างเพื่อเลือกหลายคน หรือไม่เลือกเลยเพื่อออกรายงานทุกคน</div>
      </div>
      <button class="btn btn-primary" style="margin-top:14px;" onclick="exportProfileReport()">${iconSvg('export')} ส่งออก PDF</button>
    </div>

    <div id="tab_t3" class="card card-pad" style="display:none;">
      <div class="field" style="max-width:420px;"><label>เลือกผู้มีภาวะพึ่งพิง</label>
        <select id="r3_dep" multiple size="8">${state.dependents.map(d=>`<option value="${d.id}">${esc(d.fullName)}</option>`).join("")}</select>
        <div class="helptext">1 ผู้มีภาวะพึ่งพิง ต่อ 1 แผ่น — เปรียบเทียบคะแนน ADL รายเดือน</div>
      </div>
      <button class="btn btn-primary" style="margin-top:14px;" onclick="exportSummaryReport()">${iconSvg('export')} ส่งออก PDF</button>
    </div>
  `;

  $all(".tab").forEach(tab=>{
    tab.addEventListener("click", ()=>{
      $all(".tab").forEach(t=>t.classList.remove("active"));
      tab.classList.add("active");
      ["t1","t2","t3"].forEach(id=> $(`#tab_${id}`).style.display = (id===tab.dataset.tab?'block':'none'));
    });
  });

  function refreshR1Dep(){
    const cgId = $("#r1_cg").value;
    const deps = state.dependents.filter(d=>d.cgId===cgId);
    $("#r1_dep").innerHTML = `<option value="">-- ทั้งหมดของ CG นี้ --</option>` + deps.map(d=>`<option value="${d.id}">${esc(d.fullName)}</option>`).join("");
  }
  if($("#r1_cg")){ $("#r1_cg").addEventListener("change", refreshR1Dep); refreshR1Dep(); }
}

function reportHeader(sub){
  return `<div class="rp-header">
    <div class="org">รายงานอย่างเป็นทางการ</div>
    <h2>${esc(REPORT_TITLE)}</h2>
    <div class="sub">${esc(sub||"")}</div>
  </div>`;
}
function reportSignature(){
  return `<div class="rp-signature"><div><div>ลงชื่อ ....................................................</div><div class="line">( ผู้บันทึกรายงาน / CG )</div></div></div>`;
}
async function exportPdf(containerId, filename){
  toast("กำลังสร้างไฟล์ PDF ...");
  const el = document.getElementById(containerId);
  const opt = {
    margin: 0, filename: filename,
    image: { type:"jpeg", quality:0.95 },
    html2canvas: { scale:2, useCORS:true },
    jsPDF: { unit:"mm", format:"a4", orientation:"portrait" },
    pagebreak: { mode:["css"] }
  };
  await html2pdf().set(opt).from(el).save();
  $("#pdfRoot").innerHTML = "";
}

async function exportVisitReport(){
  const cgId = $("#r1_cg").value;
  const month = $("#r1_month").value;
  const depFilter = $("#r1_dep").value;
  const cg = state.cgs.find(c=>c.id===cgId);
  if(!cg){ toast("กรุณาเลือก CG","err"); return; }
  let deps = state.dependents.filter(d=>d.cgId===cgId);
  if(depFilter) deps = deps.filter(d=>d.id===depFilter);
  if(!deps.length){ toast("ไม่พบผู้มีภาวะพึ่งพิงของ CG นี้","err"); return; }

  const snap = await db.collection("visits").where("cgId","==",cgId)
    .where("visitDate",">=",month+"-01").where("visitDate","<=",month+"-31").get();
  const allVisits = snap.docs.map(d=>d.data());

  const pages = deps.map(dep=>{
    const visits = allVisits.filter(v=>v.dependentId===dep.id).sort((a,b)=>a.visitDate.localeCompare(b.visitDate));
    const target = GROUP_INFO[dep.group]?.target || 1;
    return `<div class="report-page">
      ${reportHeader(`รายงานการเยี่ยมบ้านรายบุคคล — เดือน${fmtMonthLabel(month)}`)}
      <div class="rp-grid">
        <div class="k">ชื่อ-สกุล</div><div>${esc(dep.fullName)}</div>
        <div class="k">กลุ่ม Care Plan</div><div>${GROUP_INFO[dep.group]?.label||''} (เกณฑ์ ${target} ครั้ง/เดือน)</div>
        <div class="k">ที่อยู่</div><div>หมู่ ${esc(dep.moo||'-')} บ้าน${esc(dep.houseName||'-')}</div>
        <div class="k">CG ผู้เยี่ยม</div><div>${esc(cg.fullName)}</div>
        <div class="k">จำนวนครั้งที่เยี่ยม</div><div><b>${visits.length} / ${target} ครั้ง</b> ${visits.length>=target?'(ครบตามเกณฑ์)':'(ยังไม่ครบตามเกณฑ์)'}</div>
      </div>
      <div class="rp-section-title">รายละเอียดการเยี่ยมแต่ละครั้ง</div>
      <table class="rp-table">
        <thead><tr><th>วันที่</th><th>กิจกรรม</th><th>ADL</th><th>บันทึก</th></tr></thead>
        <tbody>
        ${visits.length? visits.map(v=>`<tr>
          <td>${fmtDate(v.visitDate)}</td>
          <td>${(v.activities||[]).join(", ")||'-'}</td>
          <td>${v.adl? v.adl.total+"/20" : "-"}</td>
          <td>${esc(v.notes||'-')}</td>
        </tr>`).join("") : `<tr><td colspan="4" style="text-align:center;color:#888;">ไม่มีการเยี่ยมในเดือนนี้</td></tr>`}
        </tbody>
      </table>
      ${visits.filter(v=>v.photo).length? `<div class="rp-section-title">ภาพประกอบการเยี่ยม</div>
        <div class="rp-photo-row">${visits.filter(v=>v.photo).slice(0,4).map(v=>`<img src="${v.photo}">`).join("")}</div>` : ""}
      ${reportSignature()}
    </div>`;
  }).join("");

  $("#pdfRoot").innerHTML = `<div id="pdfExportWrap">${pages}</div>`;
  await exportPdf("pdfExportWrap", `รายงานการเยี่ยม_${cg.fullName}_${month}.pdf`);
}

async function exportProfileReport(){
  let ids = $all("#r2_dep option:checked").map(o=>o.value);
  let deps = ids.length ? state.dependents.filter(d=>ids.includes(d.id)) : state.dependents;
  if(!deps.length){ toast("ไม่มีข้อมูลให้ออกรายงาน","err"); return; }
  const pages = deps.map(d=>{
    const cg = state.cgs.find(c=>c.id===d.cgId);
    return `<div class="report-page">
      ${reportHeader("แบบข้อมูลผู้มีภาวะพึ่งพิง")}
      <div class="rp-photo-row">
        ${d.photo?`<img src="${d.photo}">`:''}
        ${d.housePhoto?`<img src="${d.housePhoto}">`:''}
      </div>
      <div class="rp-grid">
        <div class="k">ชื่อ-สกุล</div><div>${esc(d.fullName)}</div>
        <div class="k">วันเกิด</div><div>${fmtDate(d.birthDate)}</div>
        <div class="k">เลขบัตร ปชช.</div><div>${esc(d.nationalId||'-')}</div>
        <div class="k">ที่อยู่</div><div>${esc(d.address||'-')} หมู่ ${esc(d.moo||'-')} บ้าน${esc(d.houseName||'-')}</div>
        <div class="k">เบอร์โทร</div><div>${esc(d.phone||'-')}</div>
        <div class="k">โรคประจำตัว</div><div>${esc(d.chronicDisease||'-')}</div>
        <div class="k">กลุ่ม Care Plan</div><div>${GROUP_INFO[d.group]?.label||''}</div>
        <div class="k">CG ผู้ดูแล</div><div>${esc(cg?cg.fullName:'-')}</div>
        <div class="k">ADL Baseline</div><div>${d.adlBaseline?`${d.adlBaseline.total}/20 (${fmtDate(d.adlBaseline.date)})`:'ยังไม่ประเมิน'}</div>
      </div>
      ${reportSignature()}
    </div>`;
  }).join("");
  $("#pdfRoot").innerHTML = `<div id="pdfExportWrap">${pages}</div>`;
  await exportPdf("pdfExportWrap", `ข้อมูลผู้มีภาวะพึ่งพิง.pdf`);
}

async function exportSummaryReport(){
  let ids = $all("#r3_dep option:checked").map(o=>o.value);
  let deps = ids.length ? state.dependents.filter(d=>ids.includes(d.id)) : state.dependents;
  if(!deps.length){ toast("ไม่มีข้อมูลให้ออกรายงาน","err"); return; }

  const pagesArr = [];
  for(const d of deps){
    const snap = await db.collection("visits").where("dependentId","==",d.id).orderBy("visitDate","asc").get();
    const visits = snap.docs.map(v=>v.data()).filter(v=>v.adl);
    const monthly = {};
    if(d.adlBaseline) monthly["Baseline"] = d.adlBaseline.total;
    visits.forEach(v=>{
      const ym = ymOf(v.visitDate);
      monthly[ym] = v.adl.total; // keep latest score of month
    });
    const keys = Object.keys(monthly);
    const cg = state.cgs.find(c=>c.id===d.cgId);
    const first = d.adlBaseline?d.adlBaseline.total:(visits[0]?visits[0].adl.total:null);
    const last = visits.length?visits[visits.length-1].adl.total:first;
    let trend = "-";
    if(first!==null && last!==null){
      trend = last>first? `ดีขึ้น (+${last-first} คะแนน)` : (last<first? `ลดลง (${last-first} คะแนน)` : "คงที่");
    }
    pagesArr.push(`<div class="report-page">
      ${reportHeader("สรุปผลการดำเนินงานเปรียบเทียบคะแนน ADL รายเดือน")}
      <div class="rp-grid">
        <div class="k">ชื่อ-สกุล</div><div>${esc(d.fullName)}</div>
        <div class="k">กลุ่ม Care Plan</div><div>${GROUP_INFO[d.group]?.label||''}</div>
        <div class="k">CG ผู้ดูแล</div><div>${esc(cg?cg.fullName:'-')}</div>
        <div class="k">จำนวนครั้งที่เยี่ยมสะสม</div><div>${visits.length + (d.adlBaseline?0:0)} ครั้ง (มีการประเมิน ADL)</div>
        <div class="k">แนวโน้ม ADL</div><div><b>${trend}</b></div>
      </div>
      <div class="rp-section-title">เปรียบเทียบคะแนน ADL รายเดือน (เต็ม 20 คะแนน)</div>
      ${keys.length? keys.map(k=>{
        const val = monthly[k];
        const pct = Math.round(val/20*100);
        const label = k==="Baseline" ? "ก่อนดูแล" : fmtMonthLabel(k);
        return `<div class="rp-bar-row"><div class="m">${esc(label)}</div><div class="rp-bar-track"><div class="rp-bar-fill" style="width:${pct}%;"></div></div><div class="rp-bar-val">${val}</div></div>`;
      }).join("") : `<div style="color:#888;">ยังไม่มีข้อมูลการประเมิน ADL</div>`}
      <div class="rp-section-title">สรุปผลการดำเนินงาน</div>
      <p style="font-size:13.5px;line-height:1.9;">
        ผู้มีภาวะพึ่งพิงรายนี้อยู่ใน${GROUP_INFO[d.group]?.label||''} ได้รับการเยี่ยมบ้านจาก CG ทั้งสิ้น ${visits.length} ครั้งที่มีการประเมิน ADL
        ${first!==null?`โดยคะแนน ADL เริ่มต้นอยู่ที่ ${first} คะแนน และคะแนนล่าสุดอยู่ที่ ${last} คะแนน จาก 20 คะแนน มีแนวโน้ม${trend}`:'ยังไม่มีข้อมูลคะแนน ADL เพียงพอสำหรับการเปรียบเทียบ'}
      </p>
      ${reportSignature()}
    </div>`);
  }
  $("#pdfRoot").innerHTML = `<div id="pdfExportWrap">${pagesArr.join("")}</div>`;
  await exportPdf("pdfExportWrap", `สรุปผลการดำเนินงาน.pdf`);
}

/* ======================================================================
   VIEW: ส่วนที่ 6 — จัดการผู้สมัคร/อนุมัติผู้ใช้งาน (admin)
   ====================================================================== */
async function viewAdmin(root){
  const snap = await db.collection("users").orderBy("createdAt","desc").get();
  const users = snap.docs.map(d=>({id:d.id,...d.data()}));
  const pending = users.filter(u=>u.status==="pending");
  const others = users.filter(u=>u.status!=="pending");

  root.innerHTML = `
    <div class="section-heading" style="margin-top:0;"><h2>รออนุมัติ (${pending.length})</h2></div>
    <div class="card card-pad" style="margin-bottom:26px;">
      ${pending.length? `<div class="table-wrap"><table class="data"><thead><tr>
        <th>ชื่อ-สกุล</th><th>Username</th><th>สิทธิ์</th><th></th>
      </tr></thead><tbody>
      ${pending.map(u=>`<tr>
        <td>${esc(u.fullName)}</td><td>@${esc(u.username)}</td>
        <td>${u.role}</td>
        <td style="white-space:nowrap;">
          <button class="btn btn-primary btn-sm" onclick="approveUser('${u.id}')">อนุมัติ</button>
          <button class="btn btn-danger btn-sm" onclick="rejectUser('${u.id}')">ปฏิเสธ</button>
        </td>
      </tr>`).join("")}
      </tbody></table></div>` : `<div class="empty-state"><div class="ic">✅</div>ไม่มีคำขอรออนุมัติ</div>`}
    </div>

    <div class="section-heading"><h2>ผู้ใช้งานทั้งหมด</h2></div>
    <div class="card card-pad">
      <div class="table-wrap"><table class="data"><thead><tr>
        <th>ชื่อ-สกุล</th><th>Username</th><th>สิทธิ์</th><th>สถานะ</th><th></th>
      </tr></thead><tbody>
      ${others.map(u=>`<tr>
        <td>${esc(u.fullName)}</td><td>@${esc(u.username)}</td>
        <td>${u.role}</td>
        <td><span class="badge badge-${u.status}">${u.status==='approved'?'อนุมัติแล้ว':'ปฏิเสธ'}</span></td>
        <td>${u.role!=='admin'?`<button class="btn btn-outline btn-sm" onclick="toggleUserStatus('${u.id}','${u.status}')">${u.status==='approved'?'ระงับสิทธิ์':'อนุมัติอีกครั้ง'}</button>`:''}</td>
      </tr>`).join("")}
      </tbody></table></div>
    </div>
  `;
}
async function approveUser(id){ await db.collection("users").doc(id).update({status:"approved"}); toast("อนุมัติแล้ว","ok"); renderShell(); }
async function rejectUser(id){ await db.collection("users").doc(id).update({status:"rejected"}); toast("ปฏิเสธคำขอแล้ว","ok"); renderShell(); }
async function toggleUserStatus(id, cur){ await db.collection("users").doc(id).update({status: cur==='approved'?'rejected':'approved'}); renderShell(); }

/* ======================================================================
   BOOTSTRAP
   ====================================================================== */
$("#menuToggle").addEventListener("click", ()=>{
  $("#sidebar").classList.toggle("open");
  $("#sidebarBackdrop").classList.toggle("show");
});
$("#sidebarBackdrop").addEventListener("click", closeSidebarMobile);

auth.onAuthStateChanged(async fbUser=>{
  if(fbUser){
    try{
      const snap = await db.collection("users").doc(fbUser.uid).get();
      if(snap.exists && snap.data().status === "approved"){
        state.user = { uid: fbUser.uid, ...snap.data() };
      } else {
        state.user = null;
      }
    }catch(e){ state.user = null; }
  } else {
    state.user = null;
  }
  $("#loading-screen").style.display = "none";
  $("#app").style.display = "flex";
  const r = window.location.hash.replace("#","") || "dashboard";
  state.route = r;
  renderShell();
});
</script>
</body>
</html>
