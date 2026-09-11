# new-web1
new project html sport site
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>فروشگاه من</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: Tahoma, sans-serif;
            background: #f5f5f5;
            color: #333;
        }
        header {
            background: #111;
            color: white;
            padding: 22px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        header h1 {
            font-size: 26px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin-right: 20px;
        }
        nav a:hover {
            color: #00c853;
        }
        /* بخش اصلی */
        .hero {
            text-align: center;
            padding: 80px 20px;
            background: linear-gradient(135deg, #00c853, #64dd17);
            color: white;
        }
        .hero h2 {
            font-size: 40px;
            margin-bottom: 15px;
        }
        .hero p {
            font-size: 18px;
        }
        .hero button {
            margin-top: 25px;
            padding: 12px 30px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-size: 16px;
        }

        /* محصولات */

        .products {
            width: 90%;
            max-width: 1100px;
            margin: 50px auto;
        }

        .products h2 {
            text-align: center;
            margin-bottom: 30px;
        }

        .product-container {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
        }

        .product {
            width: 280px;
            background: white;
            border-radius: 15px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: 0.3s;
        }

        .product:hover {
            transform: translateY(-10px);
        }

        .product .image {
            height: 170px;
            background: #eee;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            margin-bottom: 15px;
        }

        .product h3 {
            margin-bottom: 10px;
        }

        .price {
            color: #00a844;
            font-size: 20px;
            font-weight: bold;
            margin: 15px;
        }

        .buy {
            background: #111;
            color: white;
            border: none;
            padding: 10px 25px;
            border-radius: 20px;
            cursor: pointer;
        }

        .buy:hover {
            background: #00c853;
        }

        /* فوتر */

        footer {
            background: #111;
            color: white;
            text-align: center;
            padding: 25px;
            margin-top: 50px;
        }

        /* موبایل */

        @media (max-width: 700px) {

            header {
                flex-direction: column;
                gap: 15px;
            }

            .hero h2 {
                font-size: 30px;
            }

            nav a {
                margin: 5px;
            }
        }
    </style>
</head>

<body>

    <!-- هدر -->

    <header>

        <h1>🛍️ فروشگاه من</h1>

        <nav>
            <a href="#">خانه</a>
            <a href="#">محصولات</a>
            <a href="#">درباره ما</a>
            <a href="#">تماس</a>
        </nav>

    </header>


    <!-- بخش معرفی -->

    <section class="hero">

        <h2>به فروشگاه ما خوش آمدید</h2>

        <p>
            بهترین محصولات با بهترین قیمت
        </p>

        <button onclick="showMessage()">
            مشاهده محصولات
        </button>

    </section>


    <!-- محصولات -->

    <section class="products">

        <h2>محصولات محبوب</h2>

        <div class="product-container">


            <div class="product">

                <div class="image">
                    📱
                </div>

                <h3>گوشی هوشمند</h3>

                <p>
                    یک گوشی مدرن و قدرتمند
                </p>

                <div class="price">
                    25,000,000 تومان
                </div>

                <button class="buy"
                    onclick="buyProduct('گوشی هوشمند')">
                    خرید
                </button>

            </div>


            <div class="product">

                <div class="image">
                    💻
                </div>

                <h3>لپ‌تاپ</h3>

                <p>
                    مناسب کار و استفاده روزمره
                </p>

                <div class="price">
                    45,000,000 تومان
                </div>

                <button class="buy"
                    onclick="buyProduct('لپ‌تاپ')">
                    خرید
                </button>

            </div>


            <div class="product">

                <div class="image">
                    🎧
                </div>

                <h3>هدفون</h3>

                <p>
                    صدای باکیفیت و طراحی زیبا
                </p>

                <div class="price">
                    2,500,000 تومان
                </div>

                <button class="buy"
                    onclick="buyProduct('هدفون')">
                    خرید
                </button>

            </div>


        </div>

    </section>


    <!-- فوتر -->

    <footer>

        <p>
            © 2026 فروشگاه من | تمامی حقوق محفوظ است
        </p>

    </footer>


    <!-- JavaScript -->

    <script>

        function showMessage() {

            alert("به بخش محصولات خوش آمدید 🛍️");

        }

        function buyProduct(product) {

            alert(
                "شما محصول «" +
                product +
                "» را انتخاب کردید!"
            );

        }

    </script>

</body>
</html>
