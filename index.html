<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>my store</title>
<script src="https://telegram.org/js/telegram-web-app.js"></script>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&display=swap" rel="stylesheet">
<style>
  :root {
    --primary: #2563eb;
    --primary-dark: #1d4ed8;
    --accent: #f59e0b;
    --bg: #f1f5f9;
    --card: #ffffff;
    --text: #0f172a;
    --muted: #64748b;
    --success: #10b981;
    --radius: 18px;
    --shadow: 0 4px 24px rgba(0,0,0,0.10);
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Cairo', sans-serif;
    background: var(--bg);
    color: var(--text);
    min-height: 100vh;
    padding-bottom: 100px;
  }

  /* ===== HEADER ===== */
  .header {
    background: linear-gradient(135deg, var(--primary) 0%, #1e40af 100%);
    color: white;
    padding: 22px 20px 28px;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 4px 20px rgba(37,99,235,0.3);
  }
  .header-top {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 16px;
  }
  .store-name {
    font-size: 22px;
    font-weight: 900;
    letter-spacing: -0.5px;
  }
  .cart-btn {
    background: rgba(255,255,255,0.2);
    border: none;
    border-radius: 12px;
    padding: 8px 14px;
    color: white;
    font-size: 18px;
    cursor: pointer;
    position: relative;
    backdrop-filter: blur(10px);
    transition: all 0.2s;
  }
  .cart-btn:active { transform: scale(0.95); }
  .cart-count {
    position: absolute;
    top: -6px;
    left: -6px;
    background: var(--accent);
    color: #000;
    font-size: 11px;
    font-weight: 700;
    width: 20px;
    height: 20px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    display: none;
  }

  /* ===== SEARCH ===== */
  .search-bar {
    background: rgba(255,255,255,0.15);
    border: 1px solid rgba(255,255,255,0.3);
    border-radius: 12px;
    padding: 10px 16px;
    color: white;
    font-size: 14px;
    font-family: 'Cairo', sans-serif;
    width: 100%;
    outline: none;
    backdrop-filter: blur(10px);
  }
  .search-bar::placeholder { color: rgba(255,255,255,0.6); }

  /* ===== CATEGORIES ===== */
  .categories {
    display: flex;
    gap: 10px;
    padding: 16px 20px;
    overflow-x: auto;
    scrollbar-width: none;
  }
  .categories::-webkit-scrollbar { display: none; }
  .cat-btn {
    background: var(--card);
    border: 2px solid transparent;
    border-radius: 30px;
    padding: 8px 18px;
    font-size: 13px;
    font-weight: 600;
    font-family: 'Cairo', sans-serif;
    cursor: pointer;
    white-space: nowrap;
    transition: all 0.2s;
    color: var(--muted);
    box-shadow: var(--shadow);
  }
  .cat-btn.active {
    background: var(--primary);
    color: white;
    border-color: var(--primary);
  }

  /* ===== SECTION TITLE ===== */
  .section-title {
    font-size: 18px;
    font-weight: 700;
    padding: 4px 20px 12px;
    color: var(--text);
  }

  /* ===== PRODUCTS GRID ===== */
  .products-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 14px;
    padding: 0 16px;
  }

  /* ===== PRODUCT CARD ===== */
  .product-card {
    background: var(--card);
    border-radius: var(--radius);
    overflow: hidden;
    box-shadow: var(--shadow);
    cursor: pointer;
    transition: transform 0.2s, box-shadow 0.2s;
    animation: fadeIn 0.4s ease both;
  }
  .product-card:active { transform: scale(0.97); }
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(16px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  .product-img {
    width: 100%;
    height: 150px;
    object-fit: cover;
    background: #e2e8f0;
    display: block;
  }
  .product-img-placeholder {
    width: 100%;
    height: 150px;
    background: linear-gradient(135deg, #e2e8f0, #cbd5e1);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 40px;
  }

  .product-info {
    padding: 12px;
  }
  .product-name {
    font-size: 14px;
    font-weight: 700;
    margin-bottom: 4px;
    line-height: 1.3;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    overflow: hidden;
  }
  .product-price {
    font-size: 16px;
    font-weight: 900;
    color: var(--primary);
    margin-bottom: 10px;
  }
  .product-price span {
    font-size: 12px;
    font-weight: 600;
    color: var(--muted);
  }
  .add-btn {
    width: 100%;
    background: var(--primary);
    color: white;
    border: none;
    border-radius: 10px;
    padding: 9px;
    font-size: 13px;
    font-weight: 700;
    font-family: 'Cairo', sans-serif;
    cursor: pointer;
    transition: background 0.2s;
  }
  .add-btn:active { background: var(--primary-dark); }

  /* ===== PRODUCT MODAL ===== */
  .overlay {
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.5);
    z-index: 200;
    opacity: 0;
    pointer-events: none;
    transition: opacity 0.3s;
    backdrop-filter: blur(4px);
  }
  .overlay.show { opacity: 1; pointer-events: all; }

  .modal {
    position: fixed;
    bottom: 0;
    left: 0; right: 0;
    background: var(--card);
    border-radius: 24px 24px 0 0;
    z-index: 300;
    transform: translateY(100%);
    transition: transform 0.35s cubic-bezier(0.32, 0.72, 0, 1);
    max-height: 90vh;
    overflow-y: auto;
  }
  .modal.show { transform: translateY(0); }

  .modal-handle {
    width: 40px;
    height: 4px;
    background: #e2e8f0;
    border-radius: 2px;
    margin: 12px auto;
  }
  .modal-img {
    width: 100%;
    height: 250px;
    object-fit: cover;
  }
  .modal-img-placeholder {
    width: 100%;
    height: 220px;
    background: linear-gradient(135deg, #e2e8f0, #cbd5e1);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 70px;
  }
  .modal-body { padding: 20px; }
  .modal-name { font-size: 22px; font-weight: 900; margin-bottom: 8px; }
  .modal-price { font-size: 24px; font-weight: 900; color: var(--primary); margin-bottom: 14px; }
  .modal-desc { font-size: 14px; color: var(--muted); line-height: 1.8; margin-bottom: 20px; }

  .qty-control {
    display: flex;
    align-items: center;
    gap: 16px;
    margin-bottom: 20px;
    background: var(--bg);
    border-radius: 14px;
    padding: 8px 16px;
    width: fit-content;
  }
  .qty-btn {
    background: var(--primary);
    color: white;
    border: none;
    width: 32px; height: 32px;
    border-radius: 8px;
    font-size: 18px;
    cursor: pointer;
    display: flex; align-items: center; justify-content: center;
    font-family: 'Cairo', sans-serif;
  }
  .qty-num { font-size: 18px; font-weight: 700; min-width: 24px; text-align: center; }

  .modal-add-btn {
    width: 100%;
    background: linear-gradient(135deg, var(--primary), var(--primary-dark));
    color: white;
    border: none;
    border-radius: 14px;
    padding: 16px;
    font-size: 16px;
    font-weight: 700;
    font-family: 'Cairo', sans-serif;
    cursor: pointer;
    box-shadow: 0 4px 16px rgba(37,99,235,0.35);
  }

  /* ===== CART MODAL ===== */
  .cart-item {
    display: flex;
    align-items: center;
    gap: 14px;
    padding: 14px 0;
    border-bottom: 1px solid #f1f5f9;
  }
  .cart-item-emoji { font-size: 30px; flex-shrink: 0; }
  .cart-item-info { flex: 1; }
  .cart-item-name { font-size: 14px; font-weight: 700; }
  .cart-item-price { font-size: 13px; color: var(--muted); }
  .cart-item-remove {
    background: #fee2e2;
    color: #ef4444;
    border: none;
    border-radius: 8px;
    width: 30px; height: 30px;
    font-size: 14px;
    cursor: pointer;
    font-family: 'Cairo', sans-serif;
  }

  .cart-total {
    background: var(--bg);
    border-radius: 14px;
    padding: 16px;
    margin: 16px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .cart-total-label { font-size: 16px; font-weight: 600; color: var(--muted); }
  .cart-total-price { font-size: 22px; font-weight: 900; color: var(--primary); }

  /* ===== ORDER FORM ===== */
  .order-form { display: none; }
  .order-form.show { display: block; }
  .form-label {
    font-size: 13px;
    font-weight: 700;
    color: var(--muted);
    margin-bottom: 6px;
    display: block;
  }
  .form-input {
    width: 100%;
    background: var(--bg);
    border: 2px solid transparent;
    border-radius: 12px;
    padding: 12px 16px;
    font-size: 15px;
    font-family: 'Cairo', sans-serif;
    outline: none;
    margin-bottom: 14px;
    transition: border-color 0.2s;
    color: var(--text);
  }
  .form-input:focus { border-color: var(--primary); }

  /* ===== SUCCESS ===== */
  .success-screen {
    text-align: center;
    padding: 40px 20px;
    display: none;
  }
  .success-screen.show { display: block; }
  .success-icon { font-size: 64px; margin-bottom: 16px; }
  .success-title { font-size: 22px; font-weight: 900; margin-bottom: 8px; color: var(--success); }
  .success-msg { font-size: 14px; color: var(--muted); line-height: 1.8; }

  /* ===== TOAST ===== */
  .toast {
    position: fixed;
    bottom: 90px;
    left: 50%;
    transform: translateX(-50%) translateY(20px);
    background: #0f172a;
    color: white;
    padding: 12px 24px;
    border-radius: 30px;
    font-size: 14px;
    font-weight: 600;
    z-index: 500;
    opacity: 0;
    transition: all 0.3s;
    white-space: nowrap;
  }
  .toast.show { opacity: 1; transform: translateX(-50%) translateY(0); }
</style>
</head>
<body>

<!-- ===========================
     ✏️ بيانات المتجر — عدّل هنا
     =========================== -->
<script>
const STORE = {
  name: "🛍️ متجري",           // ← اسم متجرك
  currency: "ر.س",             // ← العملة
};

// ✏️ أضف منتجاتك هنا
// emoji: أي إيموجي إذا ما عندك صورة
// image: رابط صورة المنتج (اتركه "" إذا تستخدم الإيموجي)
// category: "الكل" أو اسم فئة

const PRODUCTS = [
  {
    id: 1,
    name: "سماعات لاسلكية",
    description: "سماعات بلوتوث عالية الجودة مع عزل للضوضاء وبطارية تدوم 30 ساعة. صوت نقي ومميز لتجربة استماع لا مثيل لها.",
    price: 150,
    emoji: "🎧",
    image: "",            // ← ضع رابط الصورة هنا
    category: "إلكترونيات"
  },
  {
    id: 2,
    name: "ساعة ذكية",
    description: "ساعة ذكية متعددة المهام مع قياس ضغط الدم ونبضات القلب. GPS مدمج ومقاومة للماء حتى 50 متر.",
    price: 299,
    emoji: "⌚",
    image: "",
    category: "إلكترونيات"
  },
  {
    id: 3,
    name: "حقيبة جلدية",
    description: "حقيبة من الجلد الطبيعي الفاخر 100%. تصميم أنيق يناسب كل المناسبات مع مساحة واسعة وأقسام منظمة.",
    price: 200,
    emoji: "👜",
    image: "",
    category: "أزياء"
  },
  {
    id: 4,
    name: "نظارة شمسية",
    description: "نظارة شمسية بحماية UV400 كاملة. إطار خفيف وعصري مناسب لجميع أشكال الوجوه.",
    price: 89,
    emoji: "🕶️",
    image: "",
    category: "أزياء"
  },
  {
    id: 5,
    name: "عطر فاخر",
    description: "عطر رجالي/نسائي بتركيبة فرنسية حصرية. رائحة تدوم طوال اليوم وتترك أثراً لا يُنسى.",
    price: 180,
    emoji: "🌸",
    image: "",
    category: "عناية"
  },
  {
    id: 6,
    name: "كريم مرطب",
    description: "كريم مرطب فاخر يحتوي على مستخلصات طبيعية. يغذي البشرة ويمنحها نضارة ملحوظة من الاستخدام الأول.",
    price: 65,
    emoji: "🧴",
    image: "",
    category: "عناية"
  },
];
// ==========================
//  نهاية التعديلات
// ==========================
</script>

<!-- HEADER -->
<div class="header">
  <div class="header-top">
    <div class="store-name" id="storeName"></div>
    <button class="cart-btn" onclick="openCart()">
      🛒 <span class="cart-count" id="cartCount">0</span>
    </button>
  </div>
  <input class="search-bar" placeholder="🔍 ابحث عن منتج..." oninput="searchProducts(this.value)">
</div>

<!-- CATEGORIES -->
<div class="categories" id="categories"></div>

<!-- PRODUCTS -->
<div class="section-title" id="sectionTitle">جميع المنتجات</div>
<div class="products-grid" id="productsGrid"></div>

<!-- OVERLAY -->
<div class="overlay" id="overlay" onclick="closeAll()"></div>

<!-- PRODUCT MODAL -->
<div class="modal" id="productModal">
  <div class="modal-handle"></div>
  <div id="modalImgWrap"></div>
  <div class="modal-body">
    <div class="modal-name" id="modalName"></div>
    <div class="modal-price" id="modalPrice"></div>
    <div class="modal-desc" id="modalDesc"></div>
    <div class="qty-control">
      <button class="qty-btn" onclick="changeQty(-1)">−</button>
      <div class="qty-num" id="qtyNum">1</div>
      <button class="qty-btn" onclick="changeQty(1)">+</button>
    </div>
    <button class="modal-add-btn" onclick="addToCartFromModal()">🛒 أضف للسلة</button>
  </div>
</div>

<!-- CART MODAL -->
<div class="modal" id="cartModal">
  <div class="modal-handle"></div>
  <div class="modal-body">
    <!-- Cart View -->
    <div id="cartView">
      <div class="modal-name">🛒 السلة</div>
      <div id="cartItems"></div>
      <div class="cart-total">
        <div class="cart-total-label">الإجمالي</div>
        <div class="cart-total-price" id="cartTotal">0 ر.س</div>
      </div>
      <button class="modal-add-btn" onclick="goToOrder()">المتابعة للطلب ←</button>
    </div>

    <!-- Order Form -->
    <div class="order-form" id="orderForm">
      <div class="modal-name">📦 بيانات التوصيل</div>
      <br>
      <label class="form-label">الاسم الكامل</label>
      <input class="form-input" id="fName" placeholder="مثال: أحمد محمد">
      <label class="form-label">رقم الهاتف</label>
      <input class="form-input" id="fPhone" placeholder="05xxxxxxxx" type="tel">
      <label class="form-label">المدينة</label>
      <input class="form-input" id="fCity" placeholder="مثال: الرياض">
      <label class="form-label">العنوان بالتفصيل</label>
      <input class="form-input" id="fAddress" placeholder="الحي، الشارع، رقم المبنى">
      <button class="modal-add-btn" onclick="submitOrder()">✅ تأكيد الطلب</button>
    </div>

    <!-- Success -->
    <div class="success-screen" id="successScreen">
      <div class="success-icon">🎉</div>
      <div class="success-title">تم استلام طلبك!</div>
      <div class="success-msg">شكراً لك! سيتم التواصل معك قريباً على رقمك لتأكيد الطلب والتوصيل.</div>
    </div>
  </div>
</div>

<!-- TOAST -->
<div class="toast" id="toast"></div>

<script>
// Init Telegram
const tg = window.Telegram?.WebApp;
if (tg) { tg.ready(); tg.expand(); }

// State
let cart = [];
let currentProduct = null;
let currentQty = 1;
let activeCategory = "الكل";

// Init
document.getElementById("storeName").textContent = STORE.name;
buildCategories();
renderProducts(PRODUCTS);

// ===== CATEGORIES =====
function buildCategories() {
  const cats = ["الكل", ...new Set(PRODUCTS.map(p => p.category))];
  const wrap = document.getElementById("categories");
  cats.forEach(c => {
    const btn = document.createElement("button");
    btn.className = "cat-btn" + (c === "الكل" ? " active" : "");
    btn.textContent = c;
    btn.onclick = () => filterCategory(c, btn);
    wrap.appendChild(btn);
  });
}

function filterCategory(cat, btn) {
  activeCategory = cat;
  document.querySelectorAll(".cat-btn").forEach(b => b.classList.remove("active"));
  btn.classList.add("active");
  const filtered = cat === "الكل" ? PRODUCTS : PRODUCTS.filter(p => p.category === cat);
  document.getElementById("sectionTitle").textContent = cat === "الكل" ? "جميع المنتجات" : cat;
  renderProducts(filtered);
}

// ===== RENDER =====
function renderProducts(list) {
  const grid = document.getElementById("productsGrid");
  grid.innerHTML = "";
  list.forEach((p, i) => {
    const card = document.createElement("div");
    card.className = "product-card";
    card.style.animationDelay = (i * 0.07) + "s";
    card.innerHTML = `
      ${p.image
        ? `<img class="product-img" src="${p.image}" alt="${p.name}" onerror="this.style.display='none';this.nextElementSibling.style.display='flex'">`
        : ''}
      <div class="product-img-placeholder" style="${p.image ? 'display:none' : ''}">${p.emoji}</div>
      <div class="product-info">
        <div class="product-name">${p.name}</div>
        <div class="product-price">${p.price} <span>${STORE.currency}</span></div>
        <button class="add-btn" onclick="event.stopPropagation(); quickAdd(${p.id})">+ أضف للسلة</button>
      </div>`;
    card.onclick = () => openProduct(p.id);
    grid.appendChild(card);
  });
}

// ===== SEARCH =====
function searchProducts(q) {
  const filtered = PRODUCTS.filter(p =>
    p.name.includes(q) || p.description.includes(q)
  );
  renderProducts(filtered);
}

// ===== PRODUCT MODAL =====
function openProduct(id) {
  currentProduct = PRODUCTS.find(p => p.id === id);
  currentQty = 1;
  document.getElementById("qtyNum").textContent = 1;
  document.getElementById("modalName").textContent = currentProduct.name;
  document.getElementById("modalPrice").textContent = currentProduct.price + " " + STORE.currency;
  document.getElementById("modalDesc").textContent = currentProduct.description;

  const imgWrap = document.getElementById("modalImgWrap");
  imgWrap.innerHTML = currentProduct.image
    ? `<img class="modal-img" src="${currentProduct.image}" alt="${currentProduct.name}">`
    : `<div class="modal-img-placeholder">${currentProduct.emoji}</div>`;

  showModal("productModal");
}

function changeQty(d) {
  currentQty = Math.max(1, currentQty + d);
  document.getElementById("qtyNum").textContent = currentQty;
}

function addToCartFromModal() {
  if (!currentProduct) return;
  addToCart(currentProduct, currentQty);
  closeAll();
}

function quickAdd(id) {
  const p = PRODUCTS.find(x => x.id === id);
  addToCart(p, 1);
}

// ===== CART =====
function addToCart(product, qty) {
  const existing = cart.find(i => i.id === product.id);
  if (existing) existing.qty += qty;
  else cart.push({ ...product, qty });
  updateCartCount();
  showToast(`✅ تمت الإضافة: ${product.name}`);
}

function updateCartCount() {
  const total = cart.reduce((s, i) => s + i.qty, 0);
  const badge = document.getElementById("cartCount");
  badge.textContent = total;
  badge.style.display = total > 0 ? "flex" : "none";
}

function openCart() {
  if (cart.length === 0) { showToast("🛒 السلة فارغة!"); return; }
  renderCart();
  document.getElementById("cartView").style.display = "block";
  document.getElementById("orderForm").classList.remove("show");
  document.getElementById("successScreen").classList.remove("show");
  showModal("cartModal");
}

function renderCart() {
  const wrap = document.getElementById("cartItems");
  wrap.innerHTML = "";
  let total = 0;
  cart.forEach(item => {
    total += item.price * item.qty;
    const div = document.createElement("div");
    div.className = "cart-item";
    div.innerHTML = `
      <div class="cart-item-emoji">${item.emoji}</div>
      <div class="cart-item-info">
        <div class="cart-item-name">${item.name} × ${item.qty}</div>
        <div class="cart-item-price">${item.price * item.qty} ${STORE.currency}</div>
      </div>
      <button class="cart-item-remove" onclick="removeFromCart(${item.id})">✕</button>`;
    wrap.appendChild(div);
  });
  document.getElementById("cartTotal").textContent = total + " " + STORE.currency;
}

function removeFromCart(id) {
  cart = cart.filter(i => i.id !== id);
  updateCartCount();
  if (cart.length === 0) { closeAll(); return; }
  renderCart();
}

// ===== ORDER =====
function goToOrder() {
  document.getElementById("cartView").style.display = "none";
  document.getElementById("orderForm").classList.add("show");
}

function submitOrder() {
  const name = document.getElementById("fName").value.trim();
  const phone = document.getElementById("fPhone").value.trim();
  const city = document.getElementById("fCity").value.trim();
  const address = document.getElementById("fAddress").value.trim();

  if (!name || !phone || !city || !address) {
    showToast("⚠️ يرجى ملء جميع الحقول");
    return;
  }

  // إرسال للبوت عبر تيليغرام
  const orderText = cart.map(i => `• ${i.name} ×${i.qty} = ${i.price * i.qty} ${STORE.currency}`).join("\n");
  const total = cart.reduce((s, i) => s + i.price * i.qty, 0);
  const msg = `طلب جديد 🛒\n\nاسم: ${name}\nهاتف: ${phone}\nمدينة: ${city}\nعنوان: ${address}\n\nالمنتجات:\n${orderText}\n\nالإجمالي: ${total} ${STORE.currency}`;

  if (tg) tg.sendData(msg);

  cart = [];
  updateCartCount();
  document.getElementById("orderForm").classList.remove("show");
  document.getElementById("successScreen").classList.add("show");
}

// ===== UTILS =====
function showModal(id) {
  document.getElementById("overlay").classList.add("show");
  document.getElementById(id).classList.add("show");
}

function closeAll() {
  document.getElementById("overlay").classList.remove("show");
  document.getElementById("productModal").classList.remove("show");
  document.getElementById("cartModal").classList.remove("show");
}

function showToast(msg) {
  const t = document.getElementById("toast");
  t.textContent = msg;
  t.classList.add("show");
  setTimeout(() => t.classList.remove("show"), 2500);
}
</script>
</body>
</html>
