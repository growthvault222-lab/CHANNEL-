<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">  
    <title>Registry Vault — Digital Asset Hub</title>  
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>  
    <link rel="preconnect" href="https://fonts.googleapis.com">  
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>  
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;900&family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">  
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">  
    <style>  
        :root { --gold-primary: #C5A059; --gold-dark: #8C7343; --gold-light: #E5C387; --bg-charcoal: #12100E; --bg-absolute: #070605; --glass-bg: rgba(18, 16, 14, 0.75); --glass-border: rgba(197, 160, 89, 0.15); }  
        body { font-family: 'Inter', sans-serif; background-color: var(--bg-absolute); color: #F1F5F9; overflow: hidden; -webkit-tap-highlight-color: transparent; user-select: none; }  
        .luxury-title { font-family: 'Cinzel', serif; letter-spacing: 0.22em; text-shadow: 0 0 12px rgba(197, 160, 89, 0.2); }  
        .deco-card { position: relative; background: var(--glass-bg); border: 1px solid var(--glass-border); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1); }  
        .deco-card::before, .deco-card::after { content: ""; position: absolute; width: 8px; height: 8px; border: 1px solid var(--gold-primary); z-index: 10; pointer-events: none; }  
        .deco-card::before { top: 3px; left: 3px; border-right: none; border-bottom: none; }  
        .deco-card::after { bottom: 3px; right: 3px; border-left: none; border-top: none; }  
        .no-scrollbar::-webkit-scrollbar { display: none; }  
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }  
        .nav-link.active i { color: var(--gold-primary); text-shadow: 0 0 15px rgba(197, 160, 89, 0.6); transform: translateY(-2px); }  
        .nav-link.active span { color: white; font-weight: 600; }  
        .nav-link::after { content: ''; position: absolute; bottom: 4px; width: 0; height: 2px; background: var(--gold-primary); transition: width 0.25s cubic-bezier(0.16, 1, 0.3, 1); }  
        .nav-link.active::after { width: 16px; }  
        .app-container { width: 100%; max-width: 480px; height: 100vh; background: var(--bg-absolute); position: relative; overflow: hidden; display: flex; flex-direction: column; }  
    </style>  
</head>  
<body class="flex items-center justify-center min-h-screen bg-[#020202]">  
    <div class="app-container border-x border-white/[0.03] shadow-2xl flex flex-col justify-between">  
        <div class="w-full bg-gradient-to-r from-[#8C7343] to-[#C5A059] text-black text-[9px] uppercase tracking-[0.15em] font-bold py-1.5 px-4 text-center shrink-0 flex items-center justify-center gap-1.5 z-50">  
            <i class="fa-solid fa-bolt-lightning animate-pulse"></i>   
            <span>Flash Sale Live: Use code <span class="underline">GOLD25</span> for 25% Off</span>  
        </div>  
        <header class="w-full pt-4 px-4 pb-3 bg-black/90 backdrop-blur-md border-b border-white/[0.04] shrink-0 z-40">  
            <div class="flex items-center justify-between mb-3">  
                <div class="flex flex-col">  
                    <span class="text-[8px] tracking-[0.3em] uppercase text-gray-500 font-bold">The Luxury Registry</span>  
                    <h1 class="text-[#C5A059] text-sm font-black uppercase luxury-title mt-0.5 cursor-pointer" onclick="window.location.href='index.html'">Digital Asset Hub</h1>  
                </div>  
                <div class="flex items-center gap-2">  
                    <button onclick="window.location.href='notifications.html'" class="w-8 h-8 rounded-full border border-white/10 bg-white/5 flex items-center justify-center text-gray-400 relative">  
                        <i class="fa-solid fa-bell text-xs"></i>  
                        <span id="globalNotificationIndicator" class="absolute top-1.5 right-1.5 w-1.5 h-1.5 bg-amber-400 rounded-full hidden"></span>  
                    </button>  
                </div>  
            </div>  
        </header>  
        <main class="flex-1 overflow-y-auto px-4 pb-24 pt-2 no-scrollbar space-y-5">  
            <div id="view-wishlist" class="application-viewport space-y-4">  
                <div class="border-b border-[#C5A059]/20 pb-2">  
                    <h2 class="text-xs uppercase tracking-widest font-bold text-[#C5A059]">Curated Wishlist Registry</h2>  
                </div>  
                <div id="wishlistItemsInject" class="space-y-3"></div>  
            </div>  
        </main>  
        <nav class="w-full bg-black/95 backdrop-blur-md border-t border-white/[0.04] py-2 px-6 flex items-center justify-between absolute bottom-0 left-0 right-0 z-40 shrink-0">  
            <button onclick="window.location.href='index.html'" id="navBtn-browse" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-gem text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Catalog</span>  
            </button>  
            <button onclick="window.location.href='wishlist.html'" id="navBtn-wishlist" class="nav-link active relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-heart text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Registry</span>  
            </button>  
            <button onclick="window.location.href='cart.html'" id="navBtn-cart" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <div class="relative">  
                    <i class="fa-solid fa-vault text-xs"></i>  
                    <span id="navCartCountIndicator" class="absolute -top-1.5 -right-2 bg-[#C5A059] text-black text-[7px] font-black h-3.5 w-3.5 flex items-center justify-center rounded-full border border-black hidden">0</span>  
                </div>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Cart</span>  
            </button>  
            <button onclick="window.location.href='dashboard.html'" id="navBtn-dashboard" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-chart-line text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Console</span>  
            </button>  
        </nav>  
    </div>  
    <script>  
        const memoryStore = window.localStorage;  
        let state = {  
            products: JSON.parse(memoryStore.getItem("dh_products")) || [],  
            cart: JSON.parse(memoryStore.getItem("dh_cart")) || [],  
            wishlist: JSON.parse(memoryStore.getItem("dh_wishlist")) || [],  
            notifications: JSON.parse(memoryStore.getItem("dh_notifications")) || []  
        };  
        function saveStateToStorage() {  
            memoryStore.setItem("dh_cart", JSON.stringify(state.cart));  
            memoryStore.setItem("dh_wishlist", JSON.stringify(state.wishlist));  
            memoryStore.setItem("dh_notifications", JSON.stringify(state.notifications));  
        }  
        const SystemUINavigation = {  
            renderWishlist() {  
                const target = document.getElementById("wishlistItemsInject");  
                const items = state.products.filter(p => state.wishlist.includes(p.id));  
                if(items.length === 0) {  
                    target.innerHTML = `<div class="text-center py-12 text-gray-600 text-[10px] font-mono uppercase tracking-widest">Wishlist Vault Empty</div>`;  
                    return;  
                }  
                target.innerHTML = items.map(p => `  
                    <div class="deco-card p-3 rounded-xl flex items-center gap-3">  
                        <img src="${p.image}" class="w-10 h-10 object-cover rounded-md bg-white/5">  
                        <div class="flex-1 min-w-0">  
                            <h4 class="text-xs font-bold text-white tracking-wide truncate uppercase">${p.title}</h4>  
                            <span class="font-mono text-[#C5A059] text-[10px]">$${p.price.toFixed(2)}</span>  
                        </div>  
                        <div class="flex items-center gap-2">  
                            <button onclick="SystemCartSuite.moveWishlistToCart('${p.id}')" class="text-[9px] font-bold bg-[#C5A059] text-black px-2 py-1 rounded uppercase tracking-wider">Move</button>  
                            <button onclick="SystemCartSuite.toggleWishlist('${p.id}')" class="text-gray-500 hover:text-red-400 px-1"><i class="fa-solid fa-trash-can text-xs"></i></button>  
                        </div>  
                    </div>  
                `).join("");  
            }  
        };  
        const SystemCartSuite = {  
            toggleWishlist(id) {  
                const index = state.wishlist.indexOf(id);  
                if (index > -1) state.wishlist.splice(index, 1);  
                saveStateToStorage();  
                SystemUINavigation.renderWishlist();  
            },  
            moveWishlistToCart(id) {  
                this.toggleWishlist(id);  
                if (!state.cart.includes(id)) state.cart.push(id);  
                saveStateToStorage();  
                this.updateCounters();  
                SystemUINavigation.renderWishlist();  
            },  
            updateCounters() {  
                const indicator = document.getElementById("navCartCountIndicator");  
                indicator.innerText = state.cart.length;  
                indicator.classList.toggle("hidden", state.cart.length === 0);  
            }  
        };  
        document.addEventListener("DOMContentLoaded", () => {  
            SystemCartSuite.updateCounters();  
            SystemUINavigation.renderWishlist();  
            const hasUnread = state.notifications.some(n => !n.read);  
            document.getElementById("globalNotificationIndicator").classList.toggle("hidden", !hasUnread);  
        });  
    </script>  
</body>  
</html>
<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">  
    <title>Transactional Matrix — Digital Asset Hub</title>  
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>  
    <link rel="preconnect" href="https://fonts.googleapis.com">  
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>  
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;900&family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">  
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">  
    <script src="https://js.paystack.co/v1/inline.js"></script>  
    <style>  
        :root { --gold-primary: #C5A059; --gold-dark: #8C7343; --gold-light: #E5C387; --bg-charcoal: #12100E; --bg-absolute: #070605; --glass-bg: rgba(18, 16, 14, 0.75); --glass-border: rgba(197, 160, 89, 0.15); }  
        body { font-family: 'Inter', sans-serif; background-color: var(--bg-absolute); color: #F1F5F9; overflow: hidden; -webkit-tap-highlight-color: transparent; user-select: none; }  
        .luxury-title { font-family: 'Cinzel', serif; letter-spacing: 0.22em; text-shadow: 0 0 12px rgba(197, 160, 89, 0.2); }  
        .deco-card { position: relative; background: var(--glass-bg); border: 1px solid var(--glass-border); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1); }  
        .deco-card::before, .deco-card::after { content: ""; position: absolute; width: 8px; height: 8px; border: 1px solid var(--gold-primary); z-index: 10; pointer-events: none; }  
        .deco-card::before { top: 3px; left: 3px; border-right: none; border-bottom: none; }  
        .deco-card::after { bottom: 3px; right: 3px; border-left: none; border-top: none; }  
        .no-scrollbar::-webkit-scrollbar { display: none; }  
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }  
        .nav-link.active i { color: var(--gold-primary); text-shadow: 0 0 15px rgba(197, 160, 89, 0.6); transform: translateY(-2px); }  
        .nav-link.active span { color: white; font-weight: 600; }  
        .nav-link::after { content: ''; position: absolute; bottom: 4px; width: 0; height: 2px; background: var(--gold-primary); transition: width 0.25s cubic-bezier(0.16, 1, 0.3, 1); }  
        .nav-link.active::after { width: 16px; }  
        .app-container { width: 100%; max-width: 480px; height: 100vh; background: var(--bg-absolute); position: relative; overflow: hidden; display: flex; flex-direction: column; }  
    </style>  
</head>  
<body class="flex items-center justify-center min-h-screen bg-[#020202]">  
    <div class="app-container border-x border-white/[0.03] shadow-2xl flex flex-col justify-between">  
        <div class="w-full bg-gradient-to-r from-[#8C7343] to-[#C5A059] text-black text-[9px] uppercase tracking-[0.15em] font-bold py-1.5 px-4 text-center shrink-0 flex items-center justify-center gap-1.5 z-50">  
            <i class="fa-solid fa-bolt-lightning animate-pulse"></i>   
            <span>Flash Sale Live: Use code <span class="underline">GOLD25</span> for 25% Off</span>  
        </div>  
        <header class="w-full pt-4 px-4 pb-3 bg-black/90 backdrop-blur-md border-b border-white/[0.04] shrink-0 z-40">  
            <div class="flex items-center justify-between mb-3">  
                <div class="flex flex-col">  
                    <span class="text-[8px] tracking-[0.3em] uppercase text-gray-500 font-bold">The Luxury Registry</span>  
                    <h1 class="text-[#C5A059] text-sm font-black uppercase luxury-title mt-0.5 cursor-pointer" onclick="window.location.href='index.html'">Digital Asset Hub</h1>  
                </div>  
                <div class="flex items-center gap-2">  
                    <button onclick="window.location.href='notifications.html'" class="w-8 h-8 rounded-full border border-white/10 bg-white/5 flex items-center justify-center text-gray-400 relative">  
                        <i class="fa-solid fa-bell text-xs"></i>  
                        <span id="globalNotificationIndicator" class="absolute top-1.5 right-1.5 w-1.5 h-1.5 bg-amber-400 rounded-full hidden"></span>  
                    </button>  
                </div>  
            </div>  
        </header>  
        <main class="flex-1 overflow-y-auto px-4 pb-24 pt-2 no-scrollbar space-y-5">  
            <div id="view-cart" class="application-viewport space-y-4">  
                <div class="border-b border-[#C5A059]/20 pb-2">  
                    <h2 class="text-xs uppercase tracking-widest font-bold text-[#C5A059]">Secure Cart Matrix</h2>  
                </div>  
                <div id="cartItemsInject" class="space-y-3"></div>  
                  
                <div id="cartLedgerSummaryBlock" class="bg-[#12100E] border border-[#C5A059]/20 rounded-xl p-4 space-y-3 hidden">  
                    <div class="space-y-2">  
                        <div class="flex justify-between items-center text-[11px] text-gray-400">  
                            <span>Subtotal Value</span>  
                            <span class="font-mono text-white" id="ledgerSubtotal">$0.00</span>  
                        </div>  
                        <div class="flex justify-between items-center text-[11px]">  
                            <span class="text-[#C5A059]">Dynamic Promotion Discount</span>  
                            <span class="font-mono text-emerald-400" id="ledgerDiscount">-$0.00</span>  
                        </div>  
                        <div class="flex items-center gap-2 pt-1">  
                            <input type="text" id="couponCodeFormInput" placeholder="Promo code (e.g., GOLD25)" class="flex-1 bg-black border border-white/10 rounded px-2.5 py-1.5 text-[10px] uppercase font-mono tracking-wider text-white focus:outline-none focus:border-[#C5A059]">  
                            <button onclick="SystemCartSuite.applyPromoCouponCode()" class="bg-white/5 border border-white/10 px-3 py-1.5 text-[10px] font-bold text-[#C5A059] uppercase tracking-wider rounded active:bg-[#C5A059]/10">Apply</button>  
                        </div>  
                        <div class="h-px bg-white/[0.05] my-1"></div>  
                        <div class="flex justify-between items-center text-xs font-bold">  
                            <span class="text-gray-300">Total Obligations</span>  
                            <span class="font-mono text-[#C5A059] text-sm" id="ledgerTotal">$0.00</span>  
                        </div>  
                    </div>  
                    <div class="space-y-1 pt-1">  
                        <label class="block text-[9px] uppercase tracking-wider text-gray-500 font-bold">Delivery Email Destination</label>  
                        <input type="email" id="checkoutReceiptEmail" value="collector@luxury.com" placeholder="your.name@luxury.com" class="w-full bg-black border border-white/10 rounded p-2 text-xs text-white focus:outline-none focus:border-[#C5A059]">  
                    </div>  
                    <button onclick="SystemPaymentGateway.initializePaystackSession(event)" class="w-full bg-gradient-to-r from-[#8C7343] to-[#C5A059] text-black font-extrabold text-[11px] uppercase tracking-[0.15em] py-3 rounded-lg mt-2 relative overflow-hidden transition-transform active:scale-[0.98]">  
                        <i class="fa-solid fa-shield-halved mr-1"></i> Authorize Premium Checkout  
                    </button>  
                </div>  
            </div>  
        </main>  
        <nav class="w-full bg-black/95 backdrop-blur-md border-t border-white/[0.04] py-2 px-6 flex items-center justify-between absolute bottom-0 left-0 right-0 z-40 shrink-0">  
            <button onclick="window.location.href='index.html'" id="navBtn-browse" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-gem text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Catalog</span>  
            </button>  
            <button onclick="window.location.href='wishlist.html'" id="navBtn-wishlist" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-heart text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Registry</span>  
            </button>  
            <button onclick="window.location.href='cart.html'" id="navBtn-cart" class="nav-link active relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <div class="relative">  
                    <i class="fa-solid fa-vault text-xs"></i>  
                    <span id="navCartCountIndicator" class="absolute -top-1.5 -right-2 bg-[#C5A059] text-black text-[7px] font-black h-3.5 w-3.5 flex items-center justify-center rounded-full border border-black hidden">0</span>  
                </div>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Cart</span>  
            </button>  
            <button onclick="window.location.href='dashboard.html'" id="navBtn-dashboard" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-chart-line text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Console</span>  
            </button>  
        </nav>  
    </div>  
    <script>  
        const memoryStore = window.localStorage;  
        let state = {  
            products: JSON.parse(memoryStore.getItem("dh_products")) || [],  
            cart: JSON.parse(memoryStore.getItem("dh_cart")) || [],  
            notifications: JSON.parse(memoryStore.getItem("dh_notifications")) || [],  
            promoApplied: memoryStore.getItem("dh_promoApplied") === "true"  
        };  
        function saveStateToStorage() {  
            memoryStore.setItem("dh_cart", JSON.stringify(state.cart));  
            memoryStore.setItem("dh_notifications", JSON.stringify(state.notifications));  
            memoryStore.setItem("dh_promoApplied", state.promoApplied);  
        }  
        const SystemCartSuite = {  
            toggleCart(id) {  
                const index = state.cart.indexOf(id);  
                if (index > -1) state.cart.splice(index, 1);  
                saveStateToStorage();  
                this.updateCounters();  
                this.renderCart();  
            },  
            updateCounters() {  
                const indicator = document.getElementById("navCartCountIndicator");  
                indicator.innerText = state.cart.length;  
                indicator.classList.toggle("hidden", state.cart.length === 0);  
            },  
            renderCart() {  
                const target = document.getElementById("cartItemsInject");  
                const ledger = document.getElementById("cartLedgerSummaryBlock");  
                const items = state.products.filter(p => state.cart.includes(p.id));  
                if(items.length === 0) {  
                    target.innerHTML = `<div class="text-center py-12 text-gray-600 text-[10px] font-mono uppercase tracking-widest">Transactional Matrix Empty</div>`;  
                    ledger.classList.add("hidden");  
                    return;  
                }  
                ledger.classList.remove("hidden");  
                target.innerHTML = items.map(p => `  
                    <div class="deco-card p-3 rounded-xl flex items-center gap-3">  
                        <img src="${p.image}" class="w-10 h-10 object-cover rounded-md bg-white/5">  
                        <div class="flex-1 min-w-0">  
                            <h4 class="text-xs font-bold text-white tracking-wide truncate uppercase">${p.title}</h4>  
                            <span class="font-mono text-[#C5A059] text-[10px]">$${p.price.toFixed(2)}</span>  
                        </div>  
                        <button onclick="SystemCartSuite.toggleCart('${p.id}')" class="text-gray-500 hover:text-red-400 px-2"><i class="fa-solid fa-xmark text-xs"></i></button>  
                    </div>  
                `).join("");  
                this.calculateLedger(items);  
            },  
            applyPromoCouponCode() {  
                const val = document.getElementById("couponCodeFormInput").value.trim().toUpperCase();  
                if(val === "GOLD25") {  
                    state.promoApplied = true;  
                    state.notifications.unshift({ id: Date.now(), text: "Coupon authorization valid: 25% allocation applied.", read: false, time: "Just Now" });  
                } else {  
                    state.notifications.unshift({ id: Date.now(), text: "Invalid deployment credential token code.", read: false, time: "Just Now" });  
                }  
                saveStateToStorage();  
                this.renderCart();  
            },  
            calculateLedger(items) {  
                const subtotal = items.reduce((acc, curr) => acc + curr.price, 0);  
                const discount = state.promoApplied ? (subtotal * 0.25) : 0;  
                const total = subtotal - discount;  
                document.getElementById("ledgerSubtotal").innerText = `$${subtotal.toFixed(2)}`;  
                document.getElementById("ledgerDiscount").innerText = `-$${discount.toFixed(2)}`;  
                document.getElementById("ledgerTotal").innerText = `$${total.toFixed(2)}`;  
            }  
        };  
        const SystemPaymentGateway = {  
            initializePaystackSession(e) {  
                e.preventDefault();  
                const email = document.getElementById("checkoutReceiptEmail").value;  
                if(!email.includes("@")) { alert("Please provide valid asset allocation node target destination email address."); return; }  
                state.notifications.unshift({ id: Date.now(), text: "Contacting transaction gateway authority pipeline...", read: false, time: "Just Now" });  
                saveStateToStorage();  
                setTimeout(() => {  
                    state.cart = [];  
                    state.promoApplied = false;  
                    state.notifications.unshift({ id: Date.now(), text: "Transaction successful! Secure links generated.", read: false, time: "Just Now" });  
                    saveStateToStorage();  
                    window.location.href = "dashboard.html";  
                }, 1500);  
            }  
        };  
        document.addEventListener("DOMContentLoaded", () => {  
            SystemCartSuite.updateCounters();  
            SystemCartSuite.renderCart();  
            const hasUnread = state.notifications.some(n => !n.read);  
            document.getElementById("globalNotificationIndicator").classList.toggle("hidden", !hasUnread);  
        });  
    </script>  
</body>  
</html>
<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">  
    <title>Console Dashboard — Digital Asset Hub</title>  
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>  
    <link rel="preconnect" href="https://fonts.googleapis.com">  
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>  
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;900&family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">  
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">  
    <style>  
        :root { --gold-primary: #C5A059; --gold-dark: #8C7343; --gold-light: #E5C387; --bg-charcoal: #12100E; --bg-absolute: #070605; --glass-bg: rgba(18, 16, 14, 0.75); --glass-border: rgba(197, 160, 89, 0.15); }  
        body { font-family: 'Inter', sans-serif; background-color: var(--bg-absolute); color: #F1F5F9; overflow: hidden; -webkit-tap-highlight-color: transparent; user-select: none; }  
        .luxury-title { font-family: 'Cinzel', serif; letter-spacing: 0.22em; text-shadow: 0 0 12px rgba(197, 160, 89, 0.2); }  
        .deco-card { position: relative; background: var(--glass-bg); border: 1px solid var(--glass-border); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1); }  
        .no-scrollbar::-webkit-scrollbar { display: none; }  
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }  
        .nav-link.active i { color: var(--gold-primary); text-shadow: 0 0 15px rgba(197, 160, 89, 0.6); transform: translateY(-2px); }  
        .nav-link.active span { color: white; font-weight: 600; }  
        .nav-link::after { content: ''; position: absolute; bottom: 4px; width: 0; height: 2px; background: var(--gold-primary); transition: width 0.25s cubic-bezier(0.16, 1, 0.3, 1); }  
        .nav-link.active::after { width: 16px; }  
        .app-container { width: 100%; max-width: 480px; height: 100vh; background: var(--bg-absolute); position: relative; overflow: hidden; display: flex; flex-direction: column; }  
    </style>  
</head>  
<body class="flex items-center justify-center min-h-screen bg-[#020202]">  
    <div class="app-container border-x border-white/[0.03] shadow-2xl flex flex-col justify-between">  
        <div class="w-full bg-gradient-to-r from-[#8C7343] to-[#C5A059] text-black text-[9px] uppercase tracking-[0.15em] font-bold py-1.5 px-4 text-center shrink-0 flex items-center justify-center gap-1.5 z-50">  
            <i class="fa-solid fa-bolt-lightning animate-pulse"></i>   
            <span>Flash Sale Live: Use code <span class="underline">GOLD25</span> for 25% Off</span>  
        </div>  
        <header class="w-full pt-4 px-4 pb-3 bg-black/90 backdrop-blur-md border-b border-white/[0.04] shrink-0 z-40">  
            <div class="flex items-center justify-between mb-3">  
                <div class="flex flex-col">  
                    <span class="text-[8px] tracking-[0.3em] uppercase text-gray-500 font-bold">The Luxury Registry</span>  
                    <h1 class="text-[#C5A059] text-sm font-black uppercase luxury-title mt-0.5 cursor-pointer" onclick="window.location.href='index.html'">Digital Asset Hub</h1>  
                </div>  
                <div class="flex items-center gap-2">  
                    <button onclick="window.location.href='notifications.html'" class="w-8 h-8 rounded-full border border-white/10 bg-white/5 flex items-center justify-center text-gray-400 relative">  
                        <i class="fa-solid fa-bell text-xs"></i>  
                        <span id="globalNotificationIndicator" class="absolute top-1.5 right-1.5 w-1.5 h-1.5 bg-amber-400 rounded-full hidden"></span>  
                    </button>  
                </div>  
            </div>  
        </header>  
        <main class="flex-1 overflow-y-auto px-4 pb-24 pt-2 no-scrollbar space-y-5">  
            <div id="view-dashboard" class="application-viewport space-y-5">  
                <div class="grid grid-cols-2 gap-3">  
                    <div class="bg-gradient-to-br from-[#161411] to-[#0A0908] border border-[#C5A059]/20 p-3.5 rounded-xl">  
                        <span class="text-[8px] text-gray-500 uppercase tracking-widest block font-bold">Gross Allocated Capital</span>  
                        <span id="kpiGrossRevenue" class="text-base font-mono font-bold text-white mt-1 block">$1,450.00</span>  
                        <span class="text-[8px] text-emerald-400 font-bold block mt-1"><i class="fa-solid fa-arrow-trend-up"></i> +14.2% Audit Cycle</span>  
                    </div>  
                    <div class="bg-gradient-to-br from-[#161411] to-[#0A0908] border border-[#C5A059]/20 p-3.5 rounded-xl">  
                        <span class="text-[8px] text-gray-500 uppercase tracking-widest block font-bold">Verified Downloads Delivered</span>  
                        <span id="kpiTotalDownloads" class="text-base font-mono font-bold text-[#C5A059] mt-1 block">42</span>  
                        <span class="text-[8px] text-[#C5A059]/60 block mt-1">100% Secure Integrity</span>  
                    </div>  
                </div>  
                <div class="bg-[#12100E] border border-white/[0.04] rounded-xl p-3.5 space-y-2">  
                    <span class="text-[9px] font-bold text-gray-400 uppercase tracking-widest block">Operational Analytics Wave</span>  
                    <div class="h-20 flex items-end gap-2.5 pt-4 pb-1 px-2">  
                        <div class="flex-1 bg-[#8C7343]/20 hover:bg-[#C5A059]/40 h-[35%] rounded-t relative group transition-all"><span class="absolute -top-4 left-1/2 -translate-x-1/2 text-[8px] font-mono text-gray-400 opacity-0 group-hover:opacity-100 transition-opacity">$35</span></div>  
                        <div class="flex-1 bg-[#8C7343]/20 hover:bg-[#C5A059]/40 h-[55%] rounded-t relative group transition-all"><span class="absolute -top-4 left-1/2 -translate-x-1/2 text-[8px] font-mono text-gray-400 opacity-0 group-hover:opacity-100 transition-opacity">$55</span></div>  
                        <div class="flex-1 bg-[#8C7343]/20 hover:bg-[#C5A059]/40 h-[40%] rounded-t relative group transition-all"><span class="absolute -top-4 left-1/2 -translate-x-1/2 text-[8px] font-mono text-gray-400 opacity-0 group-hover:opacity-100 transition-opacity">$40</span></div>  
                        <div class="flex-1 bg-[#8C7343]/20 hover:bg-[#C5A059]/40 h-[85%] rounded-t relative group transition-all"><span class="absolute -top-4 left-1/2 -translate-x-1/2 text-[8px] font-mono text-gray-400 opacity-0 group-hover:opacity-100 transition-opacity">$85</span></div>  
                        <div class="flex-1 bg-[#C5A059] h-[95%] rounded-t relative group transition-all"><span class="absolute -top-4 left-1/2 -translate-x-1/2 text-[8px] font-mono text-white font-bold opacity-100">$120</span></div>  
                    </div>  
                    <div class="flex justify-between text-[8px] font-bold text-gray-600 tracking-wider font-mono">  
                        <span>MON</span><span>TUE</span><span>WED</span><span>THU</span><span>TODAY</span>  
                    </div>  
                </div>  
                <div class="space-y-3">  
                    <div class="flex justify-between items-center border-b border-white/[0.05] pb-1.5">  
                        <span class="text-[10px] font-black uppercase tracking-widest text-gray-400">Vault Asset Management</span>  
                        <button onclick="SystemCreatorDashboard.openPublishingModal()" class="text-[9px] font-bold text-black bg-[#C5A059] px-2.5 py-1 rounded tracking-wider uppercase"><i class="fa-solid fa-plus text-[8px]"></i> Mint Asset</button>  
                    </div>  
                    <div id="creatorCatalogInject" class="space-y-2.5"></div>  
                </div>  
            </div>  
        </main>  
        <div id="assetCreationOverlayHUD" class="absolute inset-0 bg-black/95 backdrop-blur-xl z-50 flex items-center justify-center p-5 hidden opacity-0 transition-all duration-300">  
            <div class="w-full bg-[#0E0D0B] border border-[#C5A059]/30 rounded-2xl p-5 space-y-4 max-h-[90vh] overflow-y-auto no-scrollbar shadow-2xl">  
                <div class="flex justify-between items-center border-b border-white/[0.05] pb-2">  
                    <h3 class="text-xs font-bold text-[#C5A059] uppercase tracking-widest luxury-title">Mint Vault Asset Token</h3>  
                    <button onclick="SystemCreatorDashboard.closePublishingModal()" class="text-gray-500 hover:text-white"><i class="fa-solid fa-xmark text-sm"></i></button>  
                </div>  
                <div class="space-y-3">  
                    <div>  
                        <label class="block text-[9px] uppercase tracking-wider text-gray-400 font-bold mb-1">Asset Nomenclature</label>  
                        <input type="text" id="mintNameField" placeholder="e.g., Cyberpunk UI Assets Pack" class="w-full bg-black border border-white/10 rounded p-2 text-xs text-white focus:outline-none focus:border-[#C5A059]">  
                    </div>  
                    <div>  
                        <label class="block text-[9px] uppercase tracking-wider text-gray-400 font-bold mb-1">Marketplace Classification</label>  
                        <select id="mintCategoryField" class="w-full bg-[#12100E] border border-white/10 rounded p-2 text-xs text-gray-300 focus:outline-none focus:border-[#C5A059]">  
                            <option value="AI">AI Products</option>  
                            <option value="EBook">E-Books</option>  
                            <option value="Software">Software</option>  
                            <option value="Templates">Templates</option>  
                        </select>  
                    </div>  
                    <div>  
                        <label class="block text-[9px] uppercase tracking-wider text-gray-400 font-bold mb-1">Value Asset Listing Price (USD)</label>  
                        <input type="number" id="mintPriceField" placeholder="49.00" class="w-full bg-black border border-white/10 rounded p-2 text-xs text-white focus:outline-none focus:border-[#C5A059]">  
                    </div>  
                    <div>  
                        <label class="block text-[9px] uppercase tracking-wider text-gray-400 font-bold mb-1">Short Context Description</label>  
                        <input type="text" id="mintDescField" placeholder="Premium architectural node resource..." class="w-full bg-black border border-white/10 rounded p-2 text-xs text-white focus:outline-none focus:border-[#C5A059]">  
                    </div>  
                    <button onclick="SystemCreatorDashboard.executeMintTransaction()" class="w-full bg-gradient-to-r from-[#8C7343] to-[#C5A059] text-black font-extrabold text-[10px] uppercase tracking-[0.15em] py-2.5 rounded-lg mt-2">  
                        Authorize Node Deployment  
                    </button>  
                </div>  
            </div>  
        </div>  
        <nav class="w-full bg-black/95 backdrop-blur-md border-t border-white/[0.04] py-2 px-6 flex items-center justify-between absolute bottom-0 left-0 right-0 z-40 shrink-0">  
            <button onclick="window.location.href='index.html'" id="navBtn-browse" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-gem text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Catalog</span>  
            </button>  
            <button onclick="window.location.href='wishlist.html'" id="navBtn-wishlist" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-heart text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Registry</span>  
            </button>  
            <button onclick="window.location.href='cart.html'" id="navBtn-cart" class="nav-link relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <div class="relative">  
                    <i class="fa-solid fa-vault text-xs"></i>  
                    <span id="navCartCountIndicator" class="absolute -top-1.5 -right-2 bg-[#C5A059] text-black text-[7px] font-black h-3.5 w-3.5 flex items-center justify-center rounded-full border border-black hidden">0</span>  
                </div>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Cart</span>  
            </button>  
            <button onclick="window.location.href='dashboard.html'" id="navBtn-dashboard" class="nav-link active relative flex flex-col items-center gap-1 text-gray-400 py-1 transition-all">  
                <i class="fa-solid fa-chart-line text-xs"></i>  
                <span class="text-[8px] uppercase tracking-wider font-semibold">Console</span>  
            </button>  
        </nav>  
    </div>  
    <script>  
        const memoryStore = window.localStorage;  
        let state = {  
            products: JSON.parse(memoryStore.getItem("dh_products")) || [],  
            cart: JSON.parse(memoryStore.getItem("dh_cart")) || [],  
            notifications: JSON.parse(memoryStore.getItem("dh_notifications")) || []  
        };  
        function saveStateToStorage() {  
            memoryStore.setItem("dh_products", JSON.stringify(state.products));  
            memoryStore.setItem("dh_notifications", JSON.stringify(state.notifications));  
        }  
        const SystemCreatorDashboard = {  
            openPublishingModal() {  
                const modal = document.getElementById("assetCreationOverlayHUD");  
                modal.classList.remove("hidden");  
                setTimeout(() => modal.classList.remove("opacity-0"), 10);  
            },  
            closePublishingModal() {  
                const modal = document.getElementById("assetCreationOverlayHUD");  
                modal.classList.add("opacity-0");  
                setTimeout(() => modal.classList.add("hidden"), 300);  
            },  
            executeMintTransaction() {  
                const name = document.getElementById("mintNameField").value.trim();  
                const cat = document.getElementById("mintCategoryField").value;  
                const price = parseFloat(document.getElementById("mintPriceField").value) || 29.00;  
                const desc = document.getElementById("mintDescField").value.trim() || "Premium digital compilation node asset asset framework collection.";  
                if(!name) { alert("Token identity field parameter required."); return; }  
                const newAsset = {  
                    id: "custom-" + Date.now(), title: name, description: desc, price: price, category: cat, rating: 5.0, author: "Anonymous Sovereign", badge: "new",  
                    image: "https://images.unsplash.com/photo-1614741118887-7a4ee193a5fa?w=400&q=80", tags: [cat, "Mntd"]  
                };  
                state.products.unshift(newAsset);  
                state.notifications.unshift({ id: Date.now(), text: `Asset ${name} successfully minted into ledger distribution lists.`, read: false, time: "Just Now" });  
                saveStateToStorage();  
                this.closePublishingModal();  
                document.getElementById("mintNameField").value = "";  
                document.getElementById("mintDescField").value = "";  
                this.renderConsole();  
            },  
            renderConsole() {  
                const inject = document.getElementById("creatorCatalogInject");  
                const internalAssets = state.products.filter(p => p.id.startsWith("custom-") || p.id.startsWith("asset-"));  
                inject.innerHTML = internalAssets.slice(0,3).map(p => `  
                    <div class="bg-black/40 border border-white/[0.04] rounded-lg p-2 flex items-center justify-between text-xs">  
                        <div class="flex items-center gap-2 truncate">  
                            <div class="w-1.5 h-1.5 bg-[#C5A059] rounded-full animate-pulse"></div>  
                            <span class="font-mono text-gray-300 truncate uppercase tracking-wider">${p.title}</span>  
                        </div>  
                        <span class="font-mono text-[#C5A059] text-[11px] shrink-0 font-bold">$${p.price.toFixed(2)}</span>  
                    </div>  
                `).join("");  
            }  
        };  
        document.addEventListener("DOMContentLoaded", () => {  
            const indicator = document.getElementById("navCartCountIndicator");  
            indicator.innerText = state.cart.length;  
            indicator.classList.toggle("hidden", state.cart.length === 0);  
            SystemCreatorDashboard.renderConsole();  
            const hasUnread = state.notifications.some(n => !n.read);  
            document.getElementById("globalNotificationIndicator").classList.toggle("hidden", !hasUnread);  
        });  
    </script>  
</body>  
</html>
