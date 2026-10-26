<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>همسة بنات ♡</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700;800&display=swap');

:root {
    --pink: #f5dce5;
    --light-pink: #fff3f7;
    --dark-pink: #b47b91;
    --white: #ffffff;
    --text: #594b53;
    --muted: #8d7d85;
    --border: #f0e5e9;
    --lavender: #f6f2fb;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    background: #fffdfd;
    color: var(--text);
    font-family: "Cairo", Tahoma, Arial, sans-serif;
    line-height: 1.9;
}

button, input {
    font: inherit;
}

button {
    cursor: pointer;
}

header {
    background: white;
    border-bottom: 1px solid var(--border);
    padding: 16px 5%;
}

.header-inner {
    max-width: 1150px;
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
    flex-wrap: wrap;
}

.logo {
    color: var(--dark-pink);
    font-size: 29px;
    font-weight: 800;
    cursor: pointer;
}

.logo span {
    color: #d6a4b8;
}

.header-note {
    color: var(--muted);
    font-size: 13px;
}

nav {
    background: var(--light-pink);
    border-bottom: 1px solid var(--border);
    padding: 10px 3%;
}

.nav-inner {
    max-width: 1200px;
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 5px;
}

.nav-link {
    background: transparent;
    border: none;
    color: var(--text);
    padding: 7px 13px;
    border-radius: 22px;
    font-size: 13px;
    transition: 0.2s;
}

.nav-link:hover,
.nav-link.active {
    background: var(--pink);
    color: #754b5d;
}

main {
    max-width: 1100px;
    width: 92%;
    margin: 30px auto 55px;
}

.page {
    display: none;
    animation: appear 0.3s ease;
}

.page.active {
    display: block;
}

@keyframes appear {
    from {
        opacity: 0;
        transform: translateY(7px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.hero {
    background: linear-gradient(120deg, #fff0f5, white 58%, var(--lavender));
    border: 1px solid var(--border);
    border-radius: 27px;
    padding: 48px 24px;
    text-align: center;
    position: relative;
    overflow: hidden;
}

.decorations {
    color: #c995aa;
    font-size: 22px;
    letter-spacing: 5px;
    margin-bottom: 12px;
}

.hero h1 {
    color: #80576a;
    font-size: clamp(28px, 5vw, 42px);
    margin-bottom: 12px;
}

.hero p {
    max-width: 650px;
    margin: 0 auto 22px;
    color: var(--muted);
}

.button {
    display: inline-block;
    background: var(--pink);
    color: #754b5d;
    border: 1px solid #ebcbd7;
    border-radius: 25px;
    padding: 10px 22px;
    text-decoration: none;
    transition: 0.2s;
}

.button:hover {
    background: #edc7d5;
    transform: translateY(-2px);
}

.section-title {
    text-align: center;
    color: #80576a;
    font-size: 26px;
    margin: 35px 0 8px;
}

.section-description {
    text-align: center;
    color: var(--muted);
    margin-bottom: 22px;
}

.cards {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 18px;
}

.card {
    background: white;
    border: 1px solid var(--border);
    border-radius: 19px;
    padding: 23px;
    transition: 0.2s;
}

.card:hover {
    transform: translateY(-4px);
    border-color: #e6bdcd;
    box-shadow: 0 8px 24px #d9b7c31c;
}

.card-icon {
    width: 48px;
    height: 48px;
    display: grid;
    place-items: center;
    background: var(--light-pink);
    border-radius: 15px;
    font-size: 22px;
    margin-bottom: 12px;
}

.card h3 {
    color: #80576a;
    margin-bottom: 7px;
    font-size: 19px;
}

.card p {
    color: var(--muted);
    font-size: 14px;
    margin-bottom: 12px;
}

.card button {
    border: none;
    background: none;
    color: var(--dark-pink);
    font-weight: bold;
}

.card button:hover {
    text-decoration: underline;
}

.page-banner {
    text-align: center;
    background: linear-gradient(120deg, var(--light-pink), white, var(--lavender));
    border: 1px solid var(--border);
    border-radius: 23px;
    padding: 32px 20px;
    margin-bottom: 24px;
}

.page-banner .icon {
    font-size: 28px;
}

.page-banner h1 {
    color: #80576a;
    font-size: clamp(26px, 4vw, 35px);
}

.page-banner p {
    color: var(--muted);
    margin-top: 5px;
}

.article {
    background: white;
    border: 1px solid var(--border);
    border-radius: 18px;
    padding: 24px;
    margin-bottom: 18px;
}

.article h2 {
    color: #95677b;
    font-size: 21px;
    margin-bottom: 10px;
}

.article p {
    margin-bottom: 10px;
}

.article ul,
.article ol {
    padding-right: 25px;
    margin: 10px 0;
}

.article li {
    margin-bottom: 7px;
}

.tip {
    background: #faf6fd;
    border-right: 4px solid #d8c8e9;
    border-radius: 10px;
    padding: 14px;
    margin-top: 13px;
}

.quote-box {
    background: #fff5f8;
    border: 1px solid var(--border);
    color: #80576a;
    text-align: center;
    border-radius: 18px;
    padding: 22px;
    margin-top: 23px;
}

.back-button {
    display: block;
    margin: 24px auto 0;
    padding: 10px 23px;
    border: 1px solid #ebcbd7;
    background: var(--pink);
    color: #754b5d;
    border-radius: 25px;
}

.search-box {
    width: 100%;
    max-width: 550px;
    display: block;
    margin: 0 auto 25px;
    padding: 13px 17px;
    border: 1px solid var(--border);
    border-radius: 25px;
    background: white;
    outline: none;
}

.search-box:focus {
    border-color: #d6a4b8;
}

.search-result {
    text-align: center;
    color: var(--muted);
    margin: 10px 0;
}

footer {
    background: #fff7fa;
    border-top: 1px solid var(--border);
    text-align: center;
    color: var(--muted);
    padding: 25px 15px;
    font-size: 13px;
}

.footer-decoration {
    color: var(--dark-pink);
    font-size: 20px;
    margin-bottom: 6px;
}

footer p + p {
    margin-top: 5px;
}

@media (max-width: 800px) {
    .cards {
        grid-template-columns: repeat(2, minmax(0, 1fr));
    }

    .header-inner {
        justify-content: center;
        text-align: center;
    }
}

@media (max-width: 520px) {
    .cards {
        grid-template-columns: 1fr;
    }

    .nav-inner {
        gap: 3px;
    }

    .nav-link {
        padding: 6px 9px;
        font-size: 12px;
    }

    .hero {
        padding: 35px 17px;
    }

    .article {
        padding: 19px;
    }
}
</style>
</head>

<body>

<header>
    <div class="header-inner">
        <div class="logo" onclick="showPage('home')">
            همسة <span>بنات</span> ♡
        </div>
        <p class="header-note">مساحتكِ الصغيرة للقراءة والراحة</p>
    </div>
</header>

<nav>
    <div class="nav-inner">
        <button class="nav-link active" data-page="home" onclick="showPage('home')">الرئيسية</button>
        <button class="nav-link" data-page="confidence" onclick="showPage('confidence')">الثقة بالنفس</button>
        <button class="nav-link" data-page="friendship" onclick="showPage('friendship')">الصداقة</button>
        <button class="nav-link" data-page="selfcare" onclick="showPage('selfcare')">الاهتمام بالنفس</button>
        <button class="nav-link" data-page="study" onclick="showPage('study')">الدراسة</button>
        <button class="nav-link" data-page="feelings" onclick="showPage('feelings')">المشاعر</button>
        <button class="nav-link" data-page="personality" onclick="showPage('personality')">تطوير الذات</button>
        <button class="nav-link" data-page="daily" onclick="showPage('daily')">نصائح يومية</button>
    </div>
</nav>

<main>

<!-- الصفحة الأولى: الرئيسية -->
<section class="page active" id="home">

    <div class="hero">
        <div class="decorations">✿ ♡ 🦋 ♡ ✿</div>
        <h1>أهلًا بكِ في همسة بنات</h1>
        <p>
            هنا ستجدين كلمات لطيفة وأفكارًا مفيدة،
            ونصائح تساعدكِ على فهم نفسكِ والتعامل مع الحياة
            بخطوات صغيرة وواثقة.
        </p>
        <button class="button" onclick="showPage('confidence')">
            ابدئي القراءة ♡
        </button>
    </div>

    <h2 class="section-title">اختاري ما تحبين قراءته</h2>
    <p class="section-description">كل قسم فيه نصائح ومقالات خاصة فيه 🌷</p>

    <div class="cards">

        <article class="card">
            <div class="card-icon">♡</div>
            <h3>الثقة بالنفس</h3>
            <p>تعلّمي كيف تقدّرين نفسكِ وتثقين بقدراتكِ دون مقارنة نفسكِ بالآخرين.</p>
            <button onclick="showPage('confidence')">اقرئي النصائح ←</button>
        </article>

        <article class="card">
            <div class="card-icon">🌷</div>
            <h3>الصداقة</h3>
            <p>تعرّفي إلى الصداقة الصحية وكيفية التعامل مع الخلافات.</p>
            <button onclick="showPage('friendship')">اقرئي النصائح ←</button>
        </article>

        <article class="card">
            <div class="card-icon">☁</div>
            <h3>الاهتمام بالنفس</h3>
            <p>أفكار بسيطة للراحة والعناية بنفسكِ وتنظيم يومكِ.</p>
            <button onclick="showPage('selfcare')">اقرئي النصائح ←</button>
        </article>

        <article class="card">
            <div class="card-icon">📚</div>
            <h3>الدراسة</h3>
            <p>نصائح لتنظيم الوقت والمذاكرة والتركيز.</p>
            <button onclick="showPage('study')">اقرئي النصائح ←</button>
        </article>

        <article class="card">
            <div class="card-icon">💗</div>
            <h3>المشاعر</h3>
            <p>تعلّمي فهم مشاعركِ والتعبير عنها بطريقة هادئة.</p>
            <button onclick="showPage('feelings')">اقرئي النصائح ←</button>
        </article>

        <article class="card">
            <div class="card-icon">🦋</div>
            <h3>تطوير الذات</h3>
            <p>اكتشفي مواهبكِ وتعلمي مهارات جديدة واعملي نحو أهدافكِ.</p>
            <button onclick="showPage('personality')">اقرئي النصائح ←</button>
        </article>

        <article class="card">
            <div class="card-icon">✨</div>
            <h3>نصائح يومية</h3>
            <p>تذكيرات صغيرة وأفكار لطيفة يمكنكِ قراءتها في أي وقت.</p>
            <button onclick="showPage('daily')">اقرئي النصائح ←</button>
        </article>

    </div>

    <div class="quote-box">
        «ليس عليكِ أن تكوني مثالية؛ يكفي أن تمنحي نفسكِ فرصة جديدة.»
    </div>

</section>


<!-- الصفحة الثانية: الثقة بالنفس -->
<section class="page" id="confidence">

    <div class="page-banner">
        <div class="icon">♡ 🌷 ♡</div>
        <h1>الثقة بالنفس</h1>
        <p>قيمتكِ لا تحتاج إلى مقارنة، وصوتكِ يستحق أن يُسمع.</p>
    </div>

    <article class="article">
        <h2>1. لا تقارني نفسكِ بالآخرين</h2>
        <p>لكل إنسانة ظروفها وتجاربها وقدراتها. قد تتفوق صديقتكِ في مجال، وقد تتميزين أنتِ في مجال آخر. اختلافكما لا يعني أن إحداكما أفضل من الأخرى.</p>
        <p>بدلًا من سؤال نفسكِ: لماذا لست مثلها؟ اسألي: ما الشيء الذي أريد تعلمه؟ وما الخطوة التي أستطيع البدء بها؟</p>
        <div class="tip">تقدّمكِ لا يحتاج إلى أن يكون أسرع من تقدم الآخرين. المهم أن تتعلمي وتستمري.</div>
    </article>

    <article class="article">
        <h2>2. تعلّمي أن تقولي «لا» باحترام</h2>
        <p>ليس عليكِ الموافقة على كل شيء حتى يحبكِ الآخرون. يمكنكِ أن تكوني لطيفة وتحافظي في الوقت نفسه على حدودكِ.</p>
        <ul>
            <li>«أعتذر، لا أستطيع الآن».</li>
            <li>«أنا غير مرتاحة لهذا الأمر».</li>
            <li>«أحتاج إلى بعض الوقت للتفكير».</li>
        </ul>
    </article>

    <article class="article">
        <h2>3. الخطأ لا يعني الفشل</h2>
        <p>إذا أخطأتِ في اختبار أو لم تنجحي في تجربة، فهذا لا يعني أنكِ فاشلة. الخطأ جزء طبيعي من التعلم.</p>
        <ol>
            <li>حددي ما الذي لم ينجح.</li>
            <li>فكّري فيما يمكنكِ تحسينه.</li>
            <li>جرّبي مرة أخرى عندما تكونين مستعدة.</li>
        </ol>
    </article>

    <article class="article">
        <h2>4. افتخري بإنجازاتكِ الصغيرة</h2>
        <p>ربما أنهيتِ واجبًا صعبًا، أو تعلمتِ مهارة جديدة، أو ساعدتِ شخصًا. هذه أشياء تستحق التقدير، حتى لو بدت بسيطة للآخرين.</p>
    </article>

    <article class="article">
        <h2>5. عبّري عن رأيكِ</h2>
        <p>من حقكِ أن يكون لكِ رأي مختلف. استمعي للآخرين، واشرحي رأيكِ باحترام. ليس مطلوبًا أن يتفق الجميع معكِ في كل شيء.</p>
    </article>

    <div class="quote-box">أنتِ تستحقين الاحترام، حتى في الأيام التي تشكّين فيها بقدراتكِ. ♡</div>
    <button class="back-button" onclick="showPage('home')">العودة للرئيسية</button>

</section>


<!-- الصفحة الثالثة: الصداقة -->
<section class="page" id="friendship">

    <div class="page-banner">
        <div class="icon">🌷 🦋 🌷</div>
        <h1>الصداقة</h1>
        <p>الصداقة الجميلة تمنحكِ الأمان والاحترام.</p>
    </div>

    <article class="article">
        <h2>1. صفات الصديقة الجيدة</h2>
        <p>الصداقة ليست بعدد الرسائل أو طول مدة المعرفة فقط. الصديقة الجيدة تحترمكِ وتستمع إليكِ وتسمح لكِ بأن تكوني نفسكِ.</p>
        <ul>
            <li>تحترم مشاعركِ وخصوصيتكِ.</li>
            <li>تفرح لنجاحكِ ولا تقلل من إنجازاتكِ.</li>
            <li>تعتذر عندما تخطئ.</li>
            <li>لا تجبركِ على فعل شيء لا تريدينه.</li>
            <li>تختلف معكِ دون إهانتكِ.</li>
        </ul>
    </article>

    <article class="article">
        <h2>2. كيف تتعاملين مع الخلاف؟</h2>
        <p>الخلافات تحدث بين الأصدقاء. إذا كنتِ غاضبة، خذي بعض الوقت حتى تهدئي، ثم اشرحي ما أزعجكِ دون تجريح.</p>
        <div class="tip">يمكنكِ القول: «لما صار هذا الموقف، شعرت بالضيق. ممكن نحكي ونفهم بعض؟»</div>
    </article>

    <article class="article">
        <h2>3. إذا شعرتِ أن صديقتكِ ابتعدت</h2>
        <p>قد تنشغل الصديقة بالدراسة أو الأسرة أو ظروفها الخاصة. حاولي التحدث معها بدل افتراض الأسوأ.</p>
        <p>ومن الجميل أيضًا أن تكون لديكِ اهتمامات وعلاقات أخرى، حتى لا تصبح راحتكِ مرتبطة بشخص واحد فقط.</p>
    </article>

    <article class="article">
        <h2>4. حافظي على حدودكِ</h2>
        <p>إذا طلبت منكِ صديقة أن تكذبي أو تؤذي شخصًا أو تشاركي شيئًا خاصًا لا تريدين مشاركته، فمن حقكِ الرفض. الصداقة لا تعني تنفيذ كل طلب.</p>
    </article>

    <article class="article">
        <h2>5. كيف تكونين صديقة أفضل؟</h2>
        <ul>
            <li>استمعي عندما تتحدث صديقتكِ.</li>
            <li>احترمي أسرارها وخصوصيتها.</li>
            <li>اعتذري بصدق عندما تخطئين.</li>
            <li>اتركي لها مساحة ووقتًا لنفسها.</li>
            <li>عبّري عن تقديركِ لها.</li>
        </ul>
    </article>

    <div class="quote-box">الصداقة الصحية تجمع بين المحبة والاحترام والحرية. ♡</div>
    <button class="back-button" onclick="showPage('home')">العودة للرئيسية</button>

</section>


<!-- الصفحة الرابعة: الاهتمام بالنفس -->
<section class="page" id="selfcare">

    <div class="page-banner">
        <div class="icon">☁ ♡ 🌷</div>
        <h1>الاهتمام بالنفس</h1>
        <p>أنتِ أيضًا تستحقين وقتًا للراحة والاهتمام.</p>
    </div>

    <article class="article">
        <h2>1. ابدئي بعادات بسيطة</h2>
        <p>ليس عليكِ تغيير يومكِ كله دفعة واحدة. اختاري عادة صغيرة يسهل الالتزام بها، مثل ترتيب مكتبكِ أو تجهيز حقيبتكِ مساءً أو تخصيص دقائق للقراءة.</p>
    </article>

    <article class="article">
        <h2>2. امنحي النوم حقه</h2>
        <p>النوم الكافي يساعد على التركيز والتعلم والمزاج. حاولي جعل وقت النوم والاستيقاظ منتظمًا قدر الإمكان.</p>
    </article>

    <article class="article">
        <h2>3. خصصي وقتًا لهواية تحبينها</h2>
        <p>قد تكون هوايتكِ الرسم أو الكتابة أو القراءة أو البرمجة أو الزراعة. ليس ضروريًا أن تكوني محترفة؛ يكفي أن تستمتعي بالتجربة.</p>
        <div class="tip">جربي تخصيص 15 دقيقة لهواية تحبينها عندما يسمح وقتكِ.</div>
    </article>

    <article class="article">
        <h2>4. خذي استراحة من مواقع التواصل</h2>
        <p>إذا لاحظتِ أن تصفح مواقع التواصل يجعلكِ متوترة أو مشتتة، جربي تحديد وقت لاستخدامها. يمكنكِ استبدال بعض وقت الشاشة بالقراءة أو الرسم أو الحديث مع أسرتكِ.</p>
    </article>

    <article class="article">
        <h2>5. لا تلومي نفسكِ على الحاجة إلى الراحة</h2>
        <p>قد تمر عليكِ أيام مليئة بالواجبات. الراحة ليست فشلًا؛ إنها حاجة طبيعية. رتبي أولوياتكِ وخذي استراحة عندما تحتاجين إليها.</p>
    </article>

    <article class="article">
        <h2>6. تحدثي مع شخص تثقين به</h2>
        <p>إذا شعرتِ بالضغط أو واجهتِ مشكلة يصعب عليكِ التعامل معها، يمكنكِ التحدث مع أحد والديكِ أو معلمة أو شخص بالغ موثوق.</p>
    </article>

    <div class="quote-box">اهتمامكِ بنفسكِ يبدأ بخطوات صغيرة، وليس بالكمال. ♡</div>
    <button class="back-button" onclick="showPage('home')">العودة للرئيسية</button>

</section>


<!-- الصفحة الخامسة: الدراسة -->
<section class="page" id="study">

    <div class="page-banner">
        <div class="icon">📚 ✎ ♡</div>
        <h1>الدراسة وتنظيم الوقت</h1>
        <p>ابدئي بخطوة صغيرة، ثم انتقلي إلى الخطوة التالية.</p>
    </div>

    <article class="article">
        <h2>1. اكتبي قائمة بواجباتكِ</h2>
        <p>عندما تكون المهام كثيرة، اكتبي كل ما عليكِ فعله، ثم رتبيه بحسب موعد التسليم والأهمية.</p>
        <ul>
            <li>اكتبي الواجبات المطلوبة.</li>
            <li>قسمي المهمة الكبيرة إلى خطوات أصغر.</li>
            <li>ابدئي بمهمة واحدة.</li>
            <li>ضعي علامة أمام كل مهمة تنتهين منها.</li>
        </ul>
    </article>

    <article class="article">
        <h2>2. جربي الدراسة على فترات</h2>
        <p>يمكنكِ الدراسة لمدة 25 دقيقة ثم أخذ استراحة قصيرة، أو اختيار مدة أخرى تناسب تركيزكِ.</p>
        <div class="tip">جهزي الكتب والأقلام قبل البدء، وأبعدي المشتتات قدر الإمكان.</div>
    </article>

    <article class="article">
        <h2>3. اختبري فهمكِ بنفسكِ</h2>
        <p>بعد قراءة الدرس، أغلقي الكتاب وحاولي شرح الفكرة بكلماتكِ. اكتبي ما تتذكرينه، ثم افتحي الكتاب لمراجعة المعلومات وتصحيح الأخطاء.</p>
    </article>

    <article class="article">
        <h2>4. ماذا تفعلين عندما لا تفهمين؟</h2>
        <ul>
            <li>أعيدي قراءة الجزء الصعب ببطء.</li>
            <li>ابحثي عن مثال آخر.</li>
            <li>اكتبي السؤال الذي لم تفهميه.</li>
            <li>اطلبي من المعلمة شرح الفكرة بطريقة أخرى.</li>
        </ul>
    </article>

    <article class="article">
        <h2>5. استعدي للاختبار دون ضغط زائد</h2>
        <p>وزعي المراجعة على عدة أيام إن أمكن، وراجعي النقاط الأساسية وحلي أسئلة تدريبية. حاولي الحصول على نوم كافٍ قبل الاختبار.</p>
    </article>

    <article class="article">
        <h2>6. العلامة ليست كل شيء</h2>
        <p>العلامة تخبركِ عن أدائكِ في مهمة معينة، لكنها لا تحدد كل ما تستطيعين تعلمه أو تحقيقه. استفيدي من الأخطاء لمعرفة ما يحتاج إلى مراجعة.</p>
    </article>

    <div class="quote-box">كل خطوة تعلم تقومين بها اليوم يمكن أن تساعدكِ غدًا. ♡</div>
    <button class="back-button" onclick="showPage('home')">العودة للرئيسية</button>

</section>


<!-- الصفحة السادسة: المشاعر -->
<section class="page" id="feelings">

    <div class="page-banner">
        <div class="icon">♡ ☁ ♡</div>
        <h1>فهم المشاعر</h1>
        <p>مشاعركِ تستحق أن تفهميها، حتى عندما يصعب شرحها.</p>
    </div>

    <article class="article">
        <h2>1. من الطبيعي أن تتغير مشاعركِ</h2>
        <p>قد تشعرين بالفرح أو الحزن أو القلق أو الغضب خلال اليوم نفسه. وجود شعور مزعج لا يعني أنكِ ضعيفة؛ فالمشاعر جزء طبيعي من الحياة.</p>
    </article>

    <article class="article">
        <h2>2. حاولي تسمية الشعور</h2>
        <p>اسألي نفسكِ: هل أشعر بالحزن؟ أم الخوف؟ أم الإحباط؟ أم أنني متعبة وأحتاج إلى استراحة؟ معرفة الشعور قد تساعدكِ على التعامل معه.</p>
    </article>

    <article class="article">
        <h2>3. عندما تشعرين بالغضب</h2>
        <p>إذا كان الغضب شديدًا، خذي استراحة من النقاش إن أمكن. انتظري حتى تستطيعي التعبير عن نفسكِ دون إهانة أو تجريح.</p>
        <div class="tip">يمكنكِ القول: «أنا منزعجة الآن، وأحتاج إلى بعض الوقت حتى أتكلم بهدوء».</div>
    </article>

    <article class="article">
        <h2>4. عندما تشعرين بالحزن</h2>
        <p>لا تحتاجين إلى التظاهر بالسعادة طوال الوقت. قد يساعدكِ أن تكتبي ما تشعرين به، أو تمارسي هواية تحبينها، أو تتحدثي مع شخص تثقين به.</p>
        <p>إذا استمر الحزن وأثر في حياتكِ اليومية، اطلبي الدعم من شخص بالغ موثوق أو مختص مناسب.</p>
    </article>

    <article class="article">
        <h2>5. عبّري عن احتياجاتكِ بوضوح</h2>
        <p>شرح ما تشعرين به يساعد الآخرين على فهمكِ. حاولي استخدام عبارات تبدأ بـ«أنا أشعر» بدلًا من اتهام الطرف الآخر.</p>
    </article>

    <article class="article">
        <h2>6. لا تحاولي حل كل شيء وحدكِ</h2>
        <p>إذا كان هناك أمر يزعجكِ كثيرًا أو يجعلكِ تشعرين بعدم الأمان، تحدثي مع شخص بالغ تثقين به، مثل أحد والديكِ أو معلمة أو مرشدة المدرسة.</p>
    </article>

    <div class="quote-box">ليس عليكِ فهم كل شيء في لحظة واحدة. ابدئي بالإنصات إلى نفسكِ. ♡</div>
    <button class="back-button" onclick="showPage('home')">العودة للرئيسية</button>

</section>


<!-- الصفحة السابعة: تطوير الذات -->
<section class="page" id="personality">

    <div class="page-banner">
        <div class="icon">🦋 ✨ 🌷</div>
        <h1>تطوير الذات</h1>
        <p>كل مهارة جديدة فرصة لاكتشاف جانب جديد من نفسكِ.</p>
    </div>

    <article class="article">
        <h2>1. اكتشفي الأشياء التي تحبينها</h2>
        <p>فكري في الأنشطة التي تستمتعين بها، مثل الرسم أو القراءة أو الكتابة أو التكنولوجيا أو تعلم اللغات أو مساعدة الآخرين.</p>
        <p>ليس ضروريًا أن تختاري اهتمامًا واحدًا فقط. جربي أشياء مختلفة ولاحظي ما الذي يجعلكِ تشعرين بالفضول.</p>
    </article>

    <article class="article">
        <h2>2. تعلمي مهارة خطوة بخطوة</h2>
        <p>إذا أردتِ تعلم البرمجة، ابدئي بصفحة بسيطة. وإذا أحببتِ الرسم، اختاري رسمة صغيرة وتدربي عليها. البداية لا تحتاج إلى أن تكون مثالية.</p>
        <div class="tip">اختاري مهارة واحدة هذا الأسبوع، وخصصي لها وقتًا قصيرًا عندما يسمح يومكِ بذلك.</div>
    </article>

    <article class="article">
        <h2>3. اكتبي أهدافًا واضحة</h2>
        <p>بدلًا من كتابة «أريد أن أتطور»، اختاري هدفًا محددًا يمكنكِ العمل عليه.</p>
        <ul>
            <li>قراءة صفحات قليلة من كتاب.</li>
            <li>تعلم كلمات جديدة بلغة تحبينها.</li>
            <li>إنجاز مشروع صغير.</li>
            <li>التدرب على مهارة تحتاجين إليها.</li>
        </ul>
    </article>

    <article class="article">
        <h2>4. لا تخافي من البداية</h2>
        <p>كل شخص يتعلم شيئًا جديدًا يمر بمرحلة لا يعرف فيها الكثير. لا تقارني بدايتكِ بخبرة شخص يتعلم منذ سنوات. امنحي نفسكِ وقتًا للتجربة.</p>
    </article>

    <article class="article">
        <h2>5. اجعلي أهدافكِ مناسبة لظروفكِ</h2>
        <p>قد تكون لديكِ الدراسة أو مسؤوليات عائلية أو وقت محدود. اختاري أهدافًا تناسب وقتكِ وإمكاناتكِ الحالية، وعدلي خطتكِ عندما تحتاجين إلى ذلك.</p>
    </article>

    <article class="article">
        <h2>6. اكتبي رسالة إلى نفسكِ المستقبلية</h2>
        <p>اكتبي ما تتمنين تعلمه، والأشياء التي تفتخرين بها الآن، والعادات التي تريدين تطويرها. عودي إلى الرسالة بعد عدة أشهر لتري كيف تغيرت أفكاركِ وتجاربكِ.</p>
    </article>

    <div class="quote-box">لا تحتاجين إلى معرفة الطريق كله؛ يكفي أن تبدئي بخطوة. ♡</div>
    <button class="back-button" onclick="showPage('home')">العودة للرئيسية</button>

</section>


<!-- الصفحة الثامنة: نصائح يومية -->
<section class="page" id="daily">

    <div class="page-banner">
        <div class="icon">🌸 ♡ 🦋</div>
        <h1>نصائح يومية</h1>
        <p>تذكيرات صغيرة وأفكار لطيفة يمكنكِ قراءتها في أي وقت.</p>
    </div>

    <input
        type="search"
        id="tipSearch"
        class="search-box"
        placeholder="ابحثي عن نصيحة... مثل الدراسة أو الصداقة"
        aria-label="البحث في النصائح"
    >

    <p id="searchResult" class="search-result"></p>

    <div id="dailyTips">

        <article class="article">
            <h2>🌷 تذكير لنفسكِ</h2>
            <p>ليس عليكِ أن تكوني مثالية حتى تكوني إنسانة رائعة. من الطبيعي أن تخطئي وتتعلمي وتغيري رأيكِ مع الوقت.</p>
        </article>

        <article class="article">
            <h2>📚 نصيحة للدراسة</h2>
            <p>إذا شعرتِ أن واجبكِ كبير، قسميه إلى خطوات صغيرة. ابدئي بخطوة واحدة، ثم انتقلي إلى التالية.</p>
        </article>

        <article class="article">
            <h2>♡ نصيحة للصداقة</h2>
            <p>قبل أن تحكمي على تصرف صديقتكِ، حاولي فهم ما حدث. اسألي بهدوء بدلًا من افتراض الأسوأ.</p>
        </article>

        <article class="article">
            <h2>🦋 نصيحة للثقة بالنفس</h2>
            <p>لا تجعلي اختلافكِ عن الآخرين سببًا لتقليل قيمة نفسكِ. لكل إنسانة اهتماماتها وأفكارها وقدراتها.</p>
        </article>

        <article class="article">
            <h2>☁ نصيحة للراحة</h2>
            <p>عندما يمتلئ يومكِ بالمهام، توقفي قليلًا ورتبي أولوياتكِ. ليس كل شيء مستعجلًا.</p>
        </article>

        <article class="article">
            <h2>✨ نصيحة لتحقيق الأهداف</h2>
            <p>اكتبي هدفًا واحدًا تريدين الاقتراب منه هذا الأسبوع، ثم اختاري خطوة صغيرة تساعدكِ على البدء.</p>
        </article>

        <article class="article">
            <h2>💗 نصيحة عند الشعور بالضيق</h2>
            <p>حاولي تسمية الشعور الذي تمرين به وخذي وقتًا للهدوء. وإذا احتجتِ إلى الدعم، تحدثي مع شخص تثقين به.</p>
        </article>

        <article class="article">
            <h2>🌼 نصيحة للتعامل مع الآخرين</h2>
            <p>كوني لطيفة قدر الإمكان، لكن تذكري أن اللطف لا يعني قبول الإهانة أو التخلي عن حدودكِ.</p>
        </article>

        <article class="article">
            <h2>📖 فكرة صغيرة للتجربة</h2>
            <p>في نهاية اليوم، اكتبي شيئًا تعلمتِه، وشيئًا أسعدكِ، وشيئًا تريدين تجربته غدًا.</p>
        </article>

        <article class="article">
            <h2>🌷 نصيحة عندما تخطئين</h2>
            <p>بدلًا من لوم نفسكِ طوال الوقت، فكري فيما يمكنكِ تعلمه من الموقف وكيف يمكنكِ التصرف في المرة المقبلة.</p>
        </article>

        <article class="article">
            <h2>🦋 تذكير جميل</h2>
            <p>لا تحتاجين إلى مقارنة نفسكِ بالآخرين حتى تعرفي أنكِ تتقدمين. لاحظي ما تعلمتِه وما أصبح أسهل بالنسبة إليكِ.</p>
        </article>

        <article class="article">
            <h2>💗 نصيحة للوقت</h2>
            <p>إذا كان لديكِ الكثير لتفعليه، اختاري أهم مهمة وابدئي بها. لا تسمحي لكثرة المهام أن تمنعكِ من البدء.</p>
        </article>

    </div>

    <div class="quote-box">خذي من النصائح ما يناسبكِ، وتذكري أن لكل إنسانة ظروفها وطريقتها الخاصة. ♡</div>
    <button class="back-button" onclick="showPage('home')">العودة للرئيسية</button>

</section>

</main>

<footer>
    <div class="footer-decoration">✿ ♡ 🦋 ♡ ✿</div>
    <p>همسة بنات — كلمات صغيرة، ومعانٍ جميلة.</p>
    <p>مساحة للقراءة والتعلّم والتشجيع.</p>
    <p>© 2026 همسة بنات</p>
</footer>

<script>
function showPage(pageId) {
    const pages = document.querySelectorAll('.page');
    const links = document.querySelectorAll('.nav-link');

    let pageExists = false;

    pages.forEach(function(page) {
        page.classList.remove('active');

        if (page.id === pageId) {
            pageExists = true;
        }
    });

    if (!pageExists) {
        pageId = 'home';
    }

    document.getElementById(pageId).classList.add('active');

    links.forEach(function(link) {
        link.classList.remove('active');

        if (link.dataset.page === pageId) {
            link.classList.add('active');
        }
    });

    window.scrollTo({
        top: 0,
        behavior: 'smooth'
    });
}

const tipSearch = document.getElementById('tipSearch');

tipSearch.addEventListener('input', function() {
    const query = tipSearch.value.trim().toLowerCase();
    const tips = document.querySelectorAll('#dailyTips .article');
    let visibleCount = 0;

    tips.forEach(function(tip) {
        const text = tip.innerText.toLowerCase();
        const matches = text.includes(query);

        tip.style.display = matches ? '' : 'none';

        if (matches) {
            visibleCount++;
        }
    });

    const result = document.getElementById('searchResult');

    if (query === '') {
        result.textContent = '';
    } else if (visibleCount === 0) {
        result.textContent = 'لم نعثر على نصيحة مطابقة. جربي كلمة أخرى.';
    } else {
        result.textContent = 'عدد النصائح التي وجدناها: ' + visibleCount;
    }
});
</script>

</body>
</html># naba-albanat
Naba Al-Banat is a beautiful website created for girls, offering a welcoming space for inspiration, creativity, learning, and sharing ideas.
