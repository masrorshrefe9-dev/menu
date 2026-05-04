<!DOCTYPE html>
<html lang="ku" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>خارنگەها قادش یا فەرمی</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --primary: #ffcc00; --bg: #0b0b0b; --card: #1a1a1a; --text: #ffffff; }
        body { background-color: var(--bg); color: var(--text); font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; margin: 0; padding: 0; }
        
        /* Header Section */
        .header { text-align: center; padding: 60px 20px; background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1514933651103-005eec06c04b?w=800'); background-size: cover; background-position: center; border-bottom: 5px solid var(--primary); }
        .logo-circle { width: 100px; height: 100px; background: var(--primary); border-radius: 50%; display: flex; align-items: center; justify-content: center; margin: 0 auto 15px; font-size: 40px; color: black; border: 4px solid white; }
        .header h1 { margin: 10px 0; font-size: 2.5rem; text-shadow: 2px 2px 10px rgba(0,0,0,0.5); }
        .header p { color: #ccc; font-size: 1.1rem; }

        /* Categories Bar */
        .categories { display: flex; overflow-x: auto; padding: 20px; gap: 15px; background: #111; position: sticky; top: 0; z-index: 1000; scrollbar-width: none; border-bottom: 1px solid #333; }
        .categories::-webkit-scrollbar { display: none; }
        .cat-btn { background: var(--card); border: 2px solid #333; color: white; padding: 10px 25px; border-radius: 30px; white-space: nowrap; cursor: pointer; transition: 0.3s; display: flex; align-items: center; gap: 8px; }
        .cat-btn.active { background: var(--primary); color: black; border-color: var(--primary); font-weight: bold; }

        /* Menu Grid */
        .menu-grid { padding: 25px; display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 25px; max-width: 1200px; margin: 0 auto; }
        .item-card { background: var(--card); border-radius: 25px; overflow: hidden; border: 1px solid #222; transition: 0.4s; position: relative; box-shadow: 0 10px 20px rgba(0,0,0,0.3); }
        .item-card:hover { transform: translateY(-10px); border-color: var(--primary); }
        .item-img-wrapper { position: relative; width: 100%; height: 220px; }
        .item-img { width: 100%; height: 100%; object-fit: cover; }
        .price-tag { position: absolute; top: 15px; left: 15px; background: var(--primary); color: black; padding: 8px 15px; border-radius: 12px; font-weight: bold; font-size: 1.1rem; box-shadow: 0 4px 8px rgba(0,0,0,0.2); }
        
        .item-content { padding: 20px; }
        .item-content h3 { margin: 0 0 10px; font-size: 1.4rem; color: var(--primary); }
        .item-content p { color: #aaa; font-size: 0.95rem; line-height: 1.5; margin-bottom: 15px; }
        
        .order-btn { width: 100%; background: transparent; border: 2px solid var(--primary); color: var(--primary); padding: 10px; border-radius: 15px; font-weight: bold; cursor: pointer; transition: 0.3s; }
        .order-btn:hover { background: var(--primary); color: black; }

        /* Footer */
        .footer { text-align: center; padding: 40px; background: #050505; color: #666; margin-top: 50px; border-top: 1px solid #222; }
        .footer span { color: var(--primary); font-weight: bold; }
    </style>
</head>
<body>

    <div class="header">
        <div class="logo-circle"><i class="fas fa-utensils"></i></div>
        <h1>مەتعه‌مێ قادش 🍔</h1>
        <p>خارنێن خۆش و پاقژ ب دەستێن مەسروور شەریف</p>
    </div>

    <div class="categories">
        <div class="cat-btn active"><i class="fas fa-th-large"></i> هەمی</div>
        <div class="cat-btn"><i class="fas fa-hamburger"></i> بۆڕگەر</div>
        <div class="cat-btn"><i class="fas fa-pizza-slice"></i> پیتزا</div>
        <div class="cat-btn"><i class="fas fa-drumstick-bite"></i> مریشک</div>
        <div class="cat-btn"><i class="fas fa-coffee"></i> ڤەخوارن</div>
    </div>

    <div class="menu-grid">
        <div class="item-card">
            <div class="item-img-wrapper">
                <img class="item-img" src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?w=500" alt="بۆڕگەر">
                <div class="price-tag">6,000 IQD</div>
            </div>
            <div class="item-content">
                <h3>بۆڕگەر کلاسیک</h3>
                <p>گۆشتێ فرێش یێ جوان، پەنیرێ چێدەر، کاهو، سۆسا تایبەت</p>
                <button class="order-btn">داوا بکە</button>
            </div>
        </div>

        <div class="item-card">
            <div class="item-img-wrapper">
                <img class="item-img" src="https://images.unsplash.com/photo-1513104890138-7c749659a591?w=500" alt="پیتزا">
                <div class="price-tag">10,000 IQD</div>
            </div>
            <div class="item-content">
                <h3>پیتزا مارگێریتا</h3>
                <p>سۆسا تەماتێ یا ئیتاڵی، مۆزارێلا، ریحان، زەیت یێ زەیتوونێ</p>
                <button class="order-btn">داوا بکە</button>
            </div>
        </div>

        <div class="item-card">
            <div class="item-img-wrapper">
                <img class="item-img" src="https://images.unsplash.com/photo-1562967914-608f82629710?w=500" alt="مریشک">
                <div class="price-tag">8,500 IQD</div>
            </div>
            <div class="item-content">
                <h3>مریشکا برژاو</h3>
                <p>مریشکا کوردی یا فرێش ب تامەکا نایاب و سۆسا بیبەرێ</p>
                <button class="order-btn">داوا بکە</button>
            </div>
        </div>
    </div>

    <div class="footer">
        <p>دیزاین کراوە ژ لایێ <span>Masror Tech 🛡️</span></p>
        <p>© 2026 هەمی ماف پاراستینە بۆ مەتعه‌مێ قادش</p>
    </div>

</body>
</html>
