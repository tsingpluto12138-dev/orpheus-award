<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2026 奥菲斯国际青年影像奖 | ORPHEUS INTERNATIONAL YOUTH FILM & VIDEO ART AWARD</title>
    <!-- 引入Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- 引入Font Awesome图标 -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- 自定义Tailwind配置 -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#D4AF37', // 主色调-暗金
                        secondary: '#0A0F1D', // 背景主色-深空黑
                        neutral: '#1A1F2E', // 卡片背景色
                        light: '#E8E8E8', // 正文浅色
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .content-auto {
                content-visibility: auto;
            }
            .text-shadow {
                text-shadow: 0 2px 10px rgba(0,0,0,0.5);
            }
            .card-hover {
                transition: all 0.3s ease;
            }
            .bg-grain {
                background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)' opacity='0.1'/%3E%3C/svg%3E");
            }
        }
    </style>
</head>
<body class="bg-secondary text-light bg-grain min-h-screen">
    <!-- 导航栏 -->
    <nav id="navbar" class="fixed w-full top-0 z-50 transition-all duration-300 py-4">
        <div class="container mx-auto px-4 md:px-8 flex justify-between items-center">
            <a href=" " class="flex items-center gap-2">
                <span class="text-primary font-bold text-xl md:text-2xl">ORPHEUS</span>
                <span class="hidden md:inline text-sm font-light tracking-widest">国际青年影像奖</span>
            </a >
            <!-- 桌面端导航 -->
            <div class="hidden md:flex items-center gap-8">
                <a href="#home" class="hover:text-primary transition-colors">首页</a >
                <a href="#about" class="hover:text-primary transition-colors">赛事简介</a >
                <a href="#awards" class="hover:text-primary transition-colors">奖项设置</a >
                <a href="#highlights" class="hover:text-primary transition-colors">赛事亮点</a >
                <a href="#winners" class="hover:text-primary transition-colors">获奖名单</a >
                <a href="#contact" class="hover:text-primary transition-colors">合作联系</a >
            </div>
            <!-- 移动端菜单按钮 -->
            <button id="menuBtn" class="md:hidden text-2xl">
                <i class="fas fa-bars"></i>
            </button>
        </div>
        <!-- 移动端导航菜单 -->
        <div id="mobileMenu" class="md:hidden hidden bg-secondary/95 backdrop-blur-md w-full absolute top-full left-0 py-4 px-4 border-t border-primary/20">
            <div class="flex flex-col gap-4">
                <a href="#home" class="py-2 hover:text-primary transition-colors">首页</a >
                <a href="#about" class="py-2 hover:text-primary transition-colors">赛事简介</a >
                <a href="#awards" class="py-2 hover:text-primary transition-colors">奖项设置</a >
                <a href="#highlights" class="py-2 hover:text-primary transition-colors">赛事亮点</a >
                <a href="#winners" class="py-2 hover:text-primary transition-colors">获奖名单</a >
                <a href="#contact" class="py-2 hover:text-primary transition-colors">合作联系</a >
            </div>
        </div>
    </nav>

    <!-- 首屏Hero区 -->
    <section id="home" class="relative h-screen flex items-center justify-center overflow-hidden">
        <div class="absolute inset-0 bg-gradient-to-b from-secondary/80 to-secondary z-10"></div>
        <div class="absolute inset-0 bg-[url('https://picsum.photos/id/1050/1920/1080')] bg-cover bg-center opacity-40"></div>
        <div class="container mx-auto px-4 z-20 text-center">
            <p class="text-primary tracking-[0.3em] text-sm md:text-base mb-4 font-light animate-fadeIn">2026 年度获奖名单正式公布</p >
            <h1 class="text-[clamp(2rem,8vw,5rem)] font-bold text-white text-shadow mb-4 leading-tight">
                奥菲斯国际青年影像奖
            </h1>
            <p class="text-[clamp(1rem,3vw,1.5rem)] font-light tracking-widest text-white/80 mb-8">
                ORPHEUS INTERNATIONAL YOUTH FILM & VIDEO AWARD
            </p >
            <p class="max-w-2xl mx-auto text-light/70 text-lg mb-12">
                以影像为桥，以热爱为炬 | 全球青年影像创作者的国际艺术舞台
            </p >
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#winners" class="inline-block bg-primary text-secondary font-medium py-3 px-8 rounded-sm hover:bg-primary/90 transition-all duration-300 shadow-lg shadow-primary/20">
                    查看完整获奖名单
                </a >
                <a href="#about" class="inline-block border border-primary text-primary font-medium py-3 px-8 rounded-sm hover:bg-primary/10 transition-all duration-300">
                    了解赛事详情
                </a >
            </div>
        </div>
        <div class="absolute bottom-8 left-1/2 -translate-x-1/2 z-20 animate-bounce">
            <a href="#about" class="text-white/70 hover:text-primary">
                <i class="fas fa-chevron-down text-xl"></i>
            </a >
        </div>
    </section>

    <!-- 赛事简介区 -->
    <section id="about" class="py-20 md:py-28">
        <div class="container mx-auto px-4 md:px-8">
            <div class="max-w-4xl mx-auto text-center mb-16">
                <h2 class="text-[clamp(1.5rem,4vw,2.5rem)] font-bold mb-6">
                    <span class="text-primary">ABOUT</span> 赛事简介
                </h2>
                <div class="w-20 h-1 bg-primary/50 mx-auto mb-8"></div>
            </div>

            <div class="max-w-4xl mx-auto space-y-12">
                <!-- 赛事全称、创办初衷与核心宗旨 -->
                <div class="space-y-4">
                    <h3 class="text-xl md:text-2xl font-bold text-white">赛事全称、创办初衷与核心宗旨</h3>
                    <p class="text-light/80 text-lg leading-relaxed">
                        <strong>赛事全称</strong>：奥菲斯国际青年影像奖（ORPHEUS INTERNATIONAL YOUTH FILM & VIDEO AWARD）
                    </p >
                    <p class="text-light/80 text-lg leading-relaxed">
                        以希腊神话中用琴声撼动天地的奥菲斯为精神内核，奖项创办初衷，是致敬每一位用影像传递情感、表达自我的青年创作者，打破艺术表达的边界与地域文化的隔阂。我们始终坚守以影像为桥，以热爱为炬的核心宗旨，守护青年创作的原生力量，让优质青年影像作品被世界看见，让青年创作者的艺术理想拥有落地生根的舞台。
                    </p >
                </div>

                <!-- 赛事定位 -->
                <div class="space-y-4">
                    
