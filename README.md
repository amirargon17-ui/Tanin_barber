<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>آرایشگاه طنین | استایل حرفه‌ای</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@100;400;700&display=swap');

        body {
            font-family: 'Vazirmatn', sans-serif;
            background-color: #1a1a1a;
            color: #e0e0e0;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
        }

        .container {
            background: linear-gradient(145deg, #2c2c2c, #121212);
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            border: 1px solid #d4af37; /* رنگ طلایی */
            max-width: 400px;
            width: 90%;
        }

        h1 {
            color: #d4af37;
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .info-box {
            margin: 20px 0;
            padding: 15px;
            background: rgba(212, 175, 55, 0.1);
            border-radius: 10px;
        }

        .price-tag {
            font-size: 1.5rem;
            color: #fff;
            font-weight: bold;
        }

        .hours {
            color: #aaa;
            font-style: italic;
        }

        .contact-info {
            margin-top: 30px;
            font-size: 0.9rem;
            border-top: 1px solid #444;
            padding-top: 20px;
        }

        .contact-info p {
            margin: 5px 0;
        }

        .highlight {
            color: #d4af37;
            font-weight: bold;
        }

        .btn {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 25px;
            background-color: #d4af37;
            color: #000;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            transform: scale(1.05);
            background-color: #fff;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>آرایشگاه طنین</h1>
    <p>تغییر چهره، بازسازی استایل</p>

    <div class="info-box">
        <p>قیمت اصلاح مو امروز:</p>
        <div class="price-tag" id="random-price">---</div>
    </div>

    <div class="info-box">
        <p>ساعت کاری امروز:</p>
        <div class="hours" id="random-hours">---</div>
    </div>

    <div class="contact-info">
        <p>🆔 آی‌دی تلگرام: <span class="highlight" id="random-id">---</span></p>
        <p>📞 شماره تماس: <span class="highlight" id="random-phone">---</span></p>
    </div>

    <a href="#" class="btn">رزرو نوبت</a>
</div>

<script>
    // تابع برای تولید اعداد رندوم
    function getRandomInt(min, max) {
        return Math.floor(Math.random() * (max - min + 1)) + min;
    }

    // رندوم کردن قیمت (مثلاً بین ۵۰ تا ۱۵۰ هزار تومان)
    const price = getRandomInt(50, 150);
    document.getElementById('random-price').innerText = price + ' هزار تومان';

    // رندوم کردن ساعت کاری
    const startHour = getRandomInt(9, 12);
    const endHour = getRandomInt(18, 22);
    document.getElementById('random-hours').innerText = `${startHour}:00 الی ${endHour}:00`;

    // رندوم کردن آی‌دی تلگرام
    const randomId = 'Taneen_' + getRandomInt(1000, 9999);
    document.getElementById('random-id').innerText = '@' + randomId;

    // رندوم کردن شماره تماس
    const phone = '09' + getRandomInt(10000000, 99999999);
    document.getElementById('random-phone').innerText = phone;
</script>

</body>
</html>
