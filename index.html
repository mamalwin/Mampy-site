<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>راهنمای جامع ربات مدیریت گروه | MAMPY Helper</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
    <link rel="stylesheet" href="https://cdn.fontsource.org/fonts/vazir@5.0.0-alpha.2/css/vazir.min.css" />
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --bg: #f4f8fe;
            --card: #ffffff;
            --text: #1e293b;
            --text-light: #64748b;
            --primary: #3b82f6;
            --primary-dark: #2563eb;
            --primary-glow: rgba(59, 130, 246, 0.2);
            --shadow: 0 20px 40px rgba(0, 0, 0, 0.05);
            --radius: 24px;
            --transition: 0.35s cubic-bezier(0.34, 1.56, 0.64, 1);
        }

        body.dark {
            --bg: #0f172a;
            --card: #1e293b;
            --text: #f1f5f9;
            --text-light: #94a3b8;
            --shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
        }

        body {
            font-family: 'Vazir', 'Segoe UI', system-ui, -apple-system, sans-serif;
            background: var(--bg);
            color: var(--text);
            transition: background var(--transition), color var(--transition);
            padding: 20px;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            line-height: 1.8;
            font-weight: 300;
        }

        .container {
            max-width: 1000px;
            width: 100%;
            background: var(--card);
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            padding: 30px 28px;
            transition: background var(--transition), box-shadow var(--transition);
            animation: fadeIn 0.7s ease;
            position: relative;
            min-height: 550px;
        }

        @keyframes fadeIn {
            0% { opacity: 0; transform: translateY(30px) scale(0.97); }
            100% { opacity: 1; transform: translateY(0) scale(1); }
        }

        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 12px;
            margin-bottom: 28px;
            padding-bottom: 18px;
            border-bottom: 2px solid rgba(59, 130, 246, 0.1);
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-icon {
            width: 48px;
            height: 48px;
            background: linear-gradient(135deg, var(--primary), #8b5cf6);
            border-radius: 16px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            color: #fff;
            box-shadow: 0 8px 24px var(--primary-glow);
            animation: pulseGlow 3s infinite;
        }

        @keyframes pulseGlow {
            0%, 100% { box-shadow: 0 8px 24px var(--primary-glow); }
            50% { box-shadow: 0 8px 40px var(--primary-glow), 0 0 60px rgba(59, 130, 246, 0.12); }
        }

        .logo h1 {
            font-size: 24px;
            font-weight: 700;
            letter-spacing: -0.3px;
            background: linear-gradient(135deg, var(--primary), #8b5cf6);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .logo span {
            font-size: 13px;
            color: var(--text-light);
            display: block;
            margin-top: 2px;
            font-weight: 300;
        }

        .theme-toggle {
            background: var(--bg);
            border: none;
            width: 46px;
            height: 46px;
            border-radius: 50%;
            font-size: 20px;
            color: var(--text);
            cursor: pointer;
            transition: all var(--transition);
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.04);
        }

        .theme-toggle:hover {
            transform: rotate(30deg) scale(1.08);
            background: var(--primary);
            color: #fff;
        }

        .tabs {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 28px;
            border-bottom: 2px solid rgba(59, 130, 246, 0.08);
            padding-bottom: 12px;
        }

        .tab-btn {
            background: transparent;
            border: none;
            padding: 10px 20px;
            border-radius: 40px;
            font-size: 14px;
            font-weight: 500;
            color: var(--text-light);
            cursor: pointer;
            transition: all var(--transition);
            display: flex;
            align-items: center;
            gap: 8px;
            white-space: nowrap;
            font-family: 'Vazir', sans-serif;
        }

        .tab-btn i {
            font-size: 15px;
        }

        .tab-btn:hover {
            background: var(--bg);
            color: var(--primary);
        }

        .tab-btn.active {
            background: var(--primary);
            color: #fff;
            box-shadow: 0 8px 24px var(--primary-glow);
        }

        .panel {
            display: none;
            animation: slideUp 0.4s ease;
        }

        .panel.active {
            display: block;
        }

        @keyframes slideUp {
            0% { opacity: 0; transform: translateY(15px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        .panel-title {
            font-size: 26px;
            font-weight: 700;
            margin-bottom: 6px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .panel-title i {
            color: var(--primary);
            font-size: 28px;
        }

        .panel-desc {
            color: var(--text-light);
            margin-bottom: 22px;
            font-size: 16px;
            border-right: 4px solid var(--primary);
            padding-right: 16px;
            background: rgba(59, 130, 246, 0.04);
            border-radius: 0 12px 12px 0;
            padding: 14px 18px;
            font-weight: 300;
            line-height: 1.9;
        }

        .items-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
            gap: 16px;
            margin-top: 10px;
        }

        .item-btn {
            background: var(--bg);
            border: 1px solid transparent;
            border-radius: 18px;
            padding: 18px 16px;
            cursor: pointer;
            transition: all var(--transition);
            text-align: right;
            font-family: 'Vazir', sans-serif;
            color: var(--text);
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .item-btn:hover {
            transform: translateY(-3px);
            border-color: var(--primary);
            box-shadow: 0 10px 28px rgba(59, 130, 246, 0.06);
            background: rgba(59, 130, 246, 0.04);
        }

        .item-btn .icon {
            width: 40px;
            height: 40px;
            background: linear-gradient(135deg, var(--primary), #8b5cf6);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 18px;
            color: #fff;
            flex-shrink: 0;
            box-shadow: 0 6px 18px var(--primary-glow);
        }

        .item-btn .info {
            flex: 1;
        }

        .item-btn .info h4 {
            font-size: 16px;
            font-weight: 600;
            margin-bottom: 2px;
        }

        .item-btn .info p {
            font-size: 13px;
            color: var(--text-light);
            font-weight: 300;
        }

        .detail-view {
            display: none;
            animation: slideUp 0.4s ease;
        }

        .detail-view.active {
            display: block;
        }

        .detail-header {
            display: flex;
            align-items: center;
            gap: 14px;
            margin-bottom: 16px;
            padding-bottom: 14px;
            border-bottom: 2px solid rgba(59, 130, 246, 0.08);
        }

        .back-btn {
            background: var(--bg);
            border: none;
            padding: 10px 20px;
            border-radius: 40px;
            font-size: 14px;
            font-weight: 500;
            color: var(--text);
            cursor: pointer;
            transition: all var(--transition);
            font-family: 'Vazir', sans-serif;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .back-btn:hover {
            background: var(--primary);
            color: #fff;
            box-shadow: 0 8px 24px var(--primary-glow);
        }

        .detail-title {
            font-size: 24px;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .detail-title i {
            color: var(--primary);
        }

        .detail-description {
            background: rgba(59, 130, 246, 0.04);
            border-radius: 16px;
            padding: 18px 20px;
            margin-bottom: 22px;
            border-right: 4px solid var(--primary);
            color: var(--text);
            font-weight: 300;
            line-height: 2;
            font-size: 16px;
        }

        .detail-commands {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .command-item {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 12px 16px;
            background: var(--bg);
            border-radius: 14px;
            transition: background var(--transition);
        }

        .command-item:hover {
            background: rgba(59, 130, 246, 0.06);
        }

        .command-item .cmd-badge {
            font-family: 'Courier New', monospace;
            font-weight: 700;
            color: var(--primary);
            background: rgba(59, 130, 246, 0.1);
            padding: 4px 16px;
            border-radius: 30px;
            font-size: 14px;
            letter-spacing: 0.3px;
        }

        .command-item .cmd-desc {
            color: var(--text-light);
            font-size: 14px;
            font-weight: 300;
        }

        @media (max-width: 640px) {
            .container { padding: 20px 14px; }
            .logo h1 { font-size: 20px; }
            .tab-btn { font-size: 13px; padding: 8px 14px; }
            .items-grid { grid-template-columns: 1fr; }
            .panel-title { font-size: 22px; }
            .detail-title { font-size: 20px; }
            .command-item { flex-direction: column; align-items: flex-start; gap: 6px; }
        }

        ::-webkit-scrollbar { width: 6px; }
        ::-webkit-scrollbar-track { background: var(--bg); border-radius: 10px; }
        ::-webkit-scrollbar-thumb { background: var(--primary); border-radius: 10px; }
    </style>
</head>
<body>
    <div class="container" id="app">
        <!-- HEADER -->
        <header class="header">
            <div class="logo">
                <div class="logo-icon"><i class="fas fa-robot"></i></div>
                <div>
                    <h1>راهنمای MAMPY Helper</h1>
                    <span>مدیریت حرفه‌ای گروه در پیام‌رسان بله</span>
                </div>
            </div>
            <button class="theme-toggle" id="themeToggle" aria-label="تغییر تم">
                <i class="fas fa-moon"></i>
            </button>
        </header>

        <nav class="tabs" id="tabContainer">
            <button class="tab-btn active" data-panel="panel-lock"><i class="fas fa-lock"></i> قفل‌ها</button>
            <button class="tab-btn" data-panel="panel-set"><i class="fas fa-sliders-h"></i> تنظیمات</button>
            <button class="tab-btn" data-panel="panel-filter"><i class="fas fa-filter"></i> فیلتر</button>
            <button class="tab-btn" data-panel="panel-punish"><i class="fas fa-gavel"></i> مجازات‌ها</button>
            <button class="tab-btn" data-panel="panel-remove"><i class="fas fa-trash-alt"></i> پاکسازی</button>
            <button class="tab-btn" data-panel="panel-add"><i class="fas fa-user-plus"></i> عضویت اجباری</button>
            <button class="tab-btn" data-panel="panel-game"><i class="fas fa-dice"></i> سرگرمی</button>
            <button class="tab-btn" data-panel="panel-utility"><i class="fas fa-tools"></i> کاربردی</button>
            <button class="tab-btn" data-panel="panel-list"><i class="fas fa-list"></i> لیست‌ها</button>
        </nav>

        <section id="panel-lock" class="panel active">
            <div class="panel-title"><i class="fas fa-lock"></i> قفل‌های گروه</div>
            <div class="panel-desc">با فعال‌سازی هر قفل، رفتار خاصی در گروه مدیریت می‌شود. کاربران عادی محدود شده و ادمین‌ها معاف هستند. برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="lockGrid"></div>
        </section>

        <section id="panel-set" class="panel">
            <div class="panel-title"><i class="fas fa-sliders-h"></i> تنظیمات گروه</div>
            <div class="panel-desc">تنظیمات پیشرفته مانند اخطار، خوش‌آمد، قوانین، گزارش و پیام تکراری. برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="setGrid"></div>
        </section>

        <section id="panel-filter" class="panel">
            <div class="panel-title"><i class="fas fa-filter"></i> فیلتر کلمات</div>
            <div class="panel-desc">ثبت فیلتر برای کلمات و پاسخ خودکار به آنها. برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="filterGrid"></div>
        </section>

        <section id="panel-punish" class="panel">
            <div class="panel-title"><i class="fas fa-gavel"></i> مجازات‌های کاربران</div>
            <div class="panel-desc">مجازات‌های قابل اعمال بر روی کاربران متخلف. برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="punishGrid"></div>
        </section>

        <section id="panel-remove" class="panel">
            <div class="panel-title"><i class="fas fa-trash-alt"></i> پاکسازی لیست‌ها</div>
            <div class="panel-desc">پاکسازی یک‌باره لیست‌های مختلف گروه. برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="removeGrid"></div>
        </section>

        <section id="panel-add" class="panel">
            <div class="panel-title"><i class="fas fa-user-plus"></i> عضویت اجباری</div>
            <div class="panel-desc">افزودن کانال یا گروه به عنوان شرط ارسال پیام. برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="addGrid"></div>
        </section>

        <section id="panel-game" class="panel">
            <div class="panel-title"><i class="fas fa-dice"></i> سرگرمی</div>
            <div class="panel-desc">بازی‌های دوز، گل یا پوچ و … برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="gameGrid"></div>
        </section>

        <section id="panel-utility" class="panel">
            <div class="panel-title"><i class="fas fa-tools"></i> دستورات کاربردی</div>
            <div class="panel-desc">دستورات مفید روزمره برای مدیریت گروه. برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="utilityGrid"></div>
        </section>

        <section id="panel-list" class="panel">
            <div class="panel-title"><i class="fas fa-list"></i> مشاهده لیست‌ها</div>
            <div class="panel-desc">مشاهده لیست ادمین‌ها، سکوت‌ها، اخطارها و … برای مشاهده توضیحات کامل و دستورات، روی هر گزینه کلیک کنید.</div>
            <div class="items-grid" id="listGrid"></div>
        </section>

        <div class="detail-view" id="detailView">
            <div class="detail-header">
                <button class="back-btn" id="backToPanel"><i class="fas fa-arrow-right"></i> بازگشت</button>
                <div class="detail-title"><i class="fas fa-info-circle" id="detailIcon"></i> <span id="detailTitle">عنوان</span></div>
            </div>
            <div class="detail-description" id="detailDescription">توضیحات کامل این بخش در اینجا نمایش داده می‌شود.</div>
            <div class="detail-commands" id="detailCommands"></div>
        </div>

        <footer style="margin-top: 30px; text-align: center; color: var(--text-light); font-size: 13px; border-top: 1px solid rgba(59,130,246,0.08); padding-top: 16px;">
            <i class="fas fa-heart" style="color: var(--primary);"></i> ساخته شده با عشق توسط تیم MAMPY
        </footer>
    </div>

    <script>
        const SECTION_DATA = {
            lock: {
                items: [
                    { 
                        id: 'badwords', 
                        icon: 'fa-ban', 
                        title: 'قفل فحش',
                        description: '🔞 با فعال کردن این قفل، ربات به‌صورت خودکار پیام‌های حاوی کلمات رکیک و نامناسب را تشخیص داده و سریعاً از گروه حذف می‌کند تا نظم گروه حفظ شود. کاربران عادی نمی‌توانند فحش ارسال کنند، اما ادمین‌ها معاف هستند.',
                        commands: [
                            { cmd: '.قفل فحش', desc: 'فعال‌سازی قفل فحش' },
                            { cmd: '.باز کردن فحش', desc: 'غیرفعال‌سازی قفل فحش' }
                        ]
                    },
                    { 
                        id: 'links', 
                        icon: 'fa-link', 
                        title: 'قفل لینک',
                        description: '🔗 با فعال کردن این قفل، ارسال هرگونه لینک (شامل http، https، t.me، ble.ir و ...) برای کاربران عادی ممنوع شده و پیام حذف می‌شود. این قفل برای جلوگیری از تبلیغات و هرزنامه بسیار کاربردی است.',
                        commands: [
                            { cmd: '.قفل لینک', desc: 'فعال‌سازی قفل لینک' },
                            { cmd: '.باز کردن لینک', desc: 'غیرفعال‌سازی قفل لینک' }
                        ]
                    },
                    { 
                        id: 'espem', 
                        icon: 'fa-comment-slash', 
                        title: 'ضد اسپم',
                        description: '⚡ این سیستم کاربرانی را که پیام‌های تکراری و پشت سر هم ارسال می‌کنند (اسپم) شناسایی کرده و از ارسال پیام مسدود می‌کند. با فعال‌سازی این قفل، نظم گروه حفظ می‌شود.',
                        commands: [
                            { cmd: '.قفل اسپم', desc: 'فعال‌سازی ضد اسپم' },
                            { cmd: '.باز کردن اسپم', desc: 'غیرفعال‌سازی ضد اسپم' }
                        ]
                    },
                    { 
                        id: 'codehang', 
                        icon: 'fa-code', 
                        title: 'قفل کدهنگی',
                        description: '🔢 این قفل برای جلوگیری از ارسال کدهای زبان برنامه‌نویسی یا متون خاص طراحی شده است. پیام‌های با طول بیش از ۶۰۰ کاراکتر به‌عنوان کدهنگی شناسایی و حذف می‌شوند.',
                        commands: [
                            { cmd: '.قفل کدهنگی', desc: 'فعال‌سازی قفل کدهنگی' },
                            { cmd: '.باز کردن کدهنگی', desc: 'غیرفعال‌سازی قفل کدهنگی' }
                        ]
                    },
                    { 
                        id: 'forward', 
                        icon: 'fa-forward', 
                        title: 'قفل فوروارد',
                        description: '✉️ جلوگیری از ارسال پیام‌های فوروارد شده از سایر کانال‌ها یا گروه‌ها. این قفل برای جلوگیری از تبلیغات و اسپم بسیار کاربردی است و فقط ادمین‌ها می‌توانند فوروارد کنند.',
                        commands: [
                            { cmd: '.قفل فوروارد', desc: 'فعال‌سازی قفل فوروارد' },
                            { cmd: '.باز کردن فوروارد', desc: 'غیرفعال‌سازی قفل فوروارد' }
                        ]
                    },
                    { 
                        id: 'reply', 
                        icon: 'fa-reply', 
                        title: 'قفل ریپلای',
                        description: '↩️ با فعال‌سازی این قفل، کاربران عادی نمی‌توانند روی پیام‌های دیگران پاسخ (ریپلای) دهند و فقط ادمین‌ها این امکان را دارند. برای مدیریت چت‌های شلوغ مناسب است.',
                        commands: [
                            { cmd: '.قفل ریپلای', desc: 'فعال‌سازی قفل ریپلای' },
                            { cmd: '.باز کردن ریپلای', desc: 'غیرفعال‌سازی قفل ریپلای' }
                        ]
                    },
                    { 
                        id: 'hashtagh', 
                        icon: 'fa-hashtag', 
                        title: 'قفل هشتگ',
                        description: '#️⃣ جلوگیری از ارسال متنی که شامل هشتگ (#) می‌باشد. این قفل برای مدیریت چت‌های شلوغ و جلوگیری از هرزنامه مفید است.',
                        commands: [
                            { cmd: '.قفل هشتگ', desc: 'فعال‌سازی قفل هشتگ' },
                            { cmd: '.باز کردن هشتگ', desc: 'غیرفعال‌سازی قفل هشتگ' }
                        ]
                    },
                    { 
                        id: 'cammand', 
                        icon: 'fa-terminal', 
                        title: 'قفل کامند',
                        description: '⌨️ ممانعت از ارسال دستورات (اسلش کامندها) که با علامت `/` شروع می‌شوند. این قفل دسترسی به ربات‌های دیگر را محدود می‌کند و فقط ادمین‌ها می‌توانند کامند ارسال کنند.',
                        commands: [
                            { cmd: '.قفل کامند', desc: 'فعال‌سازی قفل کامند' },
                            { cmd: '.باز کردن کامند', desc: 'غیرفعال‌سازی قفل کامند' }
                        ]
                    },
                    { 
                        id: 'english', 
                        icon: 'fa-language', 
                        title: 'قفل انگلیسی',
                        description: '🔡 این قفل ارسال هرگونه متنی که حروف انگلیسی یا اعداد انگلیسی داشته باشد را ممنوع می‌کند و فقط متن فارسی مجاز است. برای گروه‌های فارسی‌زبان بسیار مفید است.',
                        commands: [
                            { cmd: '.قفل انگلیسی', desc: 'فعال‌سازی قفل انگلیسی' },
                            { cmd: '.باز کردن انگلیسی', desc: 'غیرفعال‌سازی قفل انگلیسی' }
                        ]
                    },
                    { 
                        id: 'fa', 
                        icon: 'fa-language', 
                        title: 'قفل فارسی',
                        description: '🛡️ برعکس قفل انگلیسی، این قفل فقط اجازه ارسال متن انگلیسی را می‌دهد و ارسال حروف فارسی را برای کاربران ممنوع می‌کند. برای گروه‌های بین‌المللی مناسب است.',
                        commands: [
                            { cmd: '.قفل فارسی', desc: 'فعال‌سازی قفل فارسی' },
                            { cmd: '.باز کردن فارسی', desc: 'غیرفعال‌سازی قفل فارسی' }
                        ]
                    },
                    { 
                        id: 'group', 
                        icon: 'fa-users-slash', 
                        title: 'قفل گروه',
                        description: '🔒 با فعال کردن این قفل، تمامی پیام‌های کاربران عادی به محض ارسال حذف می‌شوند و فقط ادمین‌ها می‌توانند پیام ارسال کنند (گروه فقط خواندنی برای کاربران).',
                        commands: [
                            { cmd: '.قفل گروه', desc: 'فعال‌سازی قفل گروه' },
                            { cmd: '.باز کردن گروه', desc: 'غیرفعال‌سازی قفل گروه' }
                        ]
                    },
                    { 
                        id: 'photo', 
                        icon: 'fa-image', 
                        title: 'قفل عکس',
                        description: '🖼️ جلوگیری از ارسال تصاویر و عکس‌ها در گروه. برای گروه‌های متنی که تمایل به ارسال عکس ندارند مناسب است.',
                        commands: [
                            { cmd: '.قفل عکس', desc: 'فعال‌سازی قفل عکس' },
                            { cmd: '.باز کردن عکس', desc: 'غیرفعال‌سازی قفل عکس' }
                        ]
                    },
                    { 
                        id: 'video', 
                        icon: 'fa-video', 
                        title: 'قفل فیلم',
                        description: '🎥 ممانعت از ارسال ویدیو و کلیپ در گروه. این قفل حجم مصرفی اینترنت گروه را کاهش داده و نظم را حفظ می‌کند.',
                        commands: [
                            { cmd: '.قفل فیلم', desc: 'فعال‌سازی قفل فیلم' },
                            { cmd: '.باز کردن فیلم', desc: 'غیرفعال‌سازی قفل فیلم' }
                        ]
                    },
                    { 
                        id: 'music', 
                        icon: 'fa-music', 
                        title: 'قفل موسیقی',
                        description: '🎵 جلوگیری از ارسال فایل‌های موسیقی (MP3 و …) در گروه. اگر گروه شما متنی است، این قفل باعث نظم بیشتر می‌شود.',
                        commands: [
                            { cmd: '.قفل موسیقی', desc: 'فعال‌سازی قفل موسیقی' },
                            { cmd: '.باز کردن موسیقی', desc: 'غیرفعال‌سازی قفل موسیقی' }
                        ]
                    },
                    { 
                        id: 'voice', 
                        icon: 'fa-microphone', 
                        title: 'قفل ویس',
                        description: '🎤 منع ارسال پیام‌های صوتی (ویس). این قفل کاربران را مجبور به تایپ متن می‌کند و خواندن تاریخچه چت را آسان‌تر می‌کند.',
                        commands: [
                            { cmd: '.قفل ویس', desc: 'فعال‌سازی قفل ویس' },
                            { cmd: '.باز کردن ویس', desc: 'غیرفعال‌سازی قفل ویس' }
                        ]
                    },
                    { 
                        id: 'location', 
                        icon: 'fa-map-pin', 
                        title: 'قفل مکان',
                        description: '📍 جلوگیری از ارسال موقعیت مکانی و نقشه در گروه. این قفل برای حفظ حریم خصوصی و جلوگیری از اسپم کاربرد دارد.',
                        commands: [
                            { cmd: '.قفل مکان', desc: 'فعال‌سازی قفل مکان' },
                            { cmd: '.باز کردن مکان', desc: 'غیرفعال‌سازی قفل مکان' }
                        ]
                    },
                    { 
                        id: 'file', 
                        icon: 'fa-file', 
                        title: 'قفل فایل',
                        description: '📁 ممانعت از ارسال هرگونه فایل مستند (PDF، ZIP و ...) در گروه. این قفل برای جلوگیری از انتشار فایل‌های مخرب یا نامربوط است.',
                        commands: [
                            { cmd: '.قفل فایل', desc: 'فعال‌سازی قفل فایل' },
                            { cmd: '.باز کردن فایل', desc: 'غیرفعال‌سازی قفل فایل' }
                        ]
                    },
                    { 
                        id: 'contact', 
                        icon: 'fa-address-book', 
                        title: 'قفل مخاطب',
                        description: '👤 جلوگیری از ارسال شماره تماس و اطلاعات مخاطبین در گروه. این قفل از انتشار شماره‌های شخصی جلوگیری می‌کند.',
                        commands: [
                            { cmd: '.قفل مخاطب', desc: 'فعال‌سازی قفل مخاطب' },
                            { cmd: '.باز کردن مخاطب', desc: 'غیرفعال‌سازی قفل مخاطب' }
                        ]
                    },
                    { 
                        id: 'name', 
                        icon: 'fa-user-slash', 
                        title: 'قفل نام ناپسند',
                        description: '📛 این قفل پیام کاربرانی که نام آنها حاوی کلمات ناپسند است را پاک می‌کند و هیچ پیامی ارسال نمی‌کند. برای حفظ ادب در گروه بسیار مفید است.',
                        commands: [
                            { cmd: '.قفل نام', desc: 'فعال‌سازی قفل نام ناپسند' },
                            { cmd: '.باز کردن نام', desc: 'غیرفعال‌سازی قفل نام ناپسند' }
                        ]
                    },
                    { 
                        id: 'nezam', 
                        icon: 'fa-gem', 
                        title: 'قفل حکومت نظامی',
                        description: '🫡 با فعال کردن این قفل، تمامی قفل‌های مهم (فحش، لینک، اسپم، هشتگ، کامند، فوروارد، عکس، فیلم، موسیقی، ویس، مکان، فایل، مخاطب، انگلیسی، کدهنگی) یکجا فعال می‌شوند. برای مواقع ضروری بسیار کارآمد است.',
                        commands: [
                            { cmd: '.قفل حکومت نظامی', desc: 'فعال‌سازی همه قفل‌ها' },
                            { cmd: '.باز کردن حکومت نظامی', desc: 'غیرفعال‌سازی همه قفل‌ها' }
                        ]
                    },
                    { 
                        id: 'carackter', 
                        icon: 'fa-font', 
                        title: 'قفل کاراکتر',
                        description: '⛔ با فعال کردن این قفل و تنظیم کاراکتر مجاز، پیام هر کاربری که تعداد کاراکترهایش بیشتر از حد مجاز باشد را حذف می‌کند. تعداد کاراکتر مجاز را خودتان تعیین می‌کنید.',
                        commands: [
                            { cmd: '.قفل کاراکتر [تعداد]', desc: 'فعال‌سازی با تعیین تعداد کاراکتر مجاز' },
                            { cmd: '.باز کردن کاراکتر', desc: 'غیرفعال‌سازی قفل کاراکتر' }
                        ]
                    }
                ]
            },
            set: {
                items: [
                    { 
                        id: 'warn', 
                        icon: 'fa-exclamation-triangle', 
                        title: 'تنظیم سقف اخطار',
                        description: '⚠️ با تنظیم کردن حداکثر اخطار مجاز، زمانی که کاربر به سقف مجازات می‌رسد، مجازات تنظیم شده روی کاربر اعمال می‌شود. نوع مجازات می‌تواند بن، ریم یا سکوت باشد.',
                        commands: [
                            { cmd: '.تنظیم [تعداد] اخطار [مجازات]', desc: 'مثال: .تنظیم 5 اخطار سکوت' }
                        ]
                    },
                    { 
                        id: 'mojazat', 
                        icon: 'fa-gavel', 
                        title: 'تنظیم مجازات کاربران',
                        description: '🚫 با تنظیم کردن مجازات در گروه، می‌توانید تعیین کنید که اگر کاربری پیام ممنوعه فرستاد، چه مجازاتی داشته باشد. نوع مجازات می‌تواند بن، ریم، سکوت، اخطار یا تذکر باشد.',
                        commands: [
                            { cmd: '.مجازات [نوع پیام] [مجازات]', desc: 'مثال: .مجازات فحش اخطار' }
                        ]
                    },
                    { 
                        id: 'autolock', 
                        icon: 'fa-clock', 
                        title: 'قفل خودکار گروه',
                        description: '🔐 با این قفل می‌توانید گروه را در یک زمان مشخص قفل و در زمان مشخص باز کنید. در زمان قفل، کاربران عادی اجازه ارسال پیام را ندارند. فرمت زمان: ساعت:دقیقه',
                        commands: [
                            { cmd: '.قفل خودکار گروه [شروع]-[پایان]', desc: 'مثال: .قفل خودکار گروه 23:30-7:00' },
                            { cmd: '.بازکردن قفل خودکار گروه', desc: 'غیرفعال‌سازی قفل خودکار' }
                        ]
                    },
                    { 
                        id: 'log', 
                        icon: 'fa-paper-plane', 
                        title: 'تنظیم گروه گزارش',
                        description: '📝 با تنظیم گروه گزارش، فعالیت‌های ادمین‌های گروه اصلی مانند ریم، بن، سکوت و ... به صورت خلاصه به گروه موردنظر ارسال می‌شود. ابتدا ربات را در گروه مقصد نصب کنید و شناسه آن را با دستور "چت" دریافت کنید.',
                        commands: [
                            { cmd: '.ارسال گزارش [شناسه]', desc: 'تنظیم گروه گزارش' },
                            { cmd: '.حذف گروه گزارش', desc: 'حذف گروه گزارش' }
                        ]
                    },
                    { 
                        id: 'wellcome', 
                        icon: 'fa-smile', 
                        title: 'تنظیم خوش‌آمد',
                        description: '😊 زمانی که متن خوش‌آمد را تنظیم می‌کنید، هر کاربری که به تازگی عضو گروه شود، تشخیص داده می‌شود و متن خوش‌آمد ارسال می‌شود. متغیرهای مجاز: [name]، [time]، [title]',
                        commands: [
                            { cmd: '.تنظیم خوش آمد [متن]', desc: 'تنظیم متن خوش‌آمد' }
                        ]
                    },
                    { 
                        id: 'rulse', 
                        icon: 'fa-book', 
                        title: 'تنظیم قوانین',
                        description: '🔰 زمانی که قوانین را تنظیم می‌کنید، کاربران می‌توانند قوانین را با ارسال دستور .قوانین مشاهده کنند. برای تنظیم، روی پیام موردنظر ریپلای بزنید.',
                        commands: [
                            { cmd: '.تنظیم قوانین (ریپلای)', desc: 'تنظیم قوانین گروه' },
                            { cmd: '.حذف قوانین', desc: 'حذف قوانین گروه' }
                        ]
                    },
                    { 
                        id: 'about', 
                        icon: 'fa-id-card', 
                        title: 'ثبت اصل',
                        description: '👤 ثبت کردن اصل کاربر موردنظر در اطلاعات گروه. این دستورات با ریپلای زدن روی کاربر موردنظر انجام می‌شود.',
                        commands: [
                            { cmd: '.ثبت اصل (ریپلای)', desc: 'ثبت اصل برای کاربر' },
                            { cmd: '.حذف اصل (ریپلای)', desc: 'حذف اصل کاربر' }
                        ]
                    },
                    { 
                        id: 'fohsh', 
                        icon: 'fa-skull', 
                        title: 'ثبت فحش',
                        description: '🚫 با ثبت کردن فحش موردنظر، ارسال آن فحش در گروه ممنوع می‌شود. می‌توانید کلمات جدید را به لیست فحش‌ها اضافه یا حذف کنید.',
                        commands: [
                            { cmd: '.ثبت فحش [کلمه]', desc: 'افزودن فحش جدید' },
                            { cmd: '.حذف فحش [کلمه]', desc: 'حذف فحش از لیست' }
                        ]
                    },
                    { 
                        id: 'everytext', 
                        icon: 'fa-sync-alt', 
                        title: 'پیام تکراری',
                        description: '💬 با ثبت پیام تکراری، پیام موردنظر با توجه به فاصله زمانی در گروه ارسال می‌شود. فرمت زمان به دقیقه می‌باشد. روی پیام موردنظر ریپلای بزنید.',
                        commands: [
                            { cmd: '.پیام تکراری [دقیقه] (ریپلای)', desc: 'تنظیم پیام تکراری' },
                            { cmd: '.حذف پیام تکراری', desc: 'حذف پیام تکراری' }
                        ]
                    }
                ]
            },
            filter: {
                items: [
                    { 
                        id: 'setfilter', 
                        icon: 'fa-plus-circle', 
                        title: 'افزودن فیلتر',
                        description: '📋 با افزودن فیلتر بر یک کلمه یا جمله، می‌توانید برای آن جمله یک جواب مشخص قرار دهید. روی پیام حاوی کلید (کلمه موردنظر) ریپلای بزنید و پاسخ را تعیین کنید.',
                        commands: [
                            { cmd: '.ثبت فیلتر [پاسخ] (ریپلای روی کلید)', desc: 'افزودن فیلتر جدید' }
                        ]
                    },
                    { 
                        id: 'delfilter', 
                        icon: 'fa-minus-circle', 
                        title: 'حذف فیلتر',
                        description: '📋 با حذف کردن یک فیلتر، می‌توانید جواب آن فیلتر را از اطلاعات گروه حذف کنید.',
                        commands: [
                            { cmd: '.حذف فیلتر [کلید]', desc: 'حذف فیلتر' }
                        ]
                    },
                    { 
                        id: 'seefilter', 
                        icon: 'fa-list', 
                        title: 'مشاهده لیست فیلتر',
                        description: '📋 با این دستور می‌توانید تمام فیلترهای ثبت شده را مشاهده کنید.',
                        commands: [
                            { cmd: '.لیست فیلترها', desc: 'مشاهده همه فیلترها' }
                        ]
                    }
                ]
            },
            punish: {
                items: [
                    { 
                        id: 'ban', 
                        icon: 'fa-user-slash', 
                        title: 'بن',
                        description: '⭕ زمانی که یک کاربر بن می‌شود، امکان ورود دوباره به گروه را ندارد. برای بن کردن می‌توانید روی کاربر ریپلای بزنید یا آیدی او را وارد کنید.',
                        commands: [
                            { cmd: '.بن (ریپلای)', desc: 'بن کردن کاربر موردنظر' },
                            { cmd: '.بن [آیدی]', desc: 'بن کردن کاربر با آیدی' }
                        ]
                    },
                    { 
                        id: 'rim', 
                        icon: 'fa-user-minus', 
                        title: 'ریم',
                        description: '⚠️ زمانی که یک کاربر ریم می‌شود، از گروه اخراج می‌شود اما امکان بازگشت دوباره به گروه را دارد.',
                        commands: [
                            { cmd: '.ریم (ریپلای)', desc: 'ریم کردن کاربر موردنظر' },
                            { cmd: '.ریم [آیدی]', desc: 'ریم کردن کاربر با آیدی' }
                        ]
                    },
                    { 
                        id: 'banplus', 
                        icon: 'fa-user-slash', 
                        title: 'بن پلاس',
                        description: '⭕ زمانی که یک کاربر بن پلاس می‌شود، پیام موفقیت بن ارسال نمی‌شود و پیام ادمین نیز پاک می‌شود. کاملاً مخفیانه.',
                        commands: [
                            { cmd: '.بن پلاس (ریپلای)', desc: 'بن پلاس کاربر' }
                        ]
                    },
                    { 
                        id: 'rimplus', 
                        icon: 'fa-user-minus', 
                        title: 'ریم پلاس',
                        description: '⚠️ زمانی که یک کاربر ریم پلاس می‌شود، پیام موفقیت ریم ارسال نمی‌شود و پیام ادمین نیز پاک می‌شود. کاملاً مخفیانه.',
                        commands: [
                            { cmd: '.ریم پلاس (ریپلای)', desc: 'ریم پلاس کاربر' }
                        ]
                    },
                    { 
                        id: 'warn', 
                        icon: 'fa-exclamation', 
                        title: 'اخطار',
                        description: '⚠️ ادمین می‌تواند به صورت دستی به کاربر اخطار دهد. همچنین می‌تواند اخطارهای کاربر را حذف کند یا همه اخطارها را پاک کند.',
                        commands: [
                            { cmd: '.اخطار (ریپلای)', desc: 'افزودن اخطار به کاربر' },
                            { cmd: '.حذف اخطار (ریپلای)', desc: 'کاهش یک اخطار' },
                            { cmd: '.حذف اخطارها (ریپلای)', desc: 'حذف همه اخطارهای کاربر' }
                        ]
                    },
                    { 
                        id: 'meut', 
                        icon: 'fa-microphone-slash', 
                        title: 'سکوت',
                        description: '🔇 زمانی که یک کاربر سکوت می‌شود، امکان ارسال پیام در گروه را ندارد. می‌توانید با ریپلای یا با آیدی کاربر او را سکوت کنید.',
                        commands: [
                            { cmd: '.سکوت (ریپلای)', desc: 'سکوت کاربر' },
                            { cmd: '.حذف سکوت (ریپلای)', desc: 'رفع سکوت کاربر' },
                            { cmd: '.سکوت کاربر [آیدی]', desc: 'سکوت با آیدی' },
                            { cmd: '.حذف سکوت کاربر [آیدی]', desc: 'رفع سکوت با آیدی' }
                        ]
                    },
                    { 
                        id: 'meuttime', 
                        icon: 'fa-clock', 
                        title: 'سکوت زمان‌دار',
                        description: '🔇 زمانی که ادمین یک نفر را برای زمان مشخصی سکوت می‌کند، فرد موردنظر تا پایان زمان تعیین شده، سکوت می‌ماند. فرمت زمان به دقیقه می‌باشد.',
                        commands: [
                            { cmd: '.سکوت [دقیقه] (ریپلای)', desc: 'سکوت زمان‌دار' },
                            { cmd: '.حذف سکوت (ریپلای)', desc: 'رفع سکوت' }
                        ]
                    },
                    { 
                        id: 'rulseadmin', 
                        icon: 'fa-user-cog', 
                        title: 'تغییر مجوز کاربران',
                        description: '⭕ با این دستور می‌توانید مجوزهای کاربر را از طریق ربات تغییر دهید. دسترسی‌هایی مانند ارسال پیام، ارسال رسانه، افزودن عضو و ... را مدیریت کنید.',
                        commands: [
                            { cmd: '.دسترسی (ریپلای)', desc: 'مدیریت دسترسی‌های کاربر' },
                            { cmd: '.دسترسی [آیدی]', desc: 'مدیریت دسترسی با آیدی' }
                        ]
                    },
                    { 
                        id: 'unban', 
                        icon: 'fa-undo', 
                        title: 'رفع بن',
                        description: '⭕ با این دستور می‌توانید کاربر موردنظر را از لیست حذف شدگان دربیاورید و اجازه ورود مجدد به گروه را بدهید.',
                        commands: [
                            { cmd: '.حذف بن [آیدی]', desc: 'رفع بن کاربر' }
                        ]
                    }
                ]
            },
            remove: {
                items: [
                    { id: 'removefilter', icon: 'fa-filter', title: 'پاکسازی لیست فیلتر', description: '🧹 حذف تمام فیلترهای ثبت‌شده در گروه.', commands: [{ cmd: '.پاکسازی لیست فیلتر', desc: 'حذف همه فیلترها' }] },
                    { id: 'removebad', icon: 'fa-skull', title: 'پاکسازی لیست فحش', description: '🧹 حذف تمام کلمات فحش ثبت‌شده در گروه.', commands: [{ cmd: '.پاکسازی لیست فحش', desc: 'حذف همه فحش‌ها' }] },
                    { id: 'removemoaf', icon: 'fa-user-check', title: 'پاکسازی لیست معاف', description: '🧹 حذف همه کاربران معاف از عضویت اجباری.', commands: [{ cmd: '.پاکسازی لیست معاف', desc: 'حذف همه معاف‌ها' }] },
                    { id: 'removeadd', icon: 'fa-user-plus', title: 'پاکسازی لیست عضویت اجباری', description: '🧹 حذف همه کانال‌های اجباری از لیست.', commands: [{ cmd: '.پاکسازی لیست عضویت اجباری', desc: 'حذف همه عضویت‌های اجباری' }] },
                    { id: 'removestats', icon: 'fa-chart-bar', title: 'پاکسازی لیست آمار', description: '🧹 بازنشانی آمار گروه (تعداد پیام‌ها، کاربران و ...).', commands: [{ cmd: '.پاکسازی لیست آمار', desc: 'حذف آمار گروه' }] },
                    { id: 'removemute', icon: 'fa-microphone-slash', title: 'پاکسازی لیست سکوت', description: '🧹 رفع سکوت همه کاربران و پاکسازی لیست سکوت.', commands: [{ cmd: '.پاکسازی لیست سکوت', desc: 'رفع سکوت همه' }] },
                    { id: 'removewarn', icon: 'fa-exclamation', title: 'پاکسازی لیست اخطار', description: '🧹 حذف اخطار همه کاربران و پاکسازی لیست اخطار.', commands: [{ cmd: '.پاکسازی لیست اخطار', desc: 'حذف اخطار همه' }] },
                    { id: 'removeabout', icon: 'fa-id-card', title: 'پاکسازی لیست اصل', description: '🧹 حذف همه اصل‌های ثبت‌شده برای کاربران.', commands: [{ cmd: '.پاکسازی لیست اصل', desc: 'حذف همه اصل‌ها' }] }
                ]
            },
            add: {
                items: [
                    { id: 'addforce', icon: 'fa-plus-circle', title: 'افزودن عضویت اجباری', description: '🚷 با این دستور می‌توانید برای کاربران عضویت اجباری بگذارید. کاربران برای ارسال پیام باید در کانال/گروه موردنظر عضو باشند. آیدی گروه را با دستور "چت" دریافت کنید.', commands: [{ cmd: '.عضویت اجباری [آیدی]', desc: 'افزودن عضویت اجباری' }] },
                    { id: 'removeforce', icon: 'fa-minus-circle', title: 'حذف عضویت اجباری', description: '🚷 با این دستور می‌توانید کانال/گروه موردنظر را از لیست عضویت اجباری حذف کنید.', commands: [{ cmd: '.حذف عضویت اجباری [آیدی]', desc: 'حذف عضویت اجباری' }] },
                    { id: 'seeforce', icon: 'fa-list', title: 'لیست عضویت اجباری', description: '📋 با این دستور می‌توانید لیست کانال‌هایی که جوین در آنها اجباری است را مشاهده کنید.', commands: [{ cmd: '.لیست عضویت اجباری', desc: 'مشاهده لیست' }] }
                ]
            },
            game: {
                items: [
                    { id: 'doz', icon: 'fa-times', title: 'دوز', description: '👾 با این دستور ادمین‌ها می‌توانند بازی دوز را استارت کنند. دو بازیکن می‌توانند به بازی بپیوندند و بازی شروع می‌شود.', commands: [{ cmd: '.دوز', desc: 'شروع بازی دوز' }, { cmd: '.بستن بازی‌ها', desc: 'بستن همه بازی‌ها' }] },
                    { id: 'ghool', icon: 'fa-circle', title: 'گل یا پوچ', description: '👾 با این دستور، ادمین‌ها می‌توانند بازی گل یا پوچ را استارت کنند. یک بازیکن گل را مخفی می‌کند و دیگری حدس می‌زند.', commands: [{ cmd: '.گل یا پوچ', desc: 'شروع بازی گل یا پوچ' }, { cmd: '.بستن بازی‌ها', desc: 'بستن همه بازی‌ها' }] }
                ]
            },
            utility: {
                items: [
                    { id: 'nerkh', icon: 'fa-coins', title: 'نرخ ارز', description: '💸 با این دستور، می‌توانید از آخرین قیمت ارزهای موجود (دلار، یورو، درهم، پوند، تتر، بیت‌کوین) مطلع شوید.', commands: [{ cmd: '.نرخ ارز', desc: 'مشاهده قیمت ارزها' }] },
                    { id: 'delete', icon: 'fa-eraser', title: 'پاک کردن پیام', description: '🧹 با این دستور می‌توانید تعداد مشخصی پیام از گروه را پاک کنید. حداکثر ۱۰۰ پیام در هر بار.', commands: [{ cmd: '.پاک کردن [تعداد] پیام', desc: 'مثال: .پاک کردن 50 پیام' }] },
                    { id: 'unknown', icon: 'fa-user-secret', title: 'پیام ناشناس', description: '😶‍🌫️ با این دستور می‌توانید برای کاربر موردنظر خود در گروه، پیام ناشناس ارسال کنید. روی کاربر ریپلای بزنید.', commands: [{ cmd: '.پیام ناشناس (ریپلای)', desc: 'ارسال پیام ناشناس' }] },
                    { id: 'help', icon: 'fa-life-ring', title: 'درخواست کمک', description: '🔰 با ارسال این دستور، تیم پشتیبانی برای کمک به شما و آشنا کردن شما با دستورات ربات، به گروه مراجعه خواهند کرد.', commands: [{ cmd: '.کمک', desc: 'ارسال درخواست کمک' }] },
                    { id: 'amamr', icon: 'fa-chart-pie', title: 'آمار گروه', description: '📊 با این دستور می‌توانید آمار کاربران گروه، تعداد پیام‌ها، کاربران فعال و ... را مشاهده کنید.', commands: [{ cmd: '.آمار', desc: 'مشاهده آمار گروه' }] },
                    { id: 'salavat', icon: 'fa-pray', title: 'صلوات', description: '📿 با این دستور ربات در گروه صلوات ارسال می‌کند.', commands: [{ cmd: '.صلوات', desc: 'ارسال صلوات' }] },
                    { id: 'hadis', icon: 'fa-book', title: 'حدیث', description: '📜 با این دستور، ربات به صورت تصادفی، یک حدیث ارسال می‌کند.', commands: [{ cmd: '.حدیث', desc: 'ارسال حدیث تصادفی' }] },
                    { id: 'jock', icon: 'fa-laugh', title: 'جوک', description: '🎭 با این دستور، ربات به صورت تصادفی، یک جوک ارسال می‌کند.', commands: [{ cmd: '.جوک', desc: 'ارسال جوک تصادفی' }] },
                    { id: 'hosh', icon: 'fa-brain', title: 'هوش مصنوعی', description: '🤖 با این دستور می‌توانید هر سوالی را رایگان از هوش مصنوعی ربات بپرسید.', commands: [{ cmd: '.هوش [سوال]', desc: 'پرسش از هوش مصنوعی' }] },
                    { id: 'link', icon: 'fa-link', title: 'لینک', description: '📌 با این دستور می‌توانید لینک خصوصی گروه را دریافت کنید.', commands: [{ cmd: '.لینک', desc: 'دریافت لینک گروه' }] },
                    { id: 'ping', icon: 'fa-tachometer-alt', title: 'پینگ', description: '🏓 با این دستور می‌توانید سرعت پاسخگویی ربات را مشاهده کنید.', commands: [{ cmd: '.پینگ', desc: 'بررسی سرعت ربات' }] },
                    { id: 'changename', icon: 'fa-edit', title: 'تغییر نام', description: '👾 با این دستور می‌توانید نام گروه را تغییر دهید.', commands: [{ cmd: '.تغییر نام [نام جدید]', desc: 'تغییر نام گروه' }] },
                    { id: 'changebio', icon: 'fa-edit', title: 'تغییر توضیحات', description: '🔹 با این دستور می‌توانید توضیحات گروه را تغییر دهید.', commands: [{ cmd: '.تغییر توضیحات [متن]', desc: 'تغییر توضیحات گروه' }] },
                    { id: 'admin', icon: 'fa-user-cog', title: 'دستورات ادمین', description: '🙎‍♂️ دستورات زیر برای مدیریت ادمین‌های گروه توسط مالک است.', commands: [{ cmd: '.ترفیع (ریپلای)', desc: 'ترفیع کاربر به ادمین' }, { cmd: '.عزل (ریپلای)', desc: 'عزل ادمین' }, { cmd: '.تگ کردن ادمین', desc: 'تگ کردن ادمین‌ها' }, { cmd: '.لیست ادمین', desc: 'مشاهده لیست ادمین‌ها' }] },
                    { id: 'pin', icon: 'fa-thumbtack', title: 'پین کردن', description: '📌 با این دستورات می‌توانید پیام‌های سنجاق شده را مدیریت کنید.', commands: [{ cmd: '.پین (ریپلای)', desc: 'سنجاق کردن پیام' }, { cmd: '.حذف پین (ریپلای)', desc: 'برداشتن سنجاق' }, { cmd: '.حذف پین‌ها', desc: 'برداشتن همه سنجاق‌ها' }] },
                    { id: 'panel', icon: 'fa-sliders-h', title: 'تنظیمات (پنل)', description: '⚙️ با این دستور می‌توانید پنل مختصر تنظیمات و قفل‌های گروه را مشاهده کنید.', commands: [{ cmd: '.تنظیمات', desc: 'مشاهده پنل تنظیمات' }, { cmd: '.پنل', desc: 'مشاهده پنل گروه' }] },
                    { id: 'aboutyou', icon: 'fa-user', title: 'اطلاعات کاربر', description: '👤 با این دستور، می‌توانید اطلاعات شخص مورد نظر (نام، آیدی، وضعیت، تعداد پیام) را مشاهده کنید. روی کاربر ریپلای بزنید.', commands: [{ cmd: '.اطلاعات (ریپلای)', desc: 'مشاهده اطلاعات کاربر' }] },
                    { id: 'aboutme', icon: 'fa-user-circle', title: 'اطلاعات من', description: '👤 با این دستور می‌توانید اطلاعات پروفایل خود را مشاهده کنید.', commands: [{ cmd: '.پروفایل', desc: 'مشاهده اطلاعات خود' }, { cmd: '.من', desc: 'مشاهده اطلاعات خود' }] },
                    { id: 'tarikh', icon: 'fa-calendar-alt', title: 'تاریخ و زمان', description: '⏰ با ارسال این دستور، از زمان و تاریخ (شمسی و میلادی) مطلع شوید.', commands: [{ cmd: '.تاریخ', desc: 'مشاهده تاریخ' }, { cmd: '.تایم', desc: 'مشاهده زمان' }, { cmd: '.زمان', desc: 'مشاهده زمان' }] },
                    { id: 'leave', icon: 'fa-sign-out-alt', title: 'خروج ربات از گروه', description: '🍂 با این دستورات، ربات گروه را ترک می‌کند. فقط مالک گروه مجاز به انجام این کار است.', commands: [{ cmd: '.مامپای سیکتو بزن', desc: 'خروج ربات' }, { cmd: '.مامپای سیکتیر', desc: 'خروج ربات' }, { cmd: '.مامپای برو', desc: 'خروج ربات' }] },
                    { id: 'goodbye', icon: 'fa-door-open', title: 'پیام ترک گروه', description: '👤 زمانی که کاربری گروه را ترک می‌کند، ربات اعلان ترک گروه را ارسال می‌کند و این اعلان را پس از ۳۰ ثانیه حذف می‌کند.', commands: [{ cmd: '.ترک گروه خاموش', desc: 'غیرفعال‌سازی اعلان ترک' }, { cmd: '.ترک گروه روشن', desc: 'فعال‌سازی اعلان ترک' }] },
                    { id: 'wellcomeuser', icon: 'fa-door-open', title: 'پیام خوش‌آمد', description: '🌱 زمانی که خوش‌آمدگویی فعال است، کاربری که عضو گروه می‌شود، پیام خوش‌آمدگویی برای کاربر ارسال می‌شود و پس از ۲ دقیقه حذف می‌شود.', commands: [{ cmd: '.خوش آمد روشن', desc: 'فعال‌سازی خوش‌آمد' }, { cmd: '.خوش آمد خاموش', desc: 'غیرفعال‌سازی خوش‌آمد' }] }
                ]
            },
            list: {
                items: [
                    { id: 'listmute', icon: 'fa-list', title: 'لیست سکوت', description: '📋 مشاهده لیست کاربران سکوت‌شده.', commands: [{ cmd: '.لیست سکوت', desc: 'مشاهده لیست سکوت' }] },
                    { id: 'listwarn', icon: 'fa-list', title: 'لیست اخطار', description: '📋 مشاهده لیست کاربران دارای اخطار.', commands: [{ cmd: '.لیست اخطار', desc: 'مشاهده لیست اخطار' }] },
                    { id: 'listadmin', icon: 'fa-list', title: 'لیست ادمین', description: '📋 مشاهده لیست ادمین‌های گروه.', commands: [{ cmd: '.لیست ادمین', desc: 'مشاهده لیست ادمین‌ها' }] },
                    { id: 'listfilter', icon: 'fa-list', title: 'لیست فیلتر', description: '📋 مشاهده لیست فیلترهای ثبت‌شده.', commands: [{ cmd: '.لیست فیلتر', desc: 'مشاهده لیست فیلترها' }] },
                    { id: 'listbad', icon: 'fa-list', title: 'لیست فحش‌ها', description: '📋 مشاهده لیست کلمات ممنوعه (فحش‌ها).', commands: [{ cmd: '.لیست فحش‌ها', desc: 'مشاهده لیست فحش‌ها' }] },
                    { id: 'listtarfi', icon: 'fa-list', title: 'لیست ترفیع', description: '📋 مشاهده لیست کاربران ترفیع‌گرفته.', commands: [{ cmd: '.لیست ترفیع', desc: 'مشاهده لیست ترفیع' }] },
                    { id: 'listmoaf', icon: 'fa-list', title: 'لیست معاف', description: '📋 مشاهده لیست کاربران معاف از عضویت اجباری.', commands: [{ cmd: '.لیست معاف', desc: 'مشاهده لیست معاف' }] },
                    { id: 'listabout', icon: 'fa-list', title: 'لیست اصل', description: '📋 مشاهده لیست اصل‌های ثبت‌شده برای کاربران.', commands: [{ cmd: '.لیست اصل', desc: 'مشاهده لیست اصل‌ها' }] }
                ]
            }
        };

        function renderItems(containerId, items) {
            const container = document.getElementById(containerId);
            if (!container) return;
            container.innerHTML = items.map(item => `
                <button class="item-btn" data-section="${containerId.replace('Grid','')}" data-id="${item.id}">
                    <div class="icon"><i class="fas ${item.icon}"></i></div>
                    <div class="info">
                        <h4>${item.title}</h4>
                        <p>${item.description.substring(0, 60)}...</p>
                    </div>
                </button>
            `).join('');
        }

        renderItems('lockGrid', SECTION_DATA.lock.items);
        renderItems('setGrid', SECTION_DATA.set.items);
        renderItems('filterGrid', SECTION_DATA.filter.items);
        renderItems('punishGrid', SECTION_DATA.punish.items);
        renderItems('removeGrid', SECTION_DATA.remove.items);
        renderItems('addGrid', SECTION_DATA.add.items);
        renderItems('gameGrid', SECTION_DATA.game.items);
        renderItems('utilityGrid', SECTION_DATA.utility.items);
        renderItems('listGrid', SECTION_DATA.list.items);
        const detailView = document.getElementById('detailView');
        const detailIcon = document.getElementById('detailIcon');
        const detailTitle = document.getElementById('detailTitle');
        const detailDescription = document.getElementById('detailDescription');
        const detailCommands = document.getElementById('detailCommands');
        const backBtn = document.getElementById('backToPanel');

        function showDetail(sectionKey, itemId) {
            document.querySelectorAll('.panel').forEach(p => p.classList.remove('active'));
            detailView.classList.add('active');
            const section = SECTION_DATA[sectionKey];
            if (!section) return;
            const item = section.items.find(i => i.id === itemId);
            if (!item) return;

            detailIcon.className = `fas ${item.icon}`;
            detailTitle.textContent = item.title;
            detailDescription.textContent = item.description;
            detailCommands.innerHTML = item.commands.map(cmd => `
                <div class="command-item">
                    <span class="cmd-badge">${cmd.cmd}</span>
                    <span class="cmd-desc">${cmd.desc}</span>
                </div>
            `).join('');
        }

        function backToPanel() {
            detailView.classList.remove('active');
            const activeTab = document.querySelector('.tab-btn.active');
            if (activeTab) {
                const panelId = activeTab.dataset.panel;
                const panel = document.getElementById(panelId);
                if (panel) panel.classList.add('active');
            }
        }

        document.querySelectorAll('.item-btn').forEach(btn => {
            btn.addEventListener('click', function() {
                const section = this.dataset.section;
                const id = this.dataset.id;
                showDetail(section, id);
            });
        });

        backBtn.addEventListener('click', backToPanel);
        const tabButtons = document.querySelectorAll('.tab-btn');
        const panels = {
            lock: document.getElementById('panel-lock'),
            set: document.getElementById('panel-set'),
            filter: document.getElementById('panel-filter'),
            punish: document.getElementById('panel-punish'),
            remove: document.getElementById('panel-remove'),
            add: document.getElementById('panel-add'),
            game: document.getElementById('panel-game'),
            utility: document.getElementById('panel-utility'),
            list: document.getElementById('panel-list'),
        };

        tabButtons.forEach(btn => {
            btn.addEventListener('click', function() {
                if (detailView.classList.contains('active')) {
                    detailView.classList.remove('active');
                }

                tabButtons.forEach(b => b.classList.remove('active'));
                this.classList.add('active');
                Object.values(panels).forEach(p => p.classList.remove('active'));
                const target = this.dataset.panel;
                const panelId = target.replace('panel-', '');
                if (panels[panelId]) {
                    panels[panelId].classList.add('active');
                }
            });
        });

        const themeToggle = document.getElementById('themeToggle');
        const icon = themeToggle.querySelector('i');

        if (localStorage.getItem('theme') === 'dark') {
            document.body.classList.add('dark');
            icon.className = 'fas fa-sun';
        }

        themeToggle.addEventListener('click', () => {
            document.body.classList.toggle('dark');
            const isDark = document.body.classList.contains('dark');
            localStorage.setItem('theme', isDark ? 'dark' : 'light');
            icon.className = isDark ? 'fas fa-sun' : 'fas fa-moon';
        });

    </script>
</body>
</html>
