<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>墨语智学</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#2962FF',
                        secondary: '#9C27B0'
                    },
                    borderRadius: {
                        'none': '0px',
                        'sm': '2px',
                        DEFAULT: '4px',
                        'md': '8px',
                        'lg': '12px',
                        'xl': '16px',
                        '2xl': '20px',
                        '3xl': '24px',
                        'full': '9999px',
                        'button': '4px'
                    }
                }
            }
        }
    </script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Poppins:wght@600&family=Noto+Sans+SC:wght@400;500;700&family=ZCOOL+XiaoWei&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            min-height: 1024px;
            background: linear-gradient(135deg, #F5F7FF 0%, #E3F2FF 100%);
            overflow-x: hidden;
        }
        .gradient-text {
            background: linear-gradient(90deg, #2962FF, #9C27B0);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        .blur-circle {
            position: absolute;
            border-radius: 50%;
            filter: blur(100px);
            opacity: 0.2;
        }
        .cta-button {
            animation: pulse 2s ease-in-out 2;
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.02); }
            100% { transform: scale(1); }
        }
        .bg-decoration {
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M50 50C50 77.6142 27.6142 100 0 100C-27.6142 100 -50 77.6142 -50 50C-50 22.3858 -27.6142 0 0 0C27.6142 0 50 22.3858 50 50Z' fill='%232962FF' fill-opacity='0.03'/%3E%3C/svg%3E");
            opacity: 0.03;
            pointer-events: none;
        }
    </style>
</head>
<body class="relative">
    <div class="blur-circle w-[500px] h-[500px] bg-primary top-[-100px] right-[-100px]"></div>
    <div class="blur-circle w-[500px] h-[500px] bg-secondary bottom-[-100px] left-[-100px]"></div>
    <div class="bg-decoration"></div>
    
    <div class="flex flex-col items-center justify-center min-h-screen w-full max-w-[1440px] mx-auto px-4">
        <div class="flex flex-col items-center mb-12">
            <div class="w-20 h-20 rounded-full bg-gradient-to-r from-primary to-secondary flex items-center justify-center mb-4">
                <i class="fas fa-graduation-cap text-white text-3xl"></i>
            </div>
            <h1 class="text-4xl font-['ZCOOL_XiaoWei'] gradient-text mb-2">墨语智学</h1>
        </div>
        
        <h2 class="text-2xl text-primary font-['Noto_Sans_SC'] font-medium text-center mb-16">
            AI 驱动的智能英语学习平台
        </h2>
        
        <button onclick="window.location.href='墨语智学首页.html'" class="cta-button group flex items-center justify-center w-[240px] h-[60px] bg-gradient-to-r from-primary to-secondary text-white text-lg font-['Noto_Sans_SC'] font-medium rounded-lg shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-1 !rounded-button whitespace-nowrap">
            立即体验
            <i class="fas fa-arrow-right ml-2 transition-transform duration-300 group-hover:translate-x-1"></i>
        </button>
    </div>
</body>
</html>
