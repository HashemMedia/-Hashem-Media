<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#07090d">
<title>هاشم ميديا | Hashem Media</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800;900&family=Orbitron:wght@500;700;800&display=swap');

:root {
  --red: #d51e43;
  --white: #f4f5f7;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  min-height: 100vh;
  background: #07090d;
  color: white;
  font-family: 'Cairo', Arial, sans-serif;
  overflow-x: hidden;
}

/* الخلفية */
body::before {
  content: "";
  position: fixed;
  inset: 0;
  z-index: -2;
  background: url("background.png") center/cover no-repeat;
  filter: grayscale(1) contrast(1.12);
}

body::after {
  content: "";
  position: fixed;
  inset: 0;
  z-index: -1;
  background: linear-gradient(
    90deg,
    rgba(3,5,9,.86),
    rgba(3,5,9,.66),
    rgba(3,5,9,.88)
  );
}

/* الهيدر */
header {
  height: 94px;
  padding: 0 7%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid rgba(255,255,255,.1);
  background: rgba(4,7,12,.35);
  backdrop-filter: blur(14px);
}

.brand {
  display: flex;
  align-items: center;
  gap: 13px;
  font-size: 20px;
  font-weight: 900;
}

.brand-mark {
  width: 43px;
  height: 43px;
  border: 1px solid var(--red);
  display: grid;
  place-items: center;
  transform: rotate(45deg);
}

.brand-mark span {
  transform: rotate(-45deg);
  color: #ff315b;
  font-family: Orbitron;
}

.brand small {
  display: block;
  direction: ltr;
  font: 600 9px Orbitron;
  letter-spacing: 3px;
  color: #9ca5b2;
}

.header-tag {
  font: 10px Orbitron;
  color: #c4cad3;
  direction: ltr;
}

/* المحتوى الرئيسي */
main {
  min-height: calc(100vh - 94px);
  display: flex;
  align-items: center;
  padding: 70px 10% 100px;
}

.hero {
  max-width: 760px;
  animation: rise 1s ease;
}

.eyebrow {
  color: #e5e7eb;
  font-size: 12px;
  letter-spacing: 3px;
  margin-bottom: 22px;
}

h1 {
  font-size: clamp(55px, 9vw, 112px);
  line-height: 1.05;
  margin: 0;
  font-weight: 900;
}

h1 span {
  display: block;
  color: transparent;
  -webkit-text-stroke: 1.5px white;
  font-size: .52em;
  letter-spacing: 5px;
  direction: ltr;
  text-align: right;
  margin-top: 14px;
  font-family: Orbitron;
}

.accent-line {
  width: 90px;
  height: 4px;
  background: var(--red);
  margin: 32px 0 22px;
  box-shadow: 0 0 22px var(--red);
}

.desc {
  max-width: 510px;
  color: #c0c6d0;
  font-size: 16px;
  line-height: 2;
  margin-bottom: 37px;
}

/* الأزرار */
.actions {
  display: grid;
  grid-template-columns: repeat(2, minmax(190px, 230px));
  gap: 14px;
}

.btn {
  min-height: 62px;
  padding: 13px 18px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  text-decoration: none;
  color: white;
  border: 1px solid rgba(255,255,255,.2);
  background: rgba(255,255,255,.07);
  backdrop-filter: blur(12px);
  font-size: 15px;
  font-weight: 800;
  transition: .3s;
}

.btn:hover {
  border-color: #ff315b;
  transform: translateY(-4px);
  box-shadow: 0 0 25px rgba(213,30,67,.3);
  background: rgba(213,30,67,.2);
}

.arrow {
  color: #ff315b;
  font: 700 20px Orbitron;
}

.btn.primary {
  grid-column: span 2;
  background: linear-gradient(100deg,#a91032,#d51e43);
  border-color: #e32b50;
  max-width: 474px;
}

.btn.primary .arrow {
  color: white;
}

/* الحقوق */
footer {
  position: fixed;
  bottom: 0;
  right: 0;
  left: 0;
  padding: 15px 7%;
  display: flex;
  justify-content: space-between;
  border-top: 1px solid rgba(255,255,255,.08);
  background: rgba(4,6,10,.6);
  color: #858d99;
  font-size: 11px;
}

/* الحركة */
@keyframes rise {
  from {
    opacity: 0;
    transform: translateY(24px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* الهاتف */
@media(max-width:620px) {
  header {
    height: 78px;
    padding: 0 20px;
  }

  .brand {
    font-size: 16px;
  }

  .header-tag {
    font-size: 8px;
  }

  main {
    min-height: calc(100vh - 78px);
    padding: 55px 25px 105px;
  }

  h1 {
    font-size: 58px;
  }

  .actions {
    grid-template-columns: 1fr;
  }

  .btn.primary {
    grid-column: auto;
    max-width: none;
  }

  footer {
    font-size: 9px;
    padding: 13px 15px;
  }
}
</style>
</head>

<body>

<header>
  <div class="brand">
    <div class="brand-mark"><span>H</span></div>

    <div>
      هاشم ميديا
      <small>HASHEM MEDIA</small>
    </div>
  </div>

  <div class="header-tag">
    ● OFFICIAL MEDIA PLATFORM
  </div>
</header>

<main>
  <section class="hero">

    <div class="eyebrow">
      قوة الصورة... وهيبة الحضور
    </div>

    <h1>
      هاشم ميديا
      <span>HASHEM MEDIA</span>
    </h1>

    <div class="accent-line"></div>

    <p class="desc">
      منصّتكم لمشاهدة اللقطات والإصدارات —
      محتوى يُعرض بهوية تليق باسمه.
    </p>

    <nav class="actions">

      <a class="btn" href="#">
        <span>مشاهدة لقطات</span>
        <b class="arrow">←</b>
      </a>

      <a class="btn" href="#">
        <span>مشاهدات الإصدارات</span>
        <b class="arrow">←</b>
      </a>

      <a class="btn primary"
         href="https://t.me/"
         target="_blank">
        <span>للتواصل عبر التيليجرام</span>
        <b class="arrow">↗</b>
      </a>

    </nav>

  </section>
</main>

<footer>
  <span>© هاشم ميديا — جميع الحقوق محفوظة</span>
  <span>HASHEM MEDIA / OFFICIAL</span>
</footer>

</body>
</html>
