# Jalal
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>صفحة شخصية</title>
    <style>
        /* أسلوب الألوان الأنيقة القديمة */
        body {
            font-family: Arial, sans-serif;
            background-color: #f3efe2;
            color: #3e2c1c;
            text-align: center;
            padding: 20px;
        }
        h1 {
            color: #3e2c1c;
            font-size: 2.5em;
            margin-bottom: 0.5em;
        }
        p {
            font-size: 1.2em;
            margin-bottom: 1em;
        }
        .social-links {
            margin-top: 20px;
        }
        .social-links a {
            text-decoration: none;
            color: #3e2c1c;
            font-size: 1.5em;
            margin: 0 10px;
        }
        .resume-button {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #8b6d42;
            color: white;
            font-size: 1.2em;
            border: none;
            cursor: pointer;
            text-decoration: none;
        }
        .resume-button:hover {
            background-color: #3e2c1c;
        }
        .emoji-section {
            margin-top: 20px;
            display: none; /* فقط أنت يمكنك مشاهدة التفاعلات */
        }
        .emoji {
            font-size: 2em;
            cursor: pointer;
            margin: 0 10px;
        }
    </style>
    <script>
        function toggleEmojiSection() {
            const emojiSection = document.getElementById("emoji-section");
            emojiSection.style.display = emojiSection.style.display === "none" ? "block" : "none";
        }

        function addReaction(emoji) {
            const reactions = document.getElementById("reactions");
            reactions.innerHTML += emoji + " ";
        }
    </script>
</head>
<body>
    <h1>مرحباً بكم في صفحة جلال</h1>
    <p>مرحبًا بكم في موقعي الشخصي، يمكنكم متابعة حساباتي والتفاعل بإيموجي إن أحببتم!</p>

    <!-- روابط وسائل التواصل الاجتماعي -->
    <div class="social-links">
        <a href="https://www.facebook.com/share/18CqCcUVXU/?mibextid=LQQJ4d" target="_blank">🔗 فيسبوك</a>
        <a href="https://x.com/jalalyass19?s=21" target="_blank">🔗 تويتر</a>
        <a href="https://www.instagram.com/0jlal/profilecard/?igsh=YjVtZW1xNnozcnBp" target="_blank">🔗 الانستغرام</a>

    </div>

    <!-- زر تحميل السيرة الذاتية -->
    <a href="#" class="resume-button">تحميل السيرة الذاتية</a>

    <!-- قسم التفاعل بإيموجي -->
    <div class="emoji-section" id="emoji-section">
        <h2>التفاعل بإيموجي</h2>
        <span class="emoji" onclick="addReaction('😊')">😊</span>
        <span class="emoji" onclick="addReaction('👍')">👍</span>
        <span class="emoji" onclick="addReaction('❤️')">❤️</span>
        <div id="reactions" style="margin-top: 10px;"></div>
    </div>

    <button onclick="toggleEmojiSection()">تفعيل / إخفاء قسم الإيموجي</button>
</body>
</html>
