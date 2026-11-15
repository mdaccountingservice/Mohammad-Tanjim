<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Mohammad Tanjim - Professional Accountant and Bookkeeper Portfolio">
<title>Mohammad Tanjim | Accountant & Bookkeeper</title>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700;800&family=Cairo:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<style>
:root {
  --navy: #10243a;
  --white: #193954;
  --gold: #c99d55;
  --white: #ffffff;
  --bg: #f2f5f8;
  --text: #34465a;
  --muted: #748295;
}
* { box-sizing: border-box; }
html { scroll-behavior: smooth; }
body {
  margin: 0;
  background: var(--bg);
  color: var(--text);
  font-family: 'DM Sans', sans-serif;
  line-height: 1.7;
}
.container {
  max-width: 1100px;
  margin: auto;
  padding: 25px 20px 50px;
}
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 12px 0 25px;
}
.brand {
  font-weight: 800;
  color: var(--navy);
  letter-spacing: 2px;
}
nav a {
  color: var(--navy);
  text-decoration: none;
  margin-left: 15px;
  font-size: 14px;
  font-weight: 600;
}
nav a:hover { color: var(--gold); }

.hero {
  background: linear-gradient(120deg, var(--navy), var(--blue));
  color: white;
  border-radius: 20px;
  padding: 42px;
  display: grid;
  grid-template-columns: 1fr 175px;
  align-items: center;
  gap: 25px;
  box-shadow: 0 15px 40px #10243a20;
}
.hero h1 {
  font-size: clamp(30px, 5vw, 46px);
  margin: 8px 0;
  line-height: 1.2;
}
.eyebrow {
  color: #e8c88f;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 3px;
}
.role {
  color: #e4c58f;
  font-size: 19px;
  margin: 5px 0 20px;
}
.photo {
  width: 165px;
  height: 190px;
  object-fit: cover;
  object-position: center 22%;
  border: 5px solid white;
  border-radius: 14px;
}
.contact {
  display: flex;
  flex-wrap: wrap;
  gap: 10px 20px;
  font-size: 13px;
}
.contact a {
  color: white;
  text-decoration: none;
}
.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 18px;
  border-radius: 7px;
  text-decoration: none;
  font-size: 13px;
  font-weight: 700;
  background: var(--gold);
  color: var(--navy);
}
.btn:hover { opacity: .85; }

.section {
  background: white;
  border-radius: 15px;
  padding: 27px 30px;
  margin-top: 20px;
  border: 1px solid #e5eaf0;
  box-shadow: 0 5px 20px #10243a08;
}
.section h2 {
  color: var(--navy);
  font-size: 19px;
  border-left: 4px solid var(--gold);
  padding-left: 12px;
  margin: 0 0 18px;
}
.summary { color: #596b7d; }

.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
.skill, .tag {
  background: #f3f6f9;
  border: 1px solid #e8edf2;
  padding: 10px 12px;
  border-radius: 8px;
  font-size: 13px;
  font-weight: 600;
}
.job {
  border-left: 2px solid #e4eaf0;
  padding-left: 20px;
  margin-bottom: 27px;
  position: relative;
}
.job:before {
  content: "";
  position: absolute;
  left: -6px;
  top: 7px;
  background: var(--gold);
  width: 10px;
  height: 10px;
  border-radius: 50%;
}
.job h3 {
  color: var(--navy);
  margin: 0;
  font-size: 16px;
}
.company { color: var(--muted); font-size: 13px; }
.date {
  display: inline-block;
  margin: 6px 0;
  background: #fbf4e9;
  color: #88672f;
  padding: 4px 10px;
  border-radius: 20px;
  font-size: 12px;
  font-weight: 700;
}
.job ul { color: #596b7d; font-size: 13px; padding-left: 20px; }
.job li { margin-bottom: 5px; }

.two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 18px;
}
.tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}
.edu {
  padding: 12px;
  background: #f4f6f8;
  border-radius: 8px;
  margin-bottom: 10px;
}
.edu strong { display: block; color: var(--navy); }
.edu span { font-size: 12px; color: var(--muted); }
.footer {
  text-align: center;
  padding: 25px;
  color: var(--muted);
  font-size: 12px;
}

/* Arabic section */
.arabic {
  direction: rtl;
  text-align: right;
  font-family: 'Cairo', sans-serif;
  margin-top: 45px;
}
.arabic .hero {
  grid-template-columns: 175px 1fr;
}
.arabic .hero h1 { font-family: 'Cairo', sans-serif; }
.arabic .section h2 {
  border-left: 0;
  border-right: 4px solid var(--gold);
  padding-left: 0;
  padding-right: 12px;
}
.arabic .job {
  border-left: 0;
  border-right: 2px solid #e4eaf0;
  padding-left: 0;
  padding-right: 20px;
}
.arabic .job:before {
  left: auto;
  right: -6px;
}
.arabic .job ul { padding-left: 0; padding-right: 20px; }
.arabic .contact { direction: rtl; }
.arabic .photo { grid-column: 1; }
.arabic .hero-copy { grid-column: 2; grid-row: 1; }
.arabic .job h3, .arabic .edu strong { font-family: 'Cairo', sans-serif; }

@media(max-width:700px) {
  .container { padding: 12px; }
  nav { flex-wrap: wrap; gap: 12px; }
  nav a { margin-left: 8px; }
  .hero, .arabic .hero {
    display: flex;
    flex-direction: column-reverse;
    text-align: center;
    padding: 28px 18px;
  }
  .arabic .hero { flex-direction: column; }
  .photo { width: 140px; height: 155px; }
  .contact { justify-content: center; }
  .grid { grid-template-columns: repeat(2, 1fr); }
  .two-col { grid-template-columns: 1fr; }
  .section { padding: 22px 17px; }
}
@media print {
  body { background: white; }
  nav, .btn { display: none; }
  .arabic { page-break-before: always; }
}
</style>
</head>

<body>
<main class="container">

<nav>
  <div class="brand">MT | ACCOUNTING PORTFOLIO</div>
  <div>
    <a href="#english">English</a>
    <a href="#arabic">العربية</a>
    <a href="mailto:tanjimnepal@gmail.com">Contact</a>
  </div>
</nav>

<!-- ENGLISH PORTFOLIO -->

<div id="english">

<header class="hero">
  <div>
    <div class="eyebrow">PROFESSIONAL PORTFOLIO</div>
    <h1>Mohammad Tanjim</h1>
    <p class="role">Accountant & Bookkeeper</p>

    <div class="contact">
      <span>📍 Biratnagar, Nepal</span>
      <a href="mailto:tanjimnepal@gmail.com">✉ tanjimnepal@gmail.com</a>
      <a href="tel:+9779819337926">☎ +977 9819337926</a>
      <a href="https://www.linkedin.com/in/mohammad-tanjim-9a8117282" target="_blank">LinkedIn Profile</a>
    </div>

    <a class="btn" href="mailto:tanjimnepal@gmail.com">CONTACT ME</a>
  </div>

  <img class="photo" src="assets/profile.jpg" alt="Mohammad Tanjim">
</header>

<section class="section">
<h2>Professional Summary</h2>
<p class="summary">
Detail-oriented Accountant and Bookkeeper with over 8 years of experience in financial accounting, bookkeeping, accounts payable, accounts receivable, payroll processing, bank reconciliation, financial reporting, budgeting and tax compliance. Skilled in preparing financial statements, maintaining general ledger accounts, month-end closing, cash flow management, inventory control and supporting internal and external audits. Proficient in Tally Prime, Tally ERP 9, Zoho Books, Microsoft Excel and accounting software.
</p>
</section>

<section class="section">
<h2>Core Competencies</h2>
<div class="grid">
<div class="skill">Bookkeeping</div>
<div class="skill">Financial Reporting</div>
<div class="skill">Accounts Payable (AP)</div>
<div class="skill">Accounts Receivable (AR)</div>
<div class="skill">Bank Reconciliation</div>
<div class="skill">Journal Entries</div>
<div class="skill">Payroll Processing</div>
<div class="skill">Cash Flow Management</div>
<div class="skill">Budgeting</div>
<div class="skill">Fixed Asset Management</div>
<div class="skill">Inventory Accounting</div>
<div class="skill">VAT & Tax Compliance</div>
<div class="skill">Financial Statements</div>
<div class="skill">Month-End Closing</div>
<div class="skill">Audit Support</div>
</div>
</section>

<section class="section">
<h2>Professional Experience</h2>

<div class="job">
<h3>Accountant</h3>
<div class="company">Utsav Footwear and Trade Industries · Biratnagar, Nepal</div>
<div class="date">8 March 2023 – Present</div>
<ul>
<li>Prepare monthly, quarterly and annual financial statements.</li>
<li>Maintain the general ledger and ensure accurate bookkeeping.</li>
<li>Manage Accounts Payable and Accounts Receivable.</li>
<li>Process payroll and maintain employee payroll records.</li>
<li>Prepare projected balance sheets and financial reports for banks and management.</li>
<li>Perform bank reconciliations and cash flow monitoring.</li>
<li>Maintain fixed asset registers and calculate depreciation.</li>
<li>Prepare budgets and financial analyses.</li>
<li>Coordinate internal and external audits.</li>
<li>Prepare VAT and tax reports and ensure timely statutory compliance.</li>
<li>Support bank loan documentation and financial reporting.</li>
</ul>
</div>

<div class="job">
<h3>Accountant</h3>
<div class="company">Superior Motors · Biratnagar, Nepal</div>
<div class="date">19 October 2020 – 30 January 2023</div>
<ul>
<li>Managed daily bookkeeping and accounting transactions.</li>
<li>Prepared bank reconciliations and verified ledger balances.</li>
<li>Maintained Accounts Payable and Accounts Receivable.</li>
<li>Recorded journal entries and maintained accounting records.</li>
<li>Generated management reports.</li>
<li>Processed cheque payments and verified accounting transactions.</li>
<li>Maintained accounting records using Tally and Excel.</li>
</ul>
</div>

<div class="job">
<h3>Accountant</h3>
<div class="company">Amul Enterprises and Order Suppliers · Biratnagar, Koshi, Nepal</div>
<div class="date">10 July 2018 – 18 June 2020</div>
<ul>
<li>Maintained daily bookkeeping records.</li>
<li>Prepared invoices and verified supplier bills.</li>
<li>Recorded accounting transactions accurately.</li>
<li>Assisted with monthly reconciliations.</li>
<li>Maintained financial records using accounting software and Microsoft Excel.</li>
</ul>
</div>
</section>

<div class="two-col">
<section class="section">
<h2>Technical Skills</h2>
<div class="tags">
<span class="tag">Tally Prime</span>
<span class="tag">Tally ERP 9</span>
<span class="tag">Zoho Books</span>
<span class="tag">Microsoft Excel</span>
<span class="tag">VLOOKUP</span>
<span class="tag">XLOOKUP</span>
<span class="tag">Pivot Tables</span>
<span class="tag">Microsoft Word</span>
<span class="tag">PowerPoint</span>
<span class="tag">Saral Billing (IRD Verified)</span>
<span class="tag">English & Nepali Typing</span>
</div>
</section>

<section class="section">
<h2>Soft Skills</h2>
<div class="tags">
<span class="tag">Attention to Detail</span>
<span class="tag">Analytical Thinking</span>
<span class="tag">Time Management</span>
<span class="tag">Problem Solving</span>
<span class="tag">Communication Skills</span>
<span class="tag">Teamwork</span>
<span class="tag">Adaptability</span>
</div>
</section>
</div>

<div class="two-col">
<section class="section">
<h2>Education</h2>
<div class="edu">
<strong>Bachelor of Business Studies (BBS)</strong>
<span>Tribhuvan University · Biratnagar, Nepal · 2023</span>
</div>
<div class="edu">
<strong>Intermediate (+2), Commerce</strong>
<span>Bhanu Memorial English Boarding School · Biratnagar, Nepal · 2017</span>
</div>
<div class="edu">
<strong>School Leaving Certificate (SLC)</strong>
<span>Shree Jan Priya Higher Secondary School · Katahari, Nepal · 2015</span>
</div>
</section>

<section class="section">
<h2>Languages</h2>
<div class="tags">
<span class="tag">Maithili – Native</span>
<span class="tag">English – Professional</span>
<span class="tag">Hindi – Professional</span>
<span class="tag">Nepali – Professional</span>
</div>
</section>
</div>

</div>

<!-- ARABIC PORTFOLIO -->

<div id="arabic" class="arabic" lang="ar">

<header class="hero">
<img class="photo" src="assets/profile.jpg" alt="محمد تنزيم">
<div class="hero-copy">
<div class="eyebrow">الملف المهني</div>
<h1>محمد تنزيم</h1>
<p class="role">محاسب وممسك دفاتر</p>
<div class="contact">
<span>📍 بيراتناغار، نيبال</span>
<a href="mailto:tanjimnepal@gmail.com">tanjimnepal@gmail.com</a>
<a href="tel:+9779819337926">+977 9819337926</a>
<a href="https://www.linkedin.com/in/mohammad-tanjim-9a8117282" target="_blank">LinkedIn</a>
</div>
<a class="btn" href="mailto:tanjimnepal@gmail.com">تواصل معي</a>
</div>
</header>

<section class="section">
<h2>الملخص المهني</h2>
<p class="summary">
محاسب وممسك دفاتر يتمتع بخبرة تزيد عن 8 سنوات في المحاسبة المالية ومسك الدفاتر وحسابات الدفع والقبض ومعالجة الرواتب والتسويات البنكية وإعداد التقارير المالية والميزانيات والامتثال الضريبي. لديه خبرة في إعداد القوائم المالية والحفاظ على دفتر الأستاذ العام وإقفال الحسابات في نهاية الشهر وإدارة التدفقات النقدية ومراقبة المخزون ودعم عمليات التدقيق الداخلي والخارجي. يجيد استخدام Tally Prime وTally ERP 9 وZoho Books وMicrosoft Excel وبرامج المحاسبة.
</p>
</section>

<section class="section">
<h2>الكفاءات المهنية الأساسية</h2>
<div class="grid">
<div class="skill">مسك الدفاتر</div>
<div class="skill">التقارير المالية</div>
<div class="skill">حسابات الدفع (AP)</div>
<div class="skill">حسابات القبض (AR)</div>
<div class="skill">التسويات البنكية</div>
<div class="skill">القيود اليومية</div>
<div class="skill">معالجة الرواتب</div>
<div class="skill">إدارة التدفق النقدي</div>
<div class="skill">إعداد الميزانيات</div>
<div class="skill">إدارة الأصول الثابتة</div>
<div class="skill">محاسبة المخزون</div>
<div class="skill">ضريبة القيمة المضافة والضرائب</div>
<div class="skill">إعداد القوائم المالية</div>
<div class="skill">الإقفال الشهري</div>
<div class="skill">دعم التدقيق</div>
</div>
</section>

<section class="section">
<h2>الخبرة المهنية</h2>

<div class="job">
<h3>محاسب</h3>
<div class="company">شركة أوتساف للأحذية والصناعات التجارية · بيراتناغار، نيبال</div>
<div class="date">8 مارس 2023 – حتى الآن</div>
<ul>
<li>إعداد القوائم المالية الشهرية والربع سنوية والسنوية.</li>
<li>إدارة دفتر الأستاذ العام وضمان دقة مسك الدفاتر.</li>
<li>إدارة حسابات الدفع وحسابات القبض.</li>
<li>معالجة الرواتب والاحتفاظ بسجلات رواتب الموظفين.</li>
<li>إعداد الميزانيات العمومية التقديرية والتقارير المالية للبنوك والإدارة.</li>
<li>إجراء التسويات البنكية ومراقبة التدفق النقدي.</li>
<li>الاحتفاظ بسجلات الأصول الثابتة وحساب الإهلاك.</li>
<li>إعداد الميزانيات والتحليلات المالية.</li>
<li>التنسيق مع المدققين الداخليين والخارجيين.</li>
<li>إعداد تقارير ضريبة القيمة المضافة والضرائب.</li>
<li>دعم مستندات القروض البنكية والتقارير المالية.</li>
</ul>
</div>

<div class="job">
<h3>محاسب</h3>
<div class="company">سوبيريور موتورز · بيراتناغار، نيبال</div>
<div class="date">19 أكتوبر 2020 – 30 يناير 2023</div>
<ul>
<li>إدارة مسك الدفاتر اليومية والمعاملات المحاسبية.</li>
<li>إعداد التسويات البنكية والتحقق من أرصدة دفتر الأستاذ.</li>
<li>إدارة حسابات الدفع والقبض.</li>
<li>تسجيل القيود اليومية والحفاظ على السجلات المحاسبية.</li>
<li>إعداد تقارير الإدارة.</li>
<li>معالجة مدفوعات الشيكات والتحقق من المعاملات المحاسبية.</li>
<li>الحفاظ على السجلات المالية باستخدام Tally وExcel.</li>
</ul>
</div>

<div class="job">
<h3>محاسب</h3>
<div class="company">أمول إنتربرايزز وموردو الطلبات · بيراتناغار، كوشي، نيبال</div>
<div class="date">10 يوليو 2018 – 18 يونيو 2020</div>
<ul>
<li>الحفاظ على سجلات مسك الدفاتر اليومية.</li>
<li>إعداد الفواتير والتحقق من فواتير الموردين.</li>
<li>تسجيل المعاملات المحاسبية بدقة.</li>
<li>المساعدة في التسويات الشهرية.</li>
<li>الحفاظ على السجلات المالية باستخدام برامج المحاسبة وMicrosoft Excel.</li>
</ul>
</div>
</section>

<div class="two-col">
<section class="section">
<h2>المهارات التقنية والبرمجية</h2>
<div class="tags">
<span class="tag">Tally Prime</span>
<span class="tag">Tally ERP 9</span>
<span class="tag">Zoho Books</span>
<span class="tag">Microsoft Excel</span>
<span class="tag">VLOOKUP / XLOOKUP</span>
<span class="tag">Pivot Tables</span>
<span class="tag">Microsoft Word</span>
<span class="tag">PowerPoint</span>
<span class="tag">Saral Billing (IRD)</span>
<span class="tag">الطباعة بالإنجليزية والنيبالية</span>
</div>
</section>

<section class="section">
<h2>المهارات الشخصية</h2>
<div class="tags">
<span class="tag">الاهتمام بالتفاصيل</span>
<span class="tag">التفكير التحليلي</span>
<span class="tag">إدارة الوقت</span>
<span class="tag">حل المشكلات</span>
<span class="tag">مهارات التواصل</span>
<span class="tag">العمل الجماعي</span>
<span class="tag">القدرة على التكيف</span>
</div>
</section>
</div>

<div class="two-col">
<section class="section">
<h2>التعليم والمؤهلات الأكاديمية</h2>
<div class="edu">
<strong>بكالوريوس الدراسات التجارية (BBS)</strong>
<span>جامعة تريبهوفان · بيراتناغار، نيبال · 2023</span>
</div>
<div class="edu">
<strong>المرحلة المتوسطة (+2) – تجارة</strong>
<span>مدرسة بهانو ميموريال الإنجليزية الداخلية · بيراتناغار، نيبال · 2017</span>
</div>
<div class="edu">
<strong>شهادة إتمام الدراسة الثانوية (SLC)</strong>
<span>مدرسة شري جان بريا الثانوية · كاتاهاري، نيبال · 2015</span>
</div>
</section>

<section class="section">
<h2>اللغات</h2>
<div class="tags">
<span class="tag">الميثيلية – اللغة الأم</span>
<span class="tag">الإنجليزية – مستوى مهني</span>
<span class="tag">الهندية – مستوى مهني</span>
<span class="tag">النيبالية – مستوى مهني</span>
</div>
</section>
</div>

</div>

<footer class="footer">
© <span id="year"></span> Mohammad Tanjim | Accountant & Bookkeeper
</footer>

</main>

<script>
document.getElementById("year").textContent = new Date().getFullYear();
</script>

</body>
</html>
