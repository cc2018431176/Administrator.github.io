<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>创新科技 - 引领未来科技潮流</title>
  <!-- 引入Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- 引入Font Awesome -->
  <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
  <!-- 配置Tailwind自定义颜色和字体 -->
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#165DFF',
            secondary: '#36BFFA',
            accent: '#7B61FF',
            dark: '#1D2939',
            light: '#F9FAFB'
          },
          fontFamily: {
            inter: ['Inter', 'system-ui', 'sans-serif'],
          },
        },
      }
    }
  </script>
  <style type="text/tailwindcss">
    @layer utilities {
      .content-auto {
        content-visibility: auto;
      }
      .text-shadow {
        text-shadow: 0 2px 4px rgba(0,0,0,0.1);
      }
      .card-hover {
        transition: all 0.3s ease;
      }
      .card-hover:hover {
        transform: translateY(-5px);
      }
    }
  </style>
</head>
<body class="font-inter text-dark bg-light">
  <!-- 导航栏 -->
  <header id="navbar" class="fixed w-full top-0 z-50 transition-all duration-300 bg-white/90 backdrop-blur-sm shadow-sm">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center py-4">
        <a href="#" class="flex items-center space-x-2">
          <div class="w-10 h-10 rounded-full bg-primary rounded-lg flex items-center justify-center">
            <i class="fa fa-rocket text-white text-xl"></i>
          </div>
          <span class="text-xl font-bold text-dark">创新科技</span>
        </a>
        
        <!-- 桌面导航 -->
        <nav class="hidden md:flex items-center space-x-8">
          <a href="#home" class="text-dark hover hover:text-primary transition-colors font-medium">首页</a>
          <a href="#features" class="text-dark hover:text-primary transition-colors font-medium">特色</a>
          <a href="#services" class="text-dark hover:text-primary transition-colors font-medium">服务</a>
          <a href="#testimonials" class="text-dark hover:text-primary transition-colors font-medium">客户评价</a>
          <a href="#contact" class="text-dark hover:text-primary transition-colors font-medium">联系我们</a>
        </nav>
        
        <!-- 联系按钮 -->
        <a href="#contact" class="hidden md:block bg-primary hover:bg-primary/90 text-white px-5 py-2 rounded-lg transition-all shadow-md hover:shadow-lg">
          立即咨询
        </a>
        
        <!-- 移动端菜单汉堡菜单按钮 -->
        <button id="menu-toggle" class="md:hidden text-dark focus:outline-none">
          <i class="fa fa-bars text-2xl"></i>
        </button>
      </div>
    </div>
    
    <!-- 移动端导航菜单 -->
    <div id="mobile-menu" class="md:hidden hidden-0 h-0 overflow-hidden bg-white shadow-lg transition-all duration-300">
      <div class="container mx-auto px-4 py-3 space-y-3">
        <a href="#home" class="block py-2 text-dark hover:text-primary transition-colors">首页</a>
        <a href="#features" class="block py-2 text-dark hover:text-primary transition-colors">特色</a>
        <a href="#services" class="block py-2 text-dark hover:text-primary transition-colors">服务</a>
        <a href="#testimonials" class="block py-2 text-dark hover:text-primary transition-colors">客户评价</a>
        <a href="#contact" class="block py-2 text-dark hover:text-primary transition-colors">联系我们</a>
        <a href="#contact" class="block w-full text-center bg-primary hover:bg-primary/90 text-white px-5 py-2 rounded-lg transition-all">
          立即咨询
        </a>
      </div>
    </div>
  </header>

  <main>
    <!-- 英雄区域 -->
    <section id="home" class="pt-28 pb-20 md:pt-40 md:pb-32 bg-gradient-to-br from-primary/5 to-secondary/5">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex flex-col lg:flex-row items-center">
          <div class="w-full lg:w-1/2 mb-10 lg:mb-0">
            <h1 class="text-[clamp(2rem,5vw,3.5rem)] font-bold leading-tight text-dark mb-6">
              用<span class="text-primary">创新科技</span>
              <br>塑造未来世界
            </h1>
            <p class="text-lg text-gray-600 mb-8 max-w-xl">
              我们提供前沿的技术解决方案，帮助企业实现数字化转型，提升竞争力，引领行业创新发展。
            </p>
            <div class="flex flex-col sm:flex-row gap-4">
              <a href="#services" class="bg-primary hover:bg-primary/90 text-white px-8 py-3 rounded-lg transition-all shadow-lg hover:shadow-xl text-center font-medium">
                探索服务
              </a>
              <a href="#contact" class="bg-white border border-gray-200 hover:border-primary text-dark hover:text-primary px-8 py-3 rounded-lg transition-all shadow-md hover:shadow-lg text-center font-medium">
                联系我们
              </a>
            </div>
            <div class="mt-10 flex items-center">
              <div class="flex -space-x-3">
                <img src="https://picsum.photos/id/1001/100/100" alt="客户头像" class="w-10 h-10 rounded-full border-2 border-white">
                <img src="https://picsum.photos/id/1002/100/100" alt="客户头像" class="w-10 h-10 rounded-full border-2 border-white">
                <img src="https://picsum.photos/id/1003/100/100" alt="客户头像" class="w-10 h-10 rounded-full border-2 border-white">
                <img src="https://picsum.photos/id/1004/100/100" alt="客户头像" class="w-10 h-10 rounded-full border-2 border-white">
                <div class="w-10 h-10 rounded-full bg-primary/10 text-primary border-2 border-white flex items-center justify-center text-sm font-medium">
                  99+
                </div>
              </div>
              <div class="ml-4">
                <div class="flex items-center text-yellow-400 mb-1">
                  <i class="fa fa-star"></i>
                  <i class="fa fa-star"></i>
                  <i class="fa fa-star"></i>
                  <i class="fa fa-star"></i>
                  <i class="fa fa-star-half-o"></i>
                  <span class="ml-2 text-gray-600">4.8/5</span>
                </div>
                <p class="text-sm text-gray-500">来自200+客户的好评</p>
              </div>
            </div>
          </div>
          <div class="w-full lg:w-1/2 relative">
            <div class="relative z-10 rounded-2xl overflow-hidden shadow-2xl">
              <img src="https://picsum.photos/id/1/600/400" alt="创新科技解决方案" class="w-full h-auto">
            </div>
            <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-full h-full bg-gradient-to-r from-primary/30 to-secondary/30 rounded-2xl -z-10 transform rotate-3 scale-105"></div>
            <!-- 悬浮卡片 -->
            <div class="absolute -bottom-6 -left-6 md:-left-12 bg-white p-4 rounded-xl shadow-xl z-20">
              <div class="flex items-center gap-3">
                <div class="w-12 h-12 rounded-full bg-green-100 flex items-center justify-center text-green-600">
                  <i class="fa fa-line-chart text-xl"></i>
                </div>
                <div>
                  <p class="text-sm text-gray-500">业务增长</p>
                  <p class="text-xl font-bold">+127%</p>
                </div>
              </div>
            </div>
            <div class="absolute -top-6 -right-6 md:-right-12 bg-white p-4 rounded-xl shadow-xl z-20">
              <div class="flex items-center gap-3">
                <div class="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center text-blue-600">
                  <i class="fa fa-users text-xl"></i>
                </div>
                <div>
                  <p class="text-sm text-gray-500">满意客户</p>
                  <p class="text-xl font-bold">500+</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 合作伙伴 -->
    <section class="py-12 bg-white">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <p class="text-center text-gray-500 mb-8">值得信赖的合作伙伴</p>
        <div class="flex flex-wrap justify-center items-center gap-8 md:gap-16 opacity-70">
          <div class="text-gray-400 text-2xl font-bold">阿里云</div>
          <div class="text-gray-400 text-2xl font-bold">腾讯云</div>
          <div class="text-gray-400 text-2xl font-bold">华为云</div>
          <div class="text-gray-400 text-2xl font-bold">百度智能云</div>
          <div class="text-gray-400 text-2xl font-bold">亚马逊AWS</div>
        </div>
      </div>
    </section>

    <!-- 特色内容 -->
    <section id="features" class="py-20 bg-white">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center max-w-3xl mx-auto mb-16">
          <span class="inline-block px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full mb-4">核心优势</span>
          <h2 class="text-[clamp(1.8rem,4vw,2.5rem)] font-bold mb-6">为什么选择我们的技术服务</h2>
          <p class="text-gray-600 text-lg">我们拥有多年行业经验，提供全方位的技术支持，帮助企业解决各种技术难题，实现业务增长。</p>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- 特色1 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm card-hover">
            <div class="w-14 h-14 rounded-xl bg-primary/10 flex items-center justify-center text-primary mb-6">
              <i class="fa fa-lightbulb-o text-2xl"></i>
            </div>
            <h3 class="text-xl font-bold mb-4">创新解决方案</h3>
            <p class="text-gray-600">我们提供创新的技术解决方案，帮助企业应对各种挑战，抓住市场机遇，实现业务突破。</p>
          </div>
          
          <!-- 特色2 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm card-hover">
            <div class="w-14 h-14 rounded-xl bg-secondary/10 flex items-center justify-center text-secondary mb-6">
              <i class="fa fa-rocket text-2xl"></i>
            </div>
            <h3 class="text-xl font-bold mb-4">高效执行团队</h3>
            <p class="text-gray-600">我们的团队由行业专家组成，具备丰富的实战经验，能够快速高效地完成项目交付。</p>
          </div>
          
          <!-- 特色3 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm card-hover">
            <div class="w-14 h-14 rounded-xl bg-accent/10 flex items-center justify-center text-accent mb-6">
              <i class="fa fa-shield text-2xl"></i>
            </div>
            <h3 class="text-xl font-bold mb-4">安全可靠保障</h3>
            <p class="text-gray-600">我们重视数据安全和系统稳定性，采用先进的安全技术，确保客户业务的持续稳定运行。</p>
          </div>
          
          <!-- 特色4 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm card-hover">
            <div class="w-14 h-14 rounded-xl bg-green-100 flex items-center justify-center text-green-600 mb-6">
              <i class="fa fa-cogs text-2xl"></i>
            </div>
            <h3 class="text-xl font-bold mb-4">定制化服务</h3>
            <p class="text-gray-600">根据客户的具体需求，提供个性化的解决方案，满足不同行业、不同规模企业的独特需求。</p>
          </div>
          
          <!-- 特色5 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm card-hover">
            <div class="w-14 h-14 rounded-xl bg-yellow-100 flex items-center justify-center text-yellow-600 mb-6">
              <i class="fa fa-clock-o text-2xl"></i>
            </div>
            <h3 class="text-xl font-bold mb-4">7×24小时支持</h3>
            <p class="text-gray-600">我们提供全天候的技术支持服务，随时响应客户需求，解决各种突发问题，保障业务连续性。</p>
          </div>
          
          <!-- 特色6 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm card-hover">
            <div class="w-14 h-14 rounded-xl bg-red-100 flex items-center justify-center text-red-600 mb-6">
              <i class="fa fa-line-chart text-2xl"></i>
            </div>
            <h3 class="text-xl font-bold mb-4">持续优化升级</h3>
            <p class="text-gray-600">不仅提供一次性解决方案，还会持续跟踪优化，根据业务发展和技术趋势进行系统升级。</p>
          </div>
        </div>
      </div>
    </section>

    <!-- 服务展示 -->
    <section id="services" class="py-20 bg-gray-50">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center max-w-3xl mx-auto mb-16">
          <span class="inline-block px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full mb-4">我们的服务</span>
          <h2 class="text-[clamp(1.8rem,4vw,2.5rem)] font-bold mb-6">全方位的技术服务</h2>
          <p class="text-gray-600 text-lg">我们提供从咨询到实施的全流程服务，满足企业在数字化转型过程中的各种需求。</p>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- 服务1 -->
          <div class="bg-white rounded-2xl overflow-hidden shadow-md card-hover">
            <div class="h-48 overflow-hidden">
              <img src="https://picsum.photos/id/2/600/400" alt="云计算服务" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
            </div>
            <div class="p-6">
              <h3 class="text-xl font-bold mb-3">云计算服务</h3>
              <p class="text-gray-600 mb-4">提供灵活、安全、高效的云计算解决方案，帮助企业降低IT成本，提升业务灵活性。</p>
              <a href="#contact" class="inline-flex items-center text-primary font-medium hover:underline">
                了解更多 <i class="fa fa-arrow-right ml-2"></i>
              </a>
            </div>
          </div>
          
          <!-- 服务2 -->
          <div class="bg-white rounded-2xl overflow-hidden shadow-md card-hover">
            <div class="h-48 overflow-hidden">
              <img src="https://picsum.photos/id/3/600/400" alt="人工智能解决方案" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
            </div>
            <div class="p-6">
              <h3 class="text-xl font-bold mb-3">人工智能解决方案</h3>
              <p class="text-gray-600 mb-4">利用先进的人工智能技术，帮助企业实现业务智能化，提升运营效率和决策准确性。</p>
              <a href="#contact" class="inline-flex items-center text-primary font-medium hover:underline">
                了解更多 <i class="fa fa-arrow-right ml-2"></i>
              </a>
            </div>
          </div>
          
          <!-- 服务3 -->
          <div class="bg-white rounded-2xl overflow-hidden shadow-md card-hover">
            <div class="h-48 overflow-hidden">
              <img src="https://picsum.photos/id/4/600/400" alt="大数据分析" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
            </div>
            <div class="p-6">
              <h3 class="text-xl font-bold mb-3">大数据分析</h3>
              <p class="text-gray-600 mb-4">通过大数据分析技术，帮助企业挖掘数据价值，发现市场趋势，优化业务决策。</p>
              <a href="#contact" class="inline-flex items-center text-primary font-medium hover:underline">
                了解更多 <i class="fa fa-arrow-right ml-2"></i>
              </a>
            </div>
          </div>
          
          <!-- 服务4 -->
          <div class="bg-white rounded-2xl overflow-hidden shadow-md card-hover">
            <div class="h-48 overflow-hidden">
              <img src="https://picsum.photos/id/5/600/400" alt="区块链技术" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
            </div>
            <div class="p-6">
              <h3 class="text-xl font-bold mb-3">区块链技术</h3>
              <p class="text-gray-600 mb-4">提供安全可靠的区块链解决方案，用于供应链管理、数字资产、智能合约等场景。</p>
              <a href="#contact" class="inline-flex items-center text-primary font-medium hover:underline">
                了解更多 <i class="fa fa-arrow-right ml-2"></i>
              </a>
            </div>
          </div>
          
          <!-- 服务5 -->
          <div class="bg-white rounded-2xl overflow-hidden shadow-md card-hover">
            <div class="h-48 overflow-hidden">
              <img src="https://picsum.photos/id/6/600/400" alt="物联网解决方案" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
            </div>
            <div class="p-6">
              <h3 class="text-xl font-bold mb-3">物联网解决方案</h3>
              <p class="text-gray-600 mb-4">连接智能设备，实现数据实时采集和分析，助力企业实现智能化运营和管理。</p>
              <a href="#contact" class="inline-flex items-center text-primary font-medium hover:underline">
                了解更多 <i class="fa fa-arrow-right ml-2"></i>
              </a>
            </div>
          </div>
          
          <!-- 服务6 -->
          <div class="bg-white rounded-2xl overflow-hidden shadow-md card-hover">
            <div class="h-48 overflow-hidden">
              <img src="https://picsum.photos/id/7/600/400" alt="网络安全服务" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
            </div>
            <div class="p-6">
              <h3 class="text-xl font-bold mb-3">网络安全服务</h3>
              <p class="text-gray-600 mb-4">提供全方位的网络安全防护，保护企业数据和系统安全，防范各类网络威胁。</p>
              <a href="#contact" class="inline-flex items-center text-primary font-medium hover:underline">
                了解更多 <i class="fa fa-arrow-right ml-2"></i>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 统计数据 -->
    <section class="py-16 bg-primary text-white">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
          <div>
            <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="15">0</div>
            <p class="text-white/80">年行业经验</p>
          </div>
          <div>
            <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="500">0</div>
            <p class="text-white/80">成功案例</p>
          </div>
          <div>
            <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="200">0</div>
            <p class="text-white/80">专业技术人员</p>
          </div>
          <div>
            <div class="text-4xl md:text-5xl font-bold mb-2 counter" data-target="98">0</div>
            <p class="text-white/80">客户满意度(%)</p>
          </div>
        </div>
      </div>
    </section>

    <!-- 客户评价 -->
    <section id="testimonials" class="py-20 bg-white">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center max-w-3xl mx-auto mb-16">
          <span class="inline-block px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full mb-4">客户评价</span>
          <h2 class="text-[clamp(1.8rem,4vw,2.5rem)] font-bold mb-6">客户对我们的评价</h2>
          <p class="text-gray-600 text-lg">听听我们的客户怎么说，他们的成功案例是我们服务质量的最好证明。</p>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- 评价1 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm relative card-hover">
            <div class="text-primary text-6xl absolute top-6 right-6 opacity-20">
              <i class="fa fa-quote-right"></i>
            </div>
            <div class="flex text-yellow-400 mb-4">
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
            </div>
            <p class="text-gray-600 mb-6 relative z-10">创新科技帮助我们实现了数字化转型，他们的云计算解决方案不仅降低了我们的IT成本，还大大提升了业务灵活性。团队专业且高效，值得信赖。</p>
            <div class="flex items-center">
              <img src="https://picsum.photos/id/1010/100/100" alt="客户头像" class="w-12 h-12 rounded-full mr-4">
              <div>
                <h4 class="font-bold">张明</h4>
                <p class="text-gray-500 text-sm">某科技公司CTO</p>
              </div>
            </div>
          </div>
          
          <!-- 评价2 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm relative card-hover">
            <div class="text-primary text-6xl absolute top-6 right-6 opacity-20">
              <i class="fa fa-quote-right"></i>
            </div>
            <div class="flex text-yellow-400 mb-4">
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
            </div>
            <p class="text-gray-600 mb-6 relative z-10">我们与创新科技合作已有三年，他们的大数据分析服务帮助我们深入了解客户需求，优化产品策略，业务增长了近30%。他们的专业服务让我们印象深刻。</p>
            <div class="flex items-center">
              <img src="https://picsum.photos/id/1011/100/100" alt="客户头像" class="w-12 h-12 rounded-full mr-4">
              <div>
                <h4 class="font-bold">李婷</h4>
                <p class="text-gray-500 text-sm">某电商平台产品总监</p>
              </div>
            </div>
          </div>
          
          <!-- 评价3 -->
          <div class="bg-light p-8 rounded-2xl shadow-sm relative card-hover">
            <div class="text-primary text-6xl absolute top-6 right-6 opacity-20">
              <i class="fa fa-quote-right"></i>
            </div>
            <div class="flex text-yellow-400 mb-4">
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star-half-o"></i>
            </div>
            <p class="text-gray-600 mb-6 relative z-10">创新科技的网络安全服务为我们提供了全方位的保护，让我们能够专注于核心业务发展。他们的响应速度非常快，任何问题都能得到及时解决。</p>
            <div class="flex items-center">
              <img src="https://picsum.photos/id/1012/100/100" alt="客户头像" class="w-12 h-12 rounded-full mr-4">
              <div>
                <h4 class="font-bold">王强</h4>
                <p class="text-gray-500 text-sm">某金融机构信息安全负责人</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 联系表单 -->
    <section id="contact" class="py-20 bg-gray-50">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="bg-white rounded-3xl shadow-xl overflow-hidden">
          <div class="grid grid-cols-1 lg:grid-cols-2">
            <div class="p-8 md:p-12 lg:p-16">
              <span class="inline-block px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full mb-4">联系我们</span>
              <h2 class="text-[clamp(1.8rem,4vw,2.5rem)] font-bold mb-6">让我们一起探讨您的需求</h2>
              <p class="text-gray-600 mb-8">无论您有任何疑问或需求，都可以通过以下方式联系我们，我们的专业团队会尽快回复您。</p>
              
              <form class="space-y-6">
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                  <div>
                    <label for="name" class="block text-sm font-medium text-gray-700 mb-1">姓名</label>
                    <input type="text" id="name" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-primary focus:border-primary transition-all" placeholder="请输入您的姓名">
                  </div>
                  <div>
                    <label for="email" class="block text-sm font-medium text-gray-700 mb-1">邮箱</label>
                    <input type="email" id="email" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-primary focus:border-primary transition-all" placeholder="请输入您的邮箱">
                  </div>
                </div>
                
                <div>
                  <label for="company" class="block text-sm font-medium text-gray-700 mb-1">公司名称</label>
                  <input type="text" id="company" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-primary focus:border-primary transition-all" placeholder="请输入您的公司名称">
                </div>
                
                <div>
                  <label for="service" class="block text-sm font-medium text-gray-700 mb-1">感兴趣的服务</label>
                  <select id="service" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-primary focus:border-primary transition-all">
                    <option value="" selected disabled>请选择服务类型</option>
                    <option value="cloud">云计算服务</option>
                    <option value="ai">人工智能解决方案</option>
                    <option value="bigdata">大数据分析</option>
                    <option value="blockchain">区块链技术</option>
                    <option value="iot">物联网解决方案</option>
                    <option value="security">网络安全服务</option>
                  </select>
                </div>
                
                <div>
                  <label for="message" class="block text-sm font-medium text-gray-700 mb-1">留言</label>
                  <textarea id="message" rows="4" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-primary focus:border-primary transition-all" placeholder="请详细描述您的需求..."></textarea>
                </div>
                
                <button type="submit" class="w-full bg-primary hover:bg-primary/90 text-white px-6 py-3 rounded-lg transition-all shadow-md hover:shadow-lg font-medium">
                  提交信息
                </button>
              </form>
            </div>
            
            <div class="bg-primary p-8 md:p-12 lg:p-16 text-white">
              <h3 class="text-2xl font-bold mb-8">联系方式</h3>
              
              <div class="space-y-6">
                <div class="flex items-start">
                  <div class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center mr-4 flex-shrink-0">
                    <i class="fa fa-map-marker"></i>
                  </div>
                  <div>
                    <h4 class="font-medium mb-1">公司地址</h4>
                    <p class="text-white/80">北京市海淀区中关村科技园区8号楼15层</p>
                  </div>
                </div>
                
                <div class="flex items-start">
                  <div class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center mr-4 flex-shrink-0">
                    <i class="fa fa-phone"></i>
                  </div>
                  <div>
                    <h4 class="font-medium mb-1">联系电话</h4>
                    <p class="text-white/80">400-123-4567</p>
                  </div>
                </div>
                
                <div class="flex items-start">
                  <div class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center mr-4 flex-shrink-0">
                    <i class="fa fa-envelope"></i>
                  </div>
                  <div>
                    <h4 class="font-medium mb-1">电子邮箱</h4>
                    <p class="text-white/80">contact@innovtech.com</p>
                  </div>
                </div>
                
                <div class="flex items-start">
                  <div class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center mr-4 flex-shrink-0">
                    <i class="fa fa-clock-o"></i>
                  </div>
                  <div>
                    <h4 class="font-medium mb-1">工作时间</h4>
                    <p class="text-white/80">周一至周五: 9:00 - 18:00</p>
                    <p class="text-white/80">周六至周日: 休息</p>
                  </div>
                </div>
              </div>
              
              <div class="mt-12">
                <h4 class="font-medium mb-4">关注我们</h4>
                <div class="flex space-x-4">
                  <a href="#" class="w-10 h-10 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center transition-colors">
                    <i class="fa fa-weixin"></i>
                  </a>
                  <a href="#" class="w-10 h-10 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center transition-colors">
                    <i class="fa fa-weibo"></i>
                  </a>
                  <a href="#" class="w-10 h-10 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center transition-colors">
                    <i class="fa fa-linkedin"></i>
                  </a>
                  <a href="#" class="w-10 h-10 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center transition-colors">
                    <i class="fa fa-github"></i>
                  </a>
                </div>
              </div>
              
              <div class="mt-12 p-6 bg-white/10 rounded-xl">
                <h4 class="font-medium mb-2">免费咨询</h4>
                <p class="text-white/80 mb-4">我们提供免费的初步咨询服务，帮助您了解最适合的解决方案。</p>
                <a href="tel:4001234567" class="inline-flex items-center font-medium hover:underline">
                  立即拨打: 400-123-4567
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <!-- 页脚 -->
  <footer class="bg-dark text-white pt-16 pb-8">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 mb-12">
        <div>
          <a href="#" class="flex items-center space-x-2 mb-6">
            <div class="w-10 h-10 rounded-full bg-white flex items-center justify-center">
              <i class="fa fa-rocket text-primary text-xl"></i>
            </div>
            <span class="text-xl font-bold">创新科技</span>
          </a>
          <p class="text-gray-400 mb-6">我们致力于为企业提供前沿的技术解决方案，助力企业数字化转型，提升核心竞争力。</p>
          <div class="flex space-x-4">
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <i class="fa fa-weixin text-xl"></i>
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <i class="fa fa-weibo text-xl"></i>
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <i class="fa fa-linkedin text-xl"></i>
            </a>
            <a href="#" class="text-gray-400 hover:text-white transition-colors">
              <i class="fa fa-github text-xl"></i>
            </a>
          </div>
        </div>
        
        <div>
          <h4 class="text-lg font-bold mb-6">服务</h4>
          <ul class="space-y-3">
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">云计算服务</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">人工智能解决方案</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">大数据分析</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">区块链技术</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">物联网解决方案</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">网络安全服务</a></li>
          </ul>
        </div>
        
        <div>
          <h4 class="text-lg font-bold mb-6">公司</h4>
          <ul class="space-y-3">
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">关于我们</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">团队介绍</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">成功案例</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">新闻动态</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">加入我们</a></li>
            <li><a href="#" class="text-gray-400 hover:text-white transition-colors">联系我们</a></li>
          </ul>
        </div>
        
        <div>
          <h4 class="text-lg font-bold mb-6">订阅资讯</h4>
          <p class="text-gray-400 mb-4">订阅我们的资讯，获取最新的技术动态和行业洞察。</p>
          <form class="flex">
            <input type="email" placeholder="您的邮箱地址" class="px-4 py-2 rounded-l-lg w-full focus:outline-none text-dark">
            <button type="submit" class="bg-primary hover:bg-primary/90 text-white px-4 py-2 rounded-r-lg transition-colors">
              <i class="fa fa-paper-plane"></i>
            </button>
          </form>
        </div>
      </div>
      
      <div class="border-t border-gray-800 pt-8">
        <div class="flex flex-col md:flex-row justify-between items-center">
          <p class="text-gray-400 text-sm mb-4 md:mb-0">© 2023 创新科技有限公司. 保留所有权利.</p>
          <div class="flex space-x-6">
            <a href="#" class="text-gray-400 hover:text-white text-sm transition-colors">隐私政策</a>
            <a href="#" class="text-gray-400 hover:text-white text-sm transition-colors">服务条款</a>
            <a href="#" class="text-gray-400 hover:text-white text-sm transition-colors">Cookie政策</a>
          </div>
        </div>
      </div>
    </div>
  </footer>

  <!-- 返回顶部按钮 -->
  <button id="back-to-top" class="fixed bottom-8 right-8 bg-primary text-white w-12 h-12 rounded-full flex items-center justify-center shadow-lg opacity-0 invisible transition-all z-50">
    <i class="fa fa-arrow-up"></i>
  </button>

  <!-- JavaScript -->
  <script>
    // 导航栏滚动效果
    const navbar = document.getElementById('navbar');
    const backToTop = document.getElementById('back-to-top');
    
    window.addEventListener('scroll', function() {
      if (window.scrollY > 100) {
        navbar.classList.add('py-2', 'shadow-md');
        navbar.classList.remove('py-4', 'shadow-sm');
        backToTop.classList.remove('opacity-0', 'invisible');
        backToTop.classList.add('opacity-100', 'visible');
      } else {
        navbar.classList.add('py-4', 'shadow-sm');
        navbar.classList.remove('py-2', 'shadow-md');
        backToTop.classList.add('opacity-0', 'invisible');
        backToTop.classList.remove('opacity-100', 'visible');
      }
    });
    
    // 移动端菜单切换
    const menuToggle = document.getElementById('menu-toggle');
    const mobileMenu = document.getElementById('mobile-menu');
    
    menuToggle.addEventListener('click', function() {
      if (mobileMenu.classList.contains('h-0')) {
        mobileMenu.classList.remove('h-0', 'overflow-hidden');
        mobileMenu.classList.add('h-auto', 'overflow-visible');
        menuToggle.innerHTML = '<i class="fa fa-times text-2xl"></i>';
      } else {
        mobileMenu.classList.add('h-0', 'overflow-hidden');
        mobileMenu.classList.remove('h-auto', 'overflow-visible');
        menuToggle.innerHTML = '<i class="fa fa-bars text-2xl"></i>';
      }
    });
    
    // 平滑滚动
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        
        // 关闭移动端菜单
        if (!mobileMenu.classList.contains('h-0')) {
          mobileMenu.classList.add('h-0', 'overflow-hidden');
          mobileMenu.classList.remove('h-auto', 'overflow-visible');
          menuToggle.innerHTML = '<i class="fa fa-bars text-2xl"></i>';
        }
        
        const targetId = this.getAttribute('href');
        const targetElement = document.querySelector(targetId);
        
        if (targetElement) {
          window.scrollTo({
            top: targetElement.offsetTop - 80,
            behavior: 'smooth'
          });
        }
      });
    });
    
    // 返回顶部按钮
    backToTop.addEventListener('click', function() {
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      });
    });
    
    // 数字计数器动画
    const counters = document.querySelectorAll('.counter');
    const speed = 200;
    
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          const counter = entry.target;
          const target = +counter.getAttribute('data-target');
          const count = +counter.innerText;
          const increment = target / speed;
          
          if (count < target) {
            counter.innerText = Math.ceil(count + increment);
            setTimeout(() => {
              counter.innerText = Math.ceil(count + increment);
            }, 1);
          } else {
            counter.innerText = target;
            observer.unobserve(counter);
          }
        }
      });
    }, { threshold: 0.5 });
    
    counters.forEach(counter => {
      observer.observe(counter);
    });
    
    // 表单提交处理
    const form = document.querySelector('form');
    if (form) {
      form.addEventListener('submit', function(e) {
        e.preventDefault();
        // 这里可以添加表单验证和提交逻辑
        alert('表单提交成功！我们会尽快与您联系。');
        form.reset();
      });
    }
  </script>
</body>
</html>
# Administrator.github.io
我的个人网站
