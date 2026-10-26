[Uploading style.css…]()

/* ========== 全局样式 ========== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'PingFang SC', 'Hiragino Sans GB',
        'Microsoft YaHei', 'Helvetica Neue', Helvetica, Arial, sans-serif;
    background-color: #f5f5f5;
    color: #333;
    line-height: 1.6;
}

a {
    text-decoration: none;
    color: inherit;
}

ul {
    list-style: none;
}

img {
    max-width: 100%;
    display: block;
}

button {
    cursor: pointer;
    border: none;
    outline: none;
    font-family: inherit;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* ========== 顶部导航 ========== */
.header {
    background: #fff;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.06);
    position: sticky;
    top: 0;
    z-index: 100;
}

.header-top {
    background: #f8f8f8;
    border-bottom: 1px solid #eee;
    font-size: 12px;
    color: #999;
    padding: 8px 0;
}

.header-top .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header-top-right a {
    margin-left: 20px;
    transition: color 0.2s;
}

.header-top-right a:hover {
    color: #ff6b6b;
}

.header-main {
    padding: 20px 0;
}

.header-main .container {
    display: flex;
    align-items: center;
    gap: 40px;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;
    font-size: 24px;
    font-weight: bold;
    color: #ff6b6b;
}

.logo i {
    font-size: 32px;
}

.search-box {
    flex: 1;
    display: flex;
    max-width: 500px;
    border: 2px solid #ff6b6b;
    border-radius: 24px;
    overflow: hidden;
}

.search-box input {
    flex: 1;
    padding: 10px 20px;
    border: none;
    outline: none;
    font-size: 14px;
}

.search-box button {
    background: #ff6b6b;
    color: #fff;
    padding: 0 24px;
    font-size: 16px;
    transition: background 0.2s;
}

.search-box button:hover {
    background: #ff5252;
}

.cart-btn {
    display: flex;
    align-items: center;
    gap: 8px;
    padding: 10px 20px;
    background: #fff5f5;
    border: 1px solid #ffd6d6;
    border-radius: 24px;
    color: #ff6b6b;
    font-weight: 500;
    transition: all 0.2s;
    position: relative;
}

.cart-btn:hover {
    background: #ff6b6b;
    color: #fff;
}

.cart-badge {
    position: absolute;
    top: -8px;
    right: -8px;
    background: #ff4757;
    color: #fff;
    font-size: 12px;
    min-width: 20px;
    height: 20px;
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0 6px;
}

.nav-bar {
    background: #fff;
    border-top: 1px solid #f0f0f0;
}

.nav-list {
    display: flex;
    gap: 0;
}

.nav-list li a {
    display: block;
    padding: 14px 24px;
    font-size: 15px;
    color: #333;
    transition: all 0.2s;
    border-bottom: 2px solid transparent;
}

.nav-list li a:hover,
.nav-list li a.active {
    color: #ff6b6b;
    border-bottom-color: #ff6b6b;
}

/* ========== 主内容区 ========== */
.main-content {
    min-height: calc(100vh - 300px);
    padding: 20px 0 40px;
}

/* ========== 轮播图 ========== */
.banner-slider {
    position: relative;
    border-radius: 12px;
    overflow: hidden;
    margin-bottom: 24px;
    height: 320px;
}

.banner-item {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 60px;
    color: #fff;
}

.banner-content h2 {
    font-size: 42px;
    margin-bottom: 12px;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
}

.banner-content p {
    font-size: 18px;
    margin-bottom: 24px;
    opacity: 0.9;
}

.banner-item img {
    height: 280px;
    width: auto;
    border-radius: 12px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
}

.banner-dots {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    gap: 10px;
}

.dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.5);
    cursor: pointer;
    transition: all 0.2s;
}

.dot.active {
    background: #fff;
    width: 30px;
    border-radius: 5px;
}

/* ========== 快捷入口 ========== */
.quick-entry {
    display: grid;
    grid-template-columns: repeat(8, 1fr);
    gap: 16px;
    background: #fff;
    padding: 24px;
    border-radius: 12px;
    margin-bottom: 24px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.entry-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 8px;
    padding: 12px;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.2s;
}

.entry-item:hover {
    background: #f8f8f8;
    transform: translateY(-2px);
}

.entry-item i {
    font-size: 28px;
}

.entry-item span {
    font-size: 13px;
    color: #666;
}

/* ========== 商品列表 ========== */
.product-section {
    background: #fff;
    border-radius: 12px;
    padding: 24px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.section-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
    padding-bottom: 16px;
    border-bottom: 1px solid #f0f0f0;
}

.section-title h2 {
    font-size: 20px;
    color: #333;
}

.section-title h2 small {
    font-size: 14px;
    color: #999;
    font-weight: normal;
    margin-left: 10px;
}

.filter-bar {
    display: flex;
    align-items: center;
    gap: 16px;
    font-size: 14px;
}

.filter-bar span {
    color: #999;
}

.filter-bar a {
    color: #666;
    padding: 4px 12px;
    border-radius: 4px;
    transition: all 0.2s;
}

.filter-bar a:hover,
.filter-bar a.active {
    color: #ff6b6b;
    background: #fff0f0;
}

.product-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 20px;
}

.product-card {
    background: #fff;
    border: 1px solid #f0f0f0;
    border-radius: 8px;
    overflow: hidden;
    transition: all 0.3s;
    cursor: pointer;
}

.product-card:hover {
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
    transform: translateY(-4px);
    border-color: transparent;
}

.product-image {
    position: relative;
    overflow: hidden;
    aspect-ratio: 1;
    background: #f8f8f8;
}

.product-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s;
}

.product-card:hover .product-image img {
    transform: scale(1.05);
}

.discount-tag {
    position: absolute;
    top: 10px;
    left: 10px;
    background: linear-gradient(135deg, #ff6b6b, #ff8e8e);
    color: #fff;
    padding: 4px 10px;
    font-size: 12px;
    font-weight: bold;
    border-radius: 4px;
    z-index: 2;
}

.quick-add {
    position: absolute;
    bottom: -50px;
    left: 0;
    right: 0;
    background: rgba(255, 107, 107, 0.95);
    color: #fff;
    padding: 12px;
    font-size: 14px;
    transition: bottom 0.3s;
}

.product-card:hover .quick-add {
    bottom: 0;
}

.quick-add:hover {
    background: #ff5252;
}

.product-info {
    padding: 12px;
}

.product-name {
    font-size: 14px;
    font-weight: normal;
    line-height: 1.4;
    height: 40px;
    overflow: hidden;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    margin-bottom: 8px;
}

.product-name a {
    color: #333;
    transition: color 0.2s;
}

.product-name a:hover {
    color: #ff6b6b;
}

.product-rating {
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 12px;
    margin-bottom: 8px;
    color: #999;
}

.stars i {
    color: #ddd;
    font-size: 12px;
}

.stars i.filled {
    color: #ffb800;
}

.rating-text {
    color: #ff6b6b;
    font-weight: 500;
}

.product-price {
    display: flex;
    align-items: baseline;
    gap: 8px;
}

.current-price {
    font-size: 20px;
    font-weight: bold;
    color: #ff6b6b;
}

.original-price {
    font-size: 13px;
    color: #999;
    text-decoration: line-through;
}

/* ========== 空状态 ========== */
.empty-state,
.empty-cart {
    text-align: center;
    padding: 80px 20px;
    color: #999;
}

.empty-state i,
.empty-cart i {
    font-size: 80px;
    margin-bottom: 20px;
    color: #ddd;
}

.empty-state h3,
.empty-cart h2 {
    font-size: 20px;
    margin-bottom: 12px;
    color: #666;
}

.empty-state p,
.empty-cart p {
    margin-bottom: 24px;
}

/* ========== 按钮 ========== */
.btn-primary {
    display: inline-block;
    padding: 12px 32px;
    background: linear-gradient(135deg, #ff6b6b, #ff8e8e);
    color: #fff;
    border-radius: 24px;
    font-size: 15px;
    font-weight: 500;
    transition: all 0.2s;
    border: none;
    cursor: pointer;
}

.btn-primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.4);
}

.btn-outline {
    display: inline-block;
    padding: 12px 32px;
    background: #fff;
    color: #ff6b6b;
    border: 1px solid #ff6b6b;
    border-radius: 24px;
    font-size: 15px;
    font-weight: 500;
    transition: all 0.2s;
}

.btn-outline:hover {
    background: #fff0f0;
}

/* ========== 面包屑 ========== */
.breadcrumb {
    padding: 16px 0;
    font-size: 14px;
    color: #999;
}

.breadcrumb a {
    color: #666;
    transition: color 0.2s;
}

.breadcrumb a:hover {
    color: #ff6b6b;
}

.breadcrumb .current {
    color: #333;
}

/* ========== 商品详情页 ========== */
.product-detail {
    display: grid;
    grid-template-columns: 480px 1fr;
    gap: 40px;
    background: #fff;
    padding: 30px;
    border-radius: 12px;
    margin-bottom: 24px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.product-gallery .main-image {
    width: 100%;
    aspect-ratio: 1;
    border-radius: 8px;
    overflow: hidden;
    background: #f8f8f8;
    margin-bottom: 12px;
}

.product-gallery .main-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.thumb-list {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

.thumb {
    aspect-ratio: 1;
    border: 2px solid transparent;
    border-radius: 6px;
    overflow: hidden;
    cursor: pointer;
    transition: all 0.2s;
}

.thumb:hover,
.thumb.active {
    border-color: #ff6b6b;
}

.thumb img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.product-info-detail .product-title {
    font-size: 22px;
    font-weight: 500;
    line-height: 1.5;
    margin-bottom: 12px;
}

.product-summary {
    display: flex;
    align-items: center;
    gap: 16px;
    margin-bottom: 20px;
    padding-bottom: 20px;
    border-bottom: 1px solid #f0f0f0;
}

.tag {
    padding: 2px 8px;
    font-size: 12px;
    border-radius: 4px;
    font-weight: 500;
}

.tag.hot {
    background: #fff0f0;
    color: #ff6b6b;
}

.rating i {
    color: #ffb800;
    font-size: 14px;
}

.sales-count {
    color: #999;
    font-size: 14px;
}

.price-block {
    background: linear-gradient(135deg, #fff5f5, #fff0f0);
    padding: 20px;
    border-radius: 8px;
    margin-bottom: 20px;
}

.price-row {
    display: flex;
    align-items: baseline;
    gap: 12px;
}

.price-row .label {
    color: #999;
    font-size: 14px;
}

.price-current {
    font-size: 32px;
    font-weight: bold;
    color: #ff6b6b;
}

.price-original {
    font-size: 16px;
    color: #999;
    text-decoration: line-through;
}

.discount {
    background: #ff6b6b;
    color: #fff;
    padding: 4px 10px;
    font-size: 12px;
    border-radius: 4px;
}

.delivery-info {
    display: flex;
    gap: 30px;
    margin-bottom: 20px;
    font-size: 14px;
    color: #666;
}

.info-item i {
    color: #52c41a;
    margin-right: 6px;
}

.stock-info {
    font-size: 14px;
    color: #666;
    margin-bottom: 20px;
}

.stock-info strong {
    color: #ff6b6b;
}

.quantity-selector {
    display: flex;
    align-items: center;
    gap: 20px;
    margin-bottom: 24px;
}

.quantity-selector .label {
    color: #666;
    font-size: 14px;
}

.quantity-control {
    display: flex;
    align-items: center;
    border: 1px solid #ddd;
    border-radius: 4px;
    overflow: hidden;
}

.qty-btn {
    width: 32px;
    height: 32px;
    background: #f8f8f8;
    color: #666;
    font-size: 16px;
    transition: background 0.2s;
}

.qty-btn:hover {
    background: #eee;
}

.qty-input {
    width: 50px;
    height: 32px;
    border: none;
    text-align: center;
    font-size: 14px;
    outline: none;
    border-left: 1px solid #ddd;
    border-right: 1px solid #ddd;
}

.action-buttons {
    display: flex;
    gap: 16px;
    margin-bottom: 24px;
}

.btn-add-cart {
    flex: 1;
    padding: 14px;
    background: #fff0f0;
    color: #ff6b6b;
    border: 1px solid #ff6b6b;
    border-radius: 4px;
    font-size: 16px;
    font-weight: 500;
    transition: all 0.2s;
}

.btn-add-cart:hover {
    background: #ffe0e0;
}

.btn-buy-now {
    flex: 1;
    padding: 14px;
    background: linear-gradient(135deg, #ff6b6b, #ff8e8e);
    color: #fff;
    border-radius: 4px;
    font-size: 16px;
    font-weight: 500;
    transition: all 0.2s;
}

.btn-buy-now:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.4);
}

.service-info {
    display: flex;
    gap: 24px;
    font-size: 13px;
    color: #666;
    padding-top: 20px;
    border-top: 1px solid #f0f0f0;
}

.service-info i {
    color: #52c41a;
    margin-right: 4px;
}

/* ========== 商品详情描述 ========== */
.product-description {
    background: #fff;
    border-radius: 12px;
    margin-bottom: 24px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
    overflow: hidden;
}

.desc-tabs {
    display: flex;
    border-bottom: 1px solid #f0f0f0;
}

.tab-btn {
    padding: 16px 32px;
    background: none;
    font-size: 15px;
    color: #666;
    border-bottom: 2px solid transparent;
    transition: all 0.2s;
}

.tab-btn:hover,
.tab-btn.active {
    color: #ff6b6b;
    border-bottom-color: #ff6b6b;
}

.desc-content {
    padding: 30px;
    line-height: 1.8;
}

.desc-content h3 {
    font-size: 18px;
    margin-bottom: 12px;
    color: #333;
}

.desc-content p {
    margin-bottom: 16px;
    color: #666;
}

.desc-content ul {
    margin-bottom: 20px;
}

.desc-content li {
    padding: 6px 0;
    color: #666;
}

/* ========== 相关推荐 ========== */
.related-products {
    background: #fff;
    border-radius: 12px;
    padding: 24px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.related-products .section-title {
    font-size: 20px;
    margin-bottom: 20px;
    padding-bottom: 16px;
    border-bottom: 1px solid #f0f0f0;
}

/* ========== 购物车页面 ========== */
.cart-page {
    padding: 20px 0;
}

.page-title {
    font-size: 24px;
    margin-bottom: 24px;
    color: #333;
}

.page-title small {
    font-size: 14px;
    color: #999;
    font-weight: normal;
}

.cart-layout {
    display: grid;
    grid-template-columns: 1fr 300px;
    gap: 24px;
}

.cart-list {
    background: #fff;
    border-radius: 12px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
    overflow: hidden;
}

.cart-header {
    display: grid;
    grid-template-columns: 50px 2fr 1fr 120px 1fr 80px;
    padding: 16px 20px;
    background: #fafafa;
    border-bottom: 1px solid #f0f0f0;
    font-size: 14px;
    color: #666;
    align-items: center;
}

.cart-item {
    display: grid;
    grid-template-columns: 50px 2fr 1fr 120px 1fr 80px;
    padding: 20px;
    border-bottom: 1px solid #f0f0f0;
    align-items: center;
    transition: background 0.2s;
}

.cart-item:hover {
    background: #fafafa;
}

.cart-item:last-child {
    border-bottom: none;
}

.col-info {
    display: flex;
    gap: 16px;
    align-items: center;
}

.col-info img {
    width: 80px;
    height: 80px;
    object-fit: cover;
    border-radius: 6px;
}

.item-name {
    font-size: 14px;
    color: #333;
    line-height: 1.4;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    overflow: hidden;
}

.col-price .price {
    color: #ff6b6b;
    font-weight: 500;
    font-size: 16px;
}

.col-price .original {
    display: block;
    color: #999;
    font-size: 13px;
    text-decoration: line-through;
    margin-top: 4px;
}

.col-total .subtotal {
    color: #ff6b6b;
    font-size: 18px;
    font-weight: bold;
}

.remove-btn {
    background: none;
    color: #999;
    font-size: 13px;
    transition: color 0.2s;
}

.remove-btn:hover {
    color: #ff6b6b;
}

/* ========== 订单结算侧边栏 ========== */
.cart-sidebar,
.checkout-sidebar {
    position: sticky;
    top: 160px;
    align-self: start;
}

.order-summary {
    background: #fff;
    border-radius: 12px;
    padding: 24px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.order-summary h3 {
    font-size: 18px;
    margin-bottom: 20px;
    padding-bottom: 16px;
    border-bottom: 1px solid #f0f0f0;
}

.summary-row {
    display: flex;
    justify-content: space-between;
    margin-bottom: 12px;
    font-size: 14px;
    color: #666;
}

.summary-row.discount {
    color: #ff6b6b;
}

.summary-row.shipping {
    padding-bottom: 16px;
    border-bottom: 1px solid #f0f0f0;
    margin-bottom: 16px;
}

.summary-total {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 20px;
}

.summary-total span:first-child {
    font-size: 14px;
    color: #666;
}

.total-price {
    font-size: 28px;
    font-weight: bold;
    color: #ff6b6b;
}

.btn-checkout {
    display: block;
    width: 100%;
    padding: 14px;
    background: linear-gradient(135deg, #ff6b6b, #ff8e8e);
    color: #fff;
    border-radius: 4px;
    text-align: center;
    font-size: 16px;
    font-weight: 500;
    margin-bottom: 12px;
    transition: all 0.2s;
}

.btn-checkout:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.4);
}

.btn-continue {
    display: block;
    text-align: center;
    color: #666;
    font-size: 14px;
    transition: color 0.2s;
}

.btn-continue:hover {
    color: #ff6b6b;
}

/* ========== 结算页 ========== */
.checkout-layout {
    display: grid;
    grid-template-columns: 1fr 320px;
    gap: 24px;
}

.checkout-section {
    background: #fff;
    border-radius: 12px;
    padding: 24px;
    margin-bottom: 16px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.checkout-section h3 {
    font-size: 16px;
    margin-bottom: 16px;
    color: #333;
}

.checkout-section h3 i {
    color: #ff6b6b;
    margin-right: 8px;
}

.address-card {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 16px;
    background: #fafafa;
    border-radius: 8px;
    border: 1px solid #f0f0f0;
}

.address-info .name {
    font-weight: 500;
    margin-right: 16px;
}

.address-info .phone {
    color: #666;
}

.address-detail {
    margin-top: 8px;
    color: #666;
    font-size: 14px;
}

.default-tag {
    padding: 4px 10px;
    background: #ff6b6b;
    color: #fff;
    font-size: 12px;
    border-radius: 4px;
}

.payment-methods {
    display: flex;
    gap: 16px;
}

.payment-option {
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    padding: 16px;
    border: 2px solid #f0f0f0;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.2s;
}

.payment-option:hover {
    border-color: #ffd6d6;
}

.payment-option.active {
    border-color: #ff6b6b;
    background: #fff5f5;
}

.payment-option input {
    display: none;
}

.payment-option i {
    font-size: 20px;
}

.order-items {
    max-height: 300px;
    overflow-y: auto;
}

.order-item {
    display: flex;
    align-items: center;
    gap: 16px;
    padding: 12px 0;
    border-bottom: 1px solid #f0f0f0;
}

.order-item:last-child {
    border-bottom: none;
}

.order-item img {
    width: 60px;
    height: 60px;
    object-fit: cover;
    border-radius: 6px;
}

.order-item .item-info {
    flex: 1;
}

.order-item .item-info h4 {
    font-size: 14px;
    font-weight: normal;
    margin-bottom: 4px;
}

.order-item .item-price {
    font-size: 13px;
    color: #ff6b6b;
}

.item-quantity {
    color: #999;
    font-size: 14px;
}

.item-subtotal {
    color: #ff6b6b;
    font-weight: 500;
}

.btn-submit-order {
    display: block;
    width: 100%;
    padding: 14px;
    background: linear-gradient(135deg, #ff6b6b, #ff8e8e);
    color: #fff;
    border-radius: 4px;
    text-align: center;
    font-size: 16px;
    font-weight: 500;
    transition: all 0.2s;
}

.btn-submit-order:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.4);
}

/* ========== 下单成功页 ========== */
.order-success-page {
    padding: 60px 0;
    display: flex;
    justify-content: center;
}

.success-box {
    background: #fff;
    padding: 60px 80px;
    border-radius: 12px;
    text-align: center;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
}

.success-icon {
    width: 80px;
    height: 80px;
    margin: 0 auto 24px;
    background: #f6ffed;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.success-icon i {
    font-size: 48px;
    color: #52c41a;
}

.success-box h1 {
    font-size: 28px;
    margin-bottom: 12px;
    color: #333;
}

.success-box > p {
    color: #666;
    margin-bottom: 24px;
}

.order-info {
    background: #fafafa;
    padding: 20px;
    border-radius: 8px;
    margin-bottom: 24px;
    text-align: left;
}

.order-info p {
    padding: 4px 0;
    color: #666;
    font-size: 14px;
}

.order-info strong {
    color: #333;
}

.success-actions {
    display: flex;
    gap: 16px;
    justify-content: center;
}

/* ========== 404 页面 ========== */
.error-page {
    text-align: center;
    padding: 100px 20px;
}

.error-page h1 {
    font-size: 120px;
    color: #ff6b6b;
    margin-bottom: 20px;
}

.error-page h2 {
    font-size: 24px;
    margin-bottom: 12px;
    color: #333;
}

.error-page p {
    color: #999;
    margin-bottom: 30px;
}

/* ========== 页脚 ========== */
.footer {
    background: #2c2c2c;
    color: #999;
    padding: 40px 0 0;
    margin-top: 40px;
}

.footer-content {
    display: grid;
    grid-template-columns: 2fr 1fr 1fr 1fr 1.5fr;
    gap: 40px;
    padding-bottom: 30px;
}

.footer-section h3 {
    color: #fff;
    font-size: 18px;
    margin-bottom: 16px;
}

.footer-section h3 i {
    color: #ff6b6b;
    margin-right: 8px;
}

.footer-section h4 {
    color: #fff;
    font-size: 15px;
    margin-bottom: 16px;
}

.footer-section p {
    margin-bottom: 8px;
    font-size: 13px;
    line-height: 1.8;
}

.footer-section ul li {
    padding: 6px 0;
}

.footer-section ul li a {
    font-size: 13px;
    transition: color 0.2s;
}

.footer-section ul li a:hover {
    color: #ff6b6b;
}

.footer-section i {
    margin-right: 6px;
    color: #ff6b6b;
}

.footer-bottom {
    text-align: center;
    padding: 20px 0;
    border-top: 1px solid #3a3a3a;
    font-size: 12px;
}

/* ========== Toast 提示 ========== */
.toast {
    position: fixed;
    top: 100px;
    left: 50%;
    transform: translateX(-50%) translateY(-20px);
    padding: 12px 24px;
    background: rgba(0, 0, 0, 0.8);
    color: #fff;
    border-radius: 8px;
    font-size: 14px;
    opacity: 0;
    visibility: hidden;
    transition: all 0.3s;
    z-index: 1000;
}

.toast.show {
    opacity: 1;
    visibility: visible;
    transform: translateX(-50%) translateY(0);
}

.toast.success {
    background: rgba(82, 196, 26, 0.9);
}

.toast.error {
    background: rgba(255, 71, 87, 0.9);
}

/* ========== 响应式 ========== */
@media (max-width: 1024px) {
    .product-grid {
        grid-template-columns: repeat(3, 1fr);
    }

    .quick-entry {
        grid-template-columns: repeat(4, 1fr);
    }

    .product-detail {
        grid-template-columns: 1fr;
    }

    .cart-layout,
    .checkout-layout {
        grid-template-columns: 1fr;
    }

    .footer-content {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 768px) {
    .header-main .container {
        flex-wrap: wrap;
        gap: 16px;
    }

    .search-box {
        order: 3;
        flex-basis: 100%;
    }

    .product-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .quick-entry {
        grid-template-columns: repeat(4, 1fr);
    }

    .banner-item {
        padding: 0 30px;
    }

    .banner-content h2 {
        font-size: 28px;
    }

    .banner-item img {
        display: none;
    }

    .nav-list {
        overflow-x: auto;
        flex-wrap: nowrap;
    }

    .nav-list li a {
        white-space: nowrap;
        padding: 12px 16px;
    }

    .cart-header {
        display: none;
    }

    .cart-item {
        grid-template-columns: 1fr;
        gap: 12px;
        text-align: center;
    }

    .col-info {
        justify-content: center;
    }

    .footer-content {
        grid-template-columns: 1fr;
        text-align: center;
    }
}
