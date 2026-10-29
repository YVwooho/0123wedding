#Wedding Invitation
#welcometoourwedding
<html lang="zh-TW" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calvin & Yvonne Wedding Invitation | 2027.01.23</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;0,700;1,400;1,600&family=Noto+Serif+TC:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        morandi: {
                            gold: '#d4a373',
                            'gold-light': '#f4ece1',
                            sage: '#8da399',
                            'sage-light': '#eaf0ed',
                            bg: '#fbf9f6',
                            text: '#2c3e35',
                            muted: '#7a8b83',
                            card: '#ffffff'
                        }
                    },
                    fontFamily: {
                        cormorant: ['"Cormorant Garamond"', 'serif'],
                        noto: ['"Noto Serif TC"', 'serif']
                    },
                    boxShadow: {
                        'glow': '0 10px 30px -5px rgba(212, 163, 115, 0.15), 0 4px 12px rgba(0, 0, 0, 0.03)',
                        'soft': '0 20px 40px -15px rgba(44, 62, 53, 0.07)'
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Noto Serif TC', 'Cormorant Garamond', serif;
            background-color: #fbf9f6;
            color: #2c3e35;
            overflow-x: hidden;
        }

        /* 避免手機版地點與捷運站自動斷行跑版 */
        .no-wrap {
            white-space: nowrap !important;
            word-break: keep-all !important;
        }

        /* 微光卡片樣式 */
        .glow-card {
            background: rgba(255, 255, 255, 0.92);
            backdrop-filter: blur(8px);
            border: 1px solid rgba(212, 163, 115, 0.25);
            box-shadow: 0 8px 32px 0 rgba(212, 163, 115, 0.12), inset 0 0 12px rgba(255, 255, 255, 0.8);
        }

        /* 毛玻璃導航列 */
        .glass-nav {
            background: rgba(251, 249, 246, 0.85);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(212, 163, 115, 0.15);
        }

        /* 手風琴動畫 */
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.35s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .accordion-content.active {
            max-height: 500px;
        }

        /* 優雅淡入動畫 */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(15px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .animate-fade-in {
            animation: fadeIn 1s ease-out forwards;
        }
    </style>
</head>
<body class="antialiased selection:bg-morandi-gold selection:text-white">

    <!-- 頂端固定的毛玻璃導航列 -->
    <header class="fixed top-0 left-0 right-0 z-50 glass-nav transition-all duration-300">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <a href="#" class="font-cormorant text-2xl sm:text-3xl font-semibold tracking-wider text-morandi-text hover:text-morandi-gold transition-colors">
                C <span class="text-morandi-gold font-light">&amp;</span> Y
            </a>
            
            <nav class="hidden md:flex items-center space-x-8 text-sm tracking-widest font-medium">
                <a href="#about" class="hover:text-morandi-gold transition-colors py-1 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-morandi-gold hover:after:w-full after:transition-all">關於我們 <span class="text-[10px] block opacity-60 font-cormorant tracking-normal">ABOUT</span></a>
                <a href="#details" class="hover:text-morandi-gold transition-colors py-1 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-morandi-gold hover:after:w-full after:transition-all">婚禮詳情 <span class="text-[10px] block opacity-60 font-cormorant tracking-normal">DETAILS</span></a>
                <a href="#traffic" class="hover:text-morandi-gold transition-colors py-1 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-morandi-gold hover:after:w-full after:transition-all">交通指引 <span class="text-[10px] block opacity-60 font-cormorant tracking-normal">LOCATION</span></a>
                <a href="#rsvp" class="hover:text-morandi-gold transition-colors py-1 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-[1px] after:bg-morandi-gold hover:after:w-full after:transition-all">出席回函 <span class="text-[10px] block opacity-60 font-cormorant tracking-normal">RSVP</span></a>
            </nav>

            <!-- 行動裝置選單按鈕 -->
            <button id="mobile-menu-btn" class="md:hidden text-morandi-text hover:text-morandi-gold focus:outline-none p-2" aria-label="Toggle Menu">
                <i class="fa-solid fa-bars text-xl"></i>
            </button>
        </div>

        <!-- 行動裝置下拉選單 -->
        <div id="mobile-menu" class="hidden md:hidden bg-morandi-bg/95 border-b border-morandi-gold/20 px-6 py-4 space-y-3 text-center">
            <a href="#about" class="block py-2 text-morandi-text hover:text-morandi-gold border-b border-gray-100">關於我們 ABOUT</a>
            <a href="#details" class="block py-2 text-morandi-text hover:text-morandi-gold border-b border-gray-100">婚禮詳情 DETAILS</a>
            <a href="#traffic" class="block py-2 text-morandi-text hover:text-morandi-gold border-b border-gray-100">交通指引 LOCATION</a>
            <a href="#rsvp" class="block py-2 text-morandi-text hover:text-morandi-gold">出席回函 RSVP</a>
        </div>
    </header>

    <!-- 首頁全螢幕封面 -->
    <section class="relative h-screen w-full flex items-center justify-center overflow-hidden">
        <!-- 封面背景圖片與優雅遮罩 -->
        <div class="absolute inset-0 z-0">
            <img src="https://i.postimg.cc/Wp7nXLVH/IMG-2649.jpg" alt="Calvin & Yvonne Wedding" class="w-full h-full object-cover object-center transform scale-105 transition-transform duration-10000 ease-out" onerror="this.src='https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=1920&q=80'">
            <div class="absolute inset-0 bg-gradient-to-b from-black/40 via-black/20 to-black/50"></div>
        </div>

        <!-- 封面文字內容 -->
        <div class="relative z-10 text-center text-white px-4 max-w-4xl mx-auto animate-fade-in">
            <p class="font-cormorant italic text-xl sm:text-2xl md:text-3xl tracking-widest text-morandi-gold-light mb-2">We Are Getting Married</p>
            <h1 class="font-cormorant text-5xl sm:text-7xl md:text-8xl font-light tracking-wider my-4 drop-shadow-md">
                Calvin <span class="text-morandi-gold font-serif italic">&amp;</span> Yvonne
            </h1>
            <div class="w-16 h-[1px] bg-morandi-gold mx-auto my-6"></div>
            <p class="font-cormorant italic text-lg sm:text-xl md:text-2xl font-light tracking-wide text-gray-100 px-6 max-w-2xl mx-auto">
                "You’re the energy gel for my marathon."
            </p>
            <p class="mt-8 font-noto tracking-widest text-sm sm:text-base text-gray-200">
                2027 年 01 月 23 日 ． 星期六
            </p>
            <div class="mt-10">
                <a href="#rsvp" class="inline-block px-8 py-3 bg-morandi-gold/90 hover:bg-morandi-gold text-white tracking-widest text-sm rounded-full transition-all transform hover:-translate-y-0.5 shadow-lg backdrop-blur-sm border border-white/20">
                    出席回覆 RSVP
                </a>
            </div>
        </div>

        <!-- 下滑提示 -->
        <a href="#countdown" class="absolute bottom-8 left-1/2 transform -translate-x-1/2 z-10 text-white/80 hover:text-white transition-colors text-center animate-bounce">
            <span class="block text-[10px] tracking-widest font-cormorant uppercase mb-1">Scroll Down</span>
            <i class="fa-solid fa-chevron-down text-sm"></i>
        </a>
    </section>

    <!-- 倒數計時器 Section (白色微光卡片與極致美學設計) -->
    <section id="countdown" class="py-20 px-4 bg-gradient-to-b from-morandi-bg via-white to-morandi-bg relative">
        <div class="max-w-4xl mx-auto text-center">
            <span class="font-cormorant italic text-morandi-gold text-2xl block mb-1">Counting Down To Our Big Day</span>
            <h2 class="font-noto text-2xl sm:text-3xl font-normal text-morandi-text tracking-widest mb-12">距離婚禮倒數</h2>

            <!-- 微光倒數卡片容器 -->
            <div class="grid grid-cols-2 sm:grid-cols-4 gap-4 sm:gap-6 max-w-3xl mx-auto relative">
                
                <!-- 天 -->
                <div class="glow-card rounded-2xl p-5 sm:p-6 text-center transform hover:-translate-y-1 transition-transform duration-300 relative overflow-hidden group">
                    <div class="font-cormorant text-4xl sm:text-6xl font-semibold text-morandi-text tracking-tight" id="days">00</div>
                    <div class="w-8 h-[1px] bg-morandi-gold/40 mx-auto my-2"></div>
                    <span class="text-xs tracking-widest text-morandi-muted font-cormorant uppercase block">Days</span>
                    <span class="text-[10px] text-morandi-muted/80 font-noto block mt-0.5">天</span>
                    <!-- 垂直分隔細線 (細緻設計) -->
                    <div class="hidden sm:block absolute right-0 top-1/4 bottom-1/4 w-[1px] bg-morandi-gold/20"></div>
                </div>

                <!-- 小時 -->
                <div class="glow-card rounded-2xl p-5 sm:p-6 text-center transform hover:-translate-y-1 transition-transform duration-300 relative overflow-hidden group">
                    <div class="font-cormorant text-4xl sm:text-6xl font-semibold text-morandi-text tracking-tight" id="hours">00</div>
                    <div class="w-8 h-[1px] bg-morandi-gold/40 mx-auto my-2"></div>
                    <span class="text-xs tracking-widest text-morandi-muted font-cormorant uppercase block">Hours</span>
                    <span class="text-[10px] text-morandi-muted/80 font-noto block mt-0.5">小時</span>
                    <div class="hidden sm:block absolute right-0 top-1/4 bottom-1/4 w-[1px] bg-morandi-gold/20"></div>
                </div>

                <!-- 分鐘 -->
                <div class="glow-card rounded-2xl p-5 sm:p-6 text-center transform hover:-translate-y-1 transition-transform duration-300 relative overflow-hidden group">
                    <div class="font-cormorant text-4xl sm:text-6xl font-semibold text-morandi-text tracking-tight" id="minutes">00</div>
                    <div class="w-8 h-[1px] bg-morandi-gold/40 mx-auto my-2"></div>
                    <span class="text-xs tracking-widest text-morandi-muted font-cormorant uppercase block">Minutes</span>
                    <span class="text-[10px] text-morandi-muted/80 font-noto block mt-0.5">分鐘</span>
                    <div class="hidden sm:block absolute right-0 top-1/4 bottom-1/4 w-[1px] bg-morandi-gold/20"></div>
                </div>

                <!-- 秒 -->
                <div class="glow-card rounded-2xl p-5 sm:p-6 text-center transform hover:-translate-y-1 transition-transform duration-300 relative overflow-hidden group">
                    <div class="font-cormorant text-4xl sm:text-6xl font-semibold text-morandi-gold tracking-tight" id="seconds">00</div>
                    <div class="w-8 h-[1px] bg-morandi-gold/40 mx-auto my-2"></div>
                    <span class="text-xs tracking-widest text-morandi-muted font-cormorant uppercase block">Seconds</span>
                    <span class="text-[10px] text-morandi-muted/80 font-noto block mt-0.5">秒</span>
                </div>

            </div>

            <p class="mt-8 text-xs text-morandi-muted tracking-widest font-noto">目標時間：2027 年 1 月 23 日 上午 10:00</p>
        </div>
    </section>

    <!-- 關於我們 Section (垂直 V-Card 設計) -->
    <section id="about" class="py-24 px-4 bg-morandi-bg">
        <div class="max-w-3xl mx-auto">
            <div class="text-center mb-16">
                <span class="font-cormorant italic text-morandi-gold text-2xl block">Our Story</span>
                <h2 class="font-noto text-2xl sm:text-3xl text-morandi-text tracking-widest mt-1">關於我們</h2>
                <div class="w-12 h-[1px] bg-morandi-gold mx-auto mt-4"></div>
            </div>

            <!-- 垂直 V-Card -->
            <div class="bg-white rounded-3xl p-8 sm:p-14 shadow-soft border border-morandi-gold/15 text-center relative overflow-hidden">
                <!-- 裝飾性背景印記 -->
                <div class="absolute -right-12 -bottom-12 opacity-5 pointer-events-none">
                    <i class="fa-solid fa-heart text-9xl text-morandi-gold"></i>
                </div>

                <div class="space-y-6 text-morandi-text leading-relaxed font-noto text-base sm:text-lg">
                    <p class="font-cormorant text-3xl italic text-morandi-gold font-normal">
                        "You’re the energy gel for my marathon."
                    </p>
                    <p class="text-sm sm:text-base text-morandi-text/80 leading-loose max-w-xl mx-auto pt-2">
                        人生這場漫長而美好的馬拉松，<br>
                        因為有了彼此的陪伴，每一步都變得充滿力量與幸福。<br>
                        在 2027 年的第一個月，我們決定攜手邁向人生的下一個階段。
                    </p>
                </div>

                <!-- 新郎 & 新娘 簡介卡片 -->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mt-12 pt-12 border-t border-morandi-gold/10">
                    <div class="p-6 rounded-2xl bg-morandi-gold-light/30 border border-morandi-gold/20">
                        <div class="w-16 h-16 rounded-full bg-morandi-gold/20 text-morandi-gold flex items-center justify-center mx-auto mb-4 text-xl font-cormorant font-semibold">C</div>
                        <h3 class="font-cormorant text-2xl text-morandi-text font-semibold">Calvin</h3>
                        <p class="text-xs text-morandi-muted uppercase tracking-widest mt-1 mb-3">Groom ── 新郎</p>
                        <p class="text-xs text-morandi-text/70 leading-relaxed">你的神隊友與最堅實的後盾，隨時準備好補充滿滿的能量。</p>
                    </div>

                    <div class="p-6 rounded-2xl bg-morandi-sage-light/40 border border-morandi-sage/20">
                        <div class="w-16 h-16 rounded-full bg-morandi-sage/20 text-morandi-sage flex items-center justify-center mx-auto mb-4 text-xl font-cormorant font-semibold">Y</div>
                        <h3 class="font-cormorant text-2xl text-morandi-text font-semibold">Yvonne</h3>
                        <p class="text-xs text-morandi-muted uppercase tracking-widest mt-1 mb-3">Bride ── 新娘</p>
                        <p class="text-xs text-morandi-text/70 leading-relaxed">堅定而溫柔的跑者，帶著微笑陪伴彼此奔向每一個美好的終點。</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 婚禮詳情 Section -->
    <section id="details" class="py-24 px-4 bg-white relative">
        <div class="max-w-4xl mx-auto">
            <div class="text-center mb-16">
                <span class="font-cormorant italic text-morandi-gold text-2xl block">Wedding Details</span>
                <h2 class="font-noto text-2xl sm:text-3xl text-morandi-text tracking-widest mt-1">婚禮詳情</h2>
                <div class="w-12 h-[1px] bg-morandi-gold mx-auto mt-4"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
                
                <!-- 時間卡片 -->
                <div class="p-8 rounded-2xl bg-morandi-bg border border-morandi-gold/15 hover:shadow-soft transition-all">
                    <div class="w-12 h-12 rounded-full bg-morandi-gold/10 text-morandi-gold flex items-center justify-center mx-auto mb-4 text-lg">
                        <i class="fa-regular fa-calendar-check"></i>
                    </div>
                    <h3 class="font-noto text-lg font-medium text-morandi-text mb-2">宴會日期 DATE</h3>
                    <p class="font-cormorant text-xl text-morandi-gold font-semibold">2027.01.23</p>
                    <p class="text-xs text-morandi-muted mt-2">星期六 Saturday</p>
                </div>

                <!-- 時程卡片 -->
                <div class="p-8 rounded-2xl bg-morandi-bg border border-morandi-gold/15 hover:shadow-soft transition-all">
                    <div class="w-12 h-12 rounded-full bg-morandi-gold/10 text-morandi-gold flex items-center justify-center mx-auto mb-4 text-lg">
                        <i class="fa-regular fa-clock"></i>
                    </div>
                    <h3 class="font-noto text-lg font-medium text-morandi-text mb-2">活動時間 TIME</h3>
                    <p class="text-sm text-morandi-text"><span class="font-medium">10:00 AM</span> 證婚儀式 Ceremony</p>
                    <p class="text-sm text-morandi-text mt-1"><span class="font-medium">12:00 PM</span> 午宴入場 Banquet</p>
                </div>

                <!-- 地點卡片 -->
                <div class="p-8 rounded-2xl bg-morandi-bg border border-morandi-gold/15 hover:shadow-soft transition-all">
                    <div class="w-12 h-12 rounded-full bg-morandi-gold/10 text-morandi-gold flex items-center justify-center mx-auto mb-4 text-lg">
                        <i class="fa-solid fa-location-dot"></i>
                    </div>
                    <h3 class="font-noto text-lg font-medium text-morandi-text mb-2">宴會地點 VENUE</h3>
                    <p class="text-sm text-morandi-text font-medium no-wrap">福爾摩沙遊艇酒店</p>
                    <p class="text-xs text-morandi-muted mt-1 no-wrap">708001 台南市安平區安平路988號</p>
                    <p class="text-xs text-morandi-gold mt-2 font-cormorant font-semibold tracking-wider">TEL: 06-391-1313</p>
                </div>

            </div>
        </div>
    </section>

    <!-- 交通指引 Section (折疊式面板 Accordion & 防止斷行優化) -->
    <section id="traffic" class="py-24 px-4 bg-morandi-bg">
        <div class="max-w-3xl mx-auto">
            <div class="text-center mb-16">
                <span class="font-cormorant italic text-morandi-gold text-2xl block">Location &amp; Traffic</span>
                <h2 class="font-noto text-2xl sm:text-3xl text-morandi-text tracking-widest mt-1">交通指引</h2>
                <p class="text-xs text-morandi-muted mt-2 tracking-wider no-wrap">福爾摩沙遊艇酒店 Formosa Yacht Resort</p>
                <div class="w-12 h-[1px] bg-morandi-gold mx-auto mt-4"></div>
            </div>

            <!-- 折疊面板容器 -->
            <div class="space-y-4">
                
                <!-- 面板 1：國道一號 南下路線 -->
                <div class="bg-white rounded-2xl border border-morandi-gold/15 shadow-sm overflow-hidden">
                    <button class="accordion-btn w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none hover:bg-morandi-gold-light/20 transition-colors">
                        <div class="flex items-center space-x-3">
                            <i class="fa-solid fa-route text-morandi-gold text-lg"></i>
                            <span class="font-noto text-base text-morandi-text font-medium">自行開車 ── 國道一號（南下路線）</span>
                        </div>
                        <i class="fa-solid fa-chevron-down text-morandi-muted transition-transform duration-300 transform icon-arrow"></i>
                    </button>
                    <div class="accordion-content">
                        <div class="px-6 py-5 border-t border-gray-100 text-sm text-morandi-text/80 space-y-3 leading-relaxed">
                            <p class="font-medium text-morandi-text mb-2">【南下詳細行駛路線】</p>
                            <ol class="list-decimal list-inside space-y-1.5 text-xs sm:text-sm">
                                <li>國道1號至<span class="no-wrap font-medium text-morandi-gold">【台南系統】</span>接國道8號往台南</li>
                                <li>右轉<span class="no-wrap font-medium text-morandi-gold">【台江大道】</span> » 左轉<span class="no-wrap font-medium text-morandi-gold">【北汕尾路三路】</span></li>
                                <li>靠左行駛<span class="no-wrap font-medium text-morandi-gold">【鹿耳門大道 / 四草大道】</span></li>
                                <li>行經<span class="no-wrap font-medium text-morandi-gold">【四草大橋】</span>後左轉<span class="no-wrap font-medium text-morandi-gold">【安北路】</span></li>
                                <li>右轉<span class="no-wrap font-medium text-morandi-gold">【安平路990巷】</span> » 左轉<span class="no-wrap font-medium text-morandi-gold">【安平路】</span>即可抵達</li>
                            </ol>
                        </div>
                    </div>
                </div>

                <!-- 面板 2：國道一號 北上路線 -->
                <div class="bg-white rounded-2xl border border-morandi-gold/15 shadow-sm overflow-hidden">
                    <button class="accordion-btn w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none hover:bg-morandi-gold-light/20 transition-colors">
                        <div class="flex items-center space-x-3">
                            <i class="fa-solid fa-car text-morandi-gold text-lg"></i>
                            <span class="font-noto text-base text-morandi-text font-medium">自行開車 ── 國道一號（北上路線）</span>
                        </div>
                        <i class="fa-solid fa-chevron-down text-morandi-muted transition-transform duration-300 transform icon-arrow"></i>
                    </button>
                    <div class="accordion-content">
                        <div class="px-6 py-5 border-t border-gray-100 text-sm text-morandi-text/80 space-y-3 leading-relaxed">
                            <p class="font-medium text-morandi-text mb-2">【北上詳細行駛路線】</p>
                            <ol class="list-decimal list-inside space-y-1.5 text-xs sm:text-sm">
                                <li>國道1號至<span class="no-wrap font-medium text-morandi-gold">【仁德台86線】</span>往台南</li>
                                <li><span class="no-wrap font-medium text-morandi-gold">【台17線西部濱海公路】</span>往安平</li>
                                <li>左轉<span class="no-wrap font-medium text-morandi-gold">【民權路四段】</span> » 右轉<span class="no-wrap font-medium text-morandi-gold">【安北路】</span></li>
                                <li>左轉<span class="no-wrap font-medium text-morandi-gold">【安平路990巷】</span> » 左轉<span class="no-wrap font-medium text-morandi-gold">【安平路】</span>即可抵達</li>
                            </ol>
                        </div>
                    </div>
                </div>

                <!-- 面板 3：周邊地標與停車資訊 -->
                <div class="bg-white rounded-2xl border border-morandi-gold/15 shadow-sm overflow-hidden">
                    <button class="accordion-btn w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none hover:bg-morandi-gold-light/20 transition-colors">
                        <div class="flex items-center space-x-3">
                            <i class="fa-solid fa-square-parking text-morandi-gold text-lg"></i>
                            <span class="font-noto text-base text-morandi-text font-medium">周邊地標 &amp; 停車資訊 PARKING</span>
                        </div>
                        <i class="fa-solid fa-chevron-down text-morandi-muted transition-transform duration-300 transform icon-arrow"></i>
                    </button>
                    <div class="accordion-content">
                        <div class="px-6 py-5 border-t border-gray-100 text-sm text-morandi-text/80 space-y-3 leading-relaxed">
                            <p>
                                <strong class="text-morandi-text">【停車資訊】</strong><br>
                                飯店周邊及<span class="no-wrap font-medium text-morandi-gold">【水景灣】</span>旁皆設有特約停車區與停車場，請依現場指示停放。
                            </p>
                            <p>
                                <strong class="text-morandi-text">【公車與周邊景點】</strong><br>
                                公車站點：<span class="no-wrap font-medium text-morandi-gold">【古運河站 (福爾摩沙遊艇酒店)】</span><br>
                                鄰近地標：<span class="no-wrap">安平古堡</span>、<span class="no-wrap">安平樹屋</span>、<span class="no-wrap">東興洋行</span>、<span class="no-wrap">開台天后宮</span>、<span class="no-wrap">同記豆花</span>、<span class="no-wrap">米約廚房</span>。
                            </p>
                        </div>
                    </div>
                </div>

                <!-- 面板 4：地圖導航與飯店聯絡 -->
                <div class="bg-white rounded-2xl border border-morandi-gold/15 shadow-sm overflow-hidden">
                    <button class="accordion-btn w-full px-6 py-5 text-left flex justify-between items-center focus:outline-none hover:bg-morandi-gold-light/20 transition-colors">
                        <div class="flex items-center space-x-3">
                            <i class="fa-solid fa-map-location-dot text-morandi-gold text-lg"></i>
                            <span class="font-noto text-base text-morandi-text font-medium">地圖導航 GOOGLE MAPS</span>
                        </div>
                        <i class="fa-solid fa-chevron-down text-morandi-muted transition-transform duration-300 transform icon-arrow"></i>
                    </button>
                    <div class="accordion-content">
                        <div class="px-6 py-5 border-t border-gray-100 text-sm text-center space-y-4">
                            <p class="text-morandi-text/80">點擊下方按鈕開啟 Google 地圖進行導航：</p>
                            <div>
                                <a href="https://maps.google.com/?q=福爾摩沙遊艇酒店" target="_blank" rel="noopener noreferrer" class="inline-flex items-center space-x-2 px-6 py-2.5 bg-morandi-sage text-white rounded-full text-xs tracking-widest hover:bg-morandi-sage/90 transition-colors shadow-sm">
                                    <i class="fa-solid fa-diamond-turn-right"></i>
                                    <span>開啟 Google 地圖導航</span>
                                </a>
                            </div>
                            <div class="pt-2 text-xs text-morandi-muted space-y-1">
                                <p class="no-wrap">飯店代表號：06-391-1313 ｜ 宴會諮詢：06-391-0660</p>
                                <p class="no-wrap">官網：www.formosayacht.com.tw</p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- 出席回函 RSVP Section (中英雙語標籤 + 智能表單 + 隱藏式 iframe 提交) -->
    <section id="rsvp" class="py-24 px-4 bg-white relative">
        <div class="max-w-2xl mx-auto">
            <div class="text-center mb-12">
                <span class="font-cormorant italic text-morandi-gold text-2xl block">R.S.V.P.</span>
                <h2 class="font-noto text-2xl sm:text-3xl text-morandi-text tracking-widest mt-1">出席回函</h2>
                <p class="text-xs text-morandi-muted mt-2 tracking-wider">為利座席安排，請於 2026 年 12 月 15 日前填寫完畢</p>
                <div class="w-12 h-[1px] bg-morandi-gold mx-auto mt-4"></div>
            </div>

            <!-- 隱藏式 Iframe，用於跨域提交 Google 表單不跳轉 -->
            <iframe name="hidden_iframe" id="hidden_iframe" style="display:none;"></iframe>

            <!-- 回函表單 -->
            <form id="rsvpForm" action="https://docs.google.com/forms/d/e/1FAIpQLSdpu9y3fUdXMk12FCcSLxBIqtti5PFrDTABw3accN59-wtfqg/formResponse" method="POST" target="hidden_iframe" class="bg-morandi-bg/60 p-8 sm:p-10 rounded-3xl border border-morandi-gold/20 shadow-soft space-y-6">
                
                <!-- 姓名 (NAME) -->
                <div>
                    <label class="block text-xs font-semibold text-morandi-text tracking-widest mb-2">
                        姓名 <span class="font-cormorant font-normal text-morandi-muted text-sm ml-1">NAME</span> <span class="text-red-400">*</span>
                    </label>
                    <input type="text" name="entry.100000" required placeholder="請輸入您的姓名" class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:border-morandi-gold focus:ring-1 focus:ring-morandi-gold outline-none text-sm transition-all bg-white">
                </div>

                <!-- 行動電話 (PHONE) -->
                <div>
                    <label class="block text-xs font-semibold text-morandi-text tracking-widest mb-2">
                        電話 <span class="font-cormorant font-normal text-morandi-muted text-sm ml-1">PHONE</span> <span class="text-red-400">*</span>
                    </label>
                    <input type="tel" name="entry.100001" required placeholder="例如：0912345678" class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:border-morandi-gold focus:ring-1 focus:ring-morandi-gold outline-none text-sm transition-all bg-white">
                </div>

                <!-- 是否出席 (ATTENDANCE) -->
                <div>
                    <label class="block text-xs font-semibold text-morandi-text tracking-widest mb-2">
                        是否出席 <span class="font-cormorant font-normal text-morandi-muted text-sm ml-1">ATTENDANCE</span> <span class="text-red-400">*</span>
                    </label>
                    <select name="entry.100002" id="attendanceSelect" required class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:border-morandi-gold focus:ring-1 focus:ring-morandi-gold outline-none text-sm transition-all bg-white text-morandi-text">
                        <option value="" disabled selected>請選擇您的出席狀態</option>
                        <option value="個人出席">個人出席</option>
                        <option value="攜伴出席">攜伴出席</option>
                        <option value="遺憾無法出席">遺憾無法出席，獻上祝福</option>
                    </select>
                </div>

                <!-- 參加午宴人數 (GUESTS COUNT) -->
                <div>
                    <label class="block text-xs font-semibold text-morandi-text tracking-widest mb-2">
                        參加午宴人數 <span class="font-cormorant font-normal text-morandi-muted text-sm ml-1">ATTENDING GUESTS</span> <span class="text-red-400">*</span>
                    </label>
                    <input type="number" id="guestCountInput" name="entry.100003" min="0" max="10" value="0" required class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:border-morandi-gold focus:ring-1 focus:ring-morandi-gold outline-none text-sm transition-all bg-white">
                    <p class="text-[11px] text-morandi-muted mt-1">如無法出席請填 0，出席請輸入總人數（含大人）</p>
                </div>

                <!-- 智慧動態顯示區塊 (只有人數 > 0 時才顯示) -->
                <div id="dynamicFields" class="hidden space-y-6 pt-4 border-t border-morandi-gold/10 animate-fade-in">
                    
                    <!-- 飲食需求 (DIETARY PREFERENCE) -->
                    <div>
                        <label class="block text-xs font-semibold text-morandi-text tracking-widest mb-2">
                            飲食需求 <span class="font-cormorant font-normal text-morandi-muted text-sm ml-1">DIETARY PREFERENCE</span>
                        </label>
                        <select name="entry.100004" class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:border-morandi-gold focus:ring-1 focus:ring-morandi-gold outline-none text-sm transition-all bg-white text-morandi-text">
                            <option value="葷食">葷食</option>
                            <option value="全素">全素</option>
                            <option value="蛋奶素">蛋奶素</option>
                            <option value="特殊食物過敏">特殊食物過敏（請於備註說明）</option>
                        </select>
                    </div>

                    <!-- 是否需要兒童椅 (CHILD HIGH CHAIR NEEDED) -->
                    <div>
                        <label class="block text-xs font-semibold text-morandi-text tracking-widest mb-2">
                            是否需要兒童座椅 <span class="font-cormorant font-normal text-morandi-muted text-sm ml-1">CHILD HIGH CHAIR</span>
                        </label>
                        <select name="entry.100005" class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:border-morandi-gold focus:ring-1 focus:ring-morandi-gold outline-none text-sm transition-all bg-white text-morandi-text">
                            <option value="不需要">不需要</option>
                            <option value="需要 1 張">需要 1 張</option>
                            <option value="需要 2 張">需要 2 張</option>
                            <option value="需要 3 張以上">需要 3 張以上</option>
                        </select>
                    </div>

                </div>

                <!-- 祝福的話 (MESSAGE) -->
                <div>
                    <label class="block text-xs font-semibold text-morandi-text tracking-widest mb-2">
                        給新人的祝福 <span class="font-cormorant font-normal text-morandi-muted text-sm ml-1">BLESSINGS &amp; MESSAGE</span>
                    </label>
                    <textarea name="entry.100006" rows="3" placeholder="留下想對 Calvin & Yvonne 說的話吧..." class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:border-morandi-gold focus:ring-1 focus:ring-morandi-gold outline-none text-sm transition-all bg-white resize-none"></textarea>
                </div>

                <!-- 提交按鈕 -->
                <div class="pt-4">
                    <button type="submit" class="w-full py-4 bg-morandi-gold hover:bg-morandi-gold/90 text-white font-noto tracking-widest text-sm rounded-xl transition-all shadow-md hover:shadow-lg transform hover:-translate-y-0.5">
                        確認送出 SUBMIT
                    </button>
                </div>

            </form>
        </div>
    </section>

    <!-- 頁尾 Section -->
    <footer class="py-12 bg-morandi-bg border-t border-morandi-gold/15 text-center text-morandi-muted text-xs tracking-widest">
        <p class="font-cormorant text-base text-morandi-text mb-2">Calvin <span class="text-morandi-gold">&amp;</span> Yvonne</p>
        <p>2027.01.23 ． Thank you for being part of our special day</p>
    </footer>

    <!-- 提交成功彈窗 Modal -->
    <div id="thankYouModal" class="fixed inset-0 z-50 flex items-center justify-center bg-black/50 backdrop-blur-sm hidden opacity-0 transition-opacity duration-300">
        <div class="bg-white rounded-3xl p-8 sm:p-10 max-w-md mx-4 text-center shadow-glow border border-morandi-gold/20 transform scale-95 transition-transform duration-300">
            <div class="w-16 h-16 rounded-full bg-morandi-gold/10 text-morandi-gold flex items-center justify-center mx-auto mb-4 text-2xl">
                <i class="fa-solid fa-heart"></i>
            </div>
            <h3 class="font-noto text-xl font-medium text-morandi-text mb-2">收到您的回函！</h3>
            <p class="text-sm text-morandi-text/80 leading-relaxed mb-6">
                感謝您撥冗填寫出席回函。<br>我們非常期待在 2027 年 1 月 23 日與您一同分享這份喜悅！
            </p>
            <button onclick="closeThankYouModal()" class="px-8 py-2.5 bg-morandi-gold text-white text-xs tracking-widest rounded-full hover:bg-morandi-gold/90 transition-colors">
                關閉 CLOSE
            </button>
        </div>
    </div>

    <!-- JavaScript 邏輯控制 -->
    <script>
        // 0. 全域變數與 Iframe onload 監聽器設定 (防止 ReferenceError)
        let submitted = false;
        const hiddenIframe = document.getElementById('hidden_iframe');
        if (hiddenIframe) {
            hiddenIframe.onload = function() {
                if (submitted) {
                    showThankYouModal();
                }
            };
        }

        // 1. 倒數計時邏輯 (Target: 2027-01-23T10:00:00)
        const targetDate = new Date("2027-01-23T10:00:00").getTime();

        function updateCountdown() {
            const now = new Date().getTime();
            const difference = targetDate - now;

            if (difference > 0) {
                const days = Math.floor(difference / (1000 * 60 * 60 * 24));
                const hours = Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((difference % (1000 * 60)) / 1000);

                document.getElementById("days").innerText = days.toString().padStart(2, '0');
                document.getElementById("hours").innerText = hours.toString().padStart(2, '0');
                document.getElementById("minutes").innerText = minutes.toString().padStart(2, '0');
                document.getElementById("seconds").innerText = seconds.toString().padStart(2, '0');
            } else {
                document.getElementById("days").innerText = "00";
                document.getElementById("hours").innerText = "00";
                document.getElementById("minutes").innerText = "00";
                document.getElementById("seconds").innerText = "00";
            }
        }
        setInterval(updateCountdown, 1000);
        updateCountdown();

        // 2. 交通指引摺疊面板 (Accordion)
        const accordionBtns = document.querySelectorAll('.accordion-btn');
        accordionBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                const content = btn.nextElementSibling;
                const arrow = btn.querySelector('.icon-arrow');
                
                // 切換開關
                const isOpen = content.classList.contains('active');
                
                // 關閉其他面板
                document.querySelectorAll('.accordion-content').forEach(c => c.classList.remove('active'));
                document.querySelectorAll('.icon-arrow').forEach(a => a.style.transform = 'rotate(0deg)');

                if (!isOpen) {
                    content.classList.add('active');
                    arrow.style.transform = 'rotate(180deg)';
                }
            });
        });

        // 3. 智能動態欄位控制：僅當『參加午宴人數』> 0 時顯示飲食與兒童椅需求
        const guestCountInput = document.getElementById('guestCountInput');
        const dynamicFields = document.getElementById('dynamicFields');
        const attendanceSelect = document.getElementById('attendanceSelect');

        function checkDynamicFields() {
            const count = parseInt(guestCountInput.value, 10) || 0;
            if (count > 0 && attendanceSelect.value !== "遺憾無法出席") {
                dynamicFields.classList.remove('hidden');
            } else {
                dynamicFields.classList.add('hidden');
            }
        }

        guestCountInput.addEventListener('input', checkDynamicFields);
        attendanceSelect.addEventListener('change', function() {
            if (this.value === "遺憾無法出席") {
                guestCountInput.value = 0;
            } else if (parseInt(guestCountInput.value, 10) === 0) {
                guestCountInput.value = 1;
            }
            checkDynamicFields();
        });

        // 4. 隱藏式 Iframe 表單提交機制
        const rsvpForm = document.getElementById('rsvpForm');

        rsvpForm.addEventListener('submit', function() {
            submitted = true;
        });

        function showThankYouModal() {
            const modal = document.getElementById('thankYouModal');
            modal.classList.remove('hidden');
            setTimeout(() => {
                modal.classList.remove('opacity-0');
                modal.querySelector('div').classList.remove('scale-95');
                modal.querySelector('div').classList.add('scale-100');
            }, 10);
            rsvpForm.reset();
            checkDynamicFields();
            submitted = false;
        }

        function closeThankYouModal() {
            const modal = document.getElementById('thankYouModal');
            modal.classList.add('opacity-0');
            modal.querySelector('div').classList.add('scale-95');
            setTimeout(() => {
                modal.classList.add('hidden');
            }, 300);
        }

        // 5. 行動裝置 Menu 切換
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // 點擊選單連結後自動關閉選單
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
