<!DOCTYPE html>
<html>
<head>
    <style>
        .heart { position: absolute; color: pink; animation: fall 3s linear infinite; }
        @keyframes fall { to { transform: translateY(100vh) rotate(360deg); } }
    </style>
</head>
<body style="background: linear-gradient(120deg, #ff9a9e, #fad0c4); height: 100vh;">
    <h2 style="text-align: center; padding-top: 20%;">💖 专属娟的甜蜜收容所 💖</h2>
    <div id="messages"></div>
</body>
<script>
    const messages = ["检测到可爱能量超标！", "正在生成拥抱请求...", "系统提示：你值得被无限偏爱"];
    setInterval(() => {
        const heart = document.createElement('div');
        heart.className = 'heart';
        heart.innerHTML = '❤️';
        heart.style.left = Math.random() * 100 + 'vw';
        document.body.appendChild(heart);
        setTimeout(() => heart.remove(), 3000);
    }, 300);
</script>
</html>