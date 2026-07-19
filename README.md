const INDEX_PAGE = "<!DOCTYPE html>\n<html lang=\"cs\" class=\"scroll-smooth\">\n<head>\n    <meta charset=\"UTF-8\">\n    <meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">\n    <title>Iuventus, gaude! | Pěvecký sbor</title>\n    <meta name=\"description\" content=\"Oficiální stránky pěveckého sboru Iuventus, gaude! — místo, kde se setkává vášeň pro hudbu s přátelstvím.\">\n    <script src=\"https://cdn.tailwindcss.com\"></script>\n    <script>\n        tailwind.config = { \n            theme: { \n                extend: { \n                    colors: { \n                        brandingOrange: '#E85002', \n                        darkBlack: '#171717', \n                        lightGray: '#F9F9F9' \n                    } \n                } \n            } \n        }\n    </script>\n    <link rel=\"preconnect\" href=\"https://fonts.googleapis.com\">\n    <link rel=\"preconnect\" href=\"https://fonts.gstatic.com\" crossorigin>\n    <link href=\"https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap\" rel=\"stylesheet\">\n    <style>\n        body { font-family: 'Inter', sans-serif; }\n        .gradient-text { \n            background: linear-gradient(135deg, #E85002 0%, #000000 100%);\n            -webkit-background-clip: text;\n            -webkit-text-fill-color: transparent;\n        }\n        .glass-card { \n            background: linear-gradient(180deg, #ffffff 0%, #fefefe 100%);\n            border: 1px solid rgba(0,0,0,0.05);\n        }\n        .mobile-menu { max-height: 0; overflow: hidden; transition: max-height 0.3s ease-in-out; }\n        .mobile-menu.open { max-height: 500px; }\n    </style>\n</head>\n<body class=\"bg-white text-darkBlack\">\n\n<!-- Navigační lišta -->\n<nav class=\"sticky top-0 bg-white z-50 border-b border-gray-100\">\n    <div class=\"max-w-7xl mx-auto px-6 py-6 flex justify-between items-center\">\n        <a href=\"index.html\" class=\"text-2xl font-bold tracking-tighter\">\n            Iuventus, gaude!\n        </a>\n        <button id=\"menuBtn\" class=\"lg:hidden text-2xl\" onclick=\"document.getElementById('mobileMenu').classList.toggle('open')\">\n            ☰\n        </button>\n        <div class=\"hidden lg:flex space-x-6 text-sm font-medium items-center\">\n            <a href=\"index.html\" class=\"text-brandingOrange\">Domů</a>\n            <a href=\"o-sboru.html\" class=\"hover:text-brandingOrange transition\">O sboru</a>\n            <a href=\"galerie.html\" class=\"hover:text-brandingOrange transition\">Galerie</a>\n            <a href=\"vedeni.html\" class=\"hover:text-brandingOrange transition\">Sbormistr a vedení</a>\n            <a href=\"koncerty.html\" class=\"hover:text-brandingOrange transition\">Koncerty a akce</a>\n            <a href=\"pridej-se.html\" class=\"hover:text-brandingOrange transition\">Přidej se k nám!</a>\n            <a href=\"pro-rodice.html\" class=\"hover:text-brandingOrange transition\">Pro rodiče</a>\n            <a href=\"podpora.html\" class=\"hover:text-brandingOrange transition\">Chci podpořit</a>\n            <a href=\"kontakt.html\" class=\"bg-darkBlack text-white px-5 py-2.5 rounded-full hover:bg-brandingOrange transition\">Kontakt</a>\n        </div>\n    </div>\n    <div id=\"mobileMenu\" class=\"mobile-menu lg:hidden\">\n        <div class=\"flex flex-col gap-4 px-6 pb-6 text-sm font-medium\">\n            <a href=\"index.html\" class=\"text-brandingOrange\">Domů</a>\n            <a href=\"o-sboru.html\" class=\"hover:text-brandingOrange transition\">O sboru</a>\n            <a href=\"galerie.html\" class=\"hover:text-brandingOrange transition\">Galerie</a>\n            <a href=\"vedeni.html\" class=\"hover:text-brandingOrange transition\">Sbormistr a vedení</a>\n            <a href=\"koncerty.html\" class=\"hover:text-brandingOrange transition\">Koncerty a akce</a>\n            <a href=\"pridej-se.html\" class=\"hover:text-brandingOrange transition\">Přidej se k nám!</a>\n            <a href=\"pro-rodice.html\" class=\"hover:text-brandingOrange transition\">Pro rodiče</a>\n            <a href=\"podpora.html\" class=\"hover:text-brandingOrange transition\">Chci podpořit</a>\n            <a href=\"kontakt.html\" class=\"bg-darkBlack text-white px-5 py-2.5 rounded-full text-center\">Kontakt</a>\n        </div>\n    </div>\n</nav>\n\n<!-- Hero -->\n<header class=\"max-w-7xl mx-auto px-6 pt-20 pb-32\">\n    <h1 class=\"text-7xl md:text-8xl font-bold tracking-tighter mb-8 leading-[0.9]\">\n        Radost, <br>\n        <span class=\"gradient-text\">která zní.</span>\n    </h1>\n    <p class=\"text-xl text-gray-500 max-w-xl mb-10\">\n        Oficiální stránky pěveckého sboru Iuventus, gaude! – místo,\n        kde se setkává vášeň pro hudbu s přátelstvím.\n    </p>\n    <div class=\"flex gap-4\">\n        <a href=\"pridej-se.html\" class=\"bg-brandingOrange text-white px-8 py-4 rounded-xl font-bold hover:bg-black transition\">Přidej se k nám</a>\n        <a href=\"koncerty.html\" class=\"border border-gray-200 px-8 py-4 rounded-xl font-bold hover:bg-lightGray transition\">Naše koncerty</a>\n    </div>\n</header>\n\n<!-- Sekce -->\n<section class=\"bg-lightGray py-24\">\n<div class=\"max-w-7xl mx-auto px-6\">\n<h2 class=\"text-4xl font-bold mb-16 tracking-tighter\">Informace o sboru</h2>\n<div class=\"grid md:grid-2 lg:grid-cols-4 gap-8\">\n<a href=\"o-sboru.html\" class=\"glass-card p-8 rounded-3xl\">\n<h3 class=\"font-bold text-lg mb-2\">O sboru</h3>\n<p class=\"text-sm text-gray-600\">Historie, naše poslání a hudební směřování.</p>\n</a>\n<a href=\"galerie.html\" class=\"glass-card p-8 rounded-3xl\">\n<h3 class=\"font-bold text-lg mb-2\">Galerie</h3>\n<p class=\"text-sm text-gray-600\">Fotoreportáže z koncertů a momentky ze života sboru.</p>\n</a>\n<a href=\"vedeni.html\" class=\"glass-card p-8 rounded-3xl\">\n<h3 class=\"font-bold text-lg mb-2\">Sbormistr a vedení</h3>\n<p class=\"text-sm text-gray-600\">Dirigent, korepetitor a organizační tým.</p>\n</a>\n<a href=\"koncerty.html\" class=\"glass-card p-8 rounded-3xl\">\n<h3 class=\"font-bold text-lg mb-2\">Koncerty a akce</h3>\n<p class=\"text-sm text-gray-600\">Kalendář vystoupení a archiv akcí.</p>\n</a>\n<a href=\"pridej-se.html\" class=\"glass-card p-8 rounded-3xl\">\n<h3 class=\"font-bold text-lg mb-2\">Přidej se k nám!</h3>\n<p class=\"text-sm text-gray-600\">Informace pro nové členy.</p>\n</a>\n<a href=\"pro-rodice.html\" class=\"glass-card p-8 rounded-3xl\">\n<h3 class=\"font-bold text-lg mb-2\">Pro rodiče</h3>\n<p class=\"text-sm text-gray-600\">Termíny, informace a pokyny.</p>\n</a>\n<a href=\"podpora.html\" class=\"glass-card p-8 rounded-3xl\">\n<h3 class=\"font-bold text-lg mb-2\">Chci podpořit</h3>\n<p class=\"text-sm text-gray-600\">Partnerství, dary a podpora sboru.</p>\n</a>\n</div>\n</div>\n</section>\n\n<!-- Kontakt -->\n<footer class=\"max-w-7xl mx-auto px-6 py-24\">\n<h2 class=\"text-5xl font-bold tracking-tighter mb-12\">Kontakt</h2>\n<div class=\"grid md:grid-cols-2 gap-16\">\n<div class=\"space-y-4\">\n<p>Máte dotaz? Napište nám e-mail nebo nás sledujte na sociálních sítích.</p>\n<a href=\"mailto:iuventus@zusjbc.cz\" class=\"text-brandingOrange text-2xl font-bold underline\">iuventus@zusjbc.cz</a>\n</div>\n</div>\n</footer>\n</body>\n</html>";
const COMING_SOON_PAGE = "<!DOCTYPE html>\n<html lang=\"cs\" class=\"scroll-smooth\">\n<head>\n<meta charset=\"UTF-8\">\n<meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">\n<title>Připravujeme | Iuventus, gaude!</title>\n<script src=\"https://cdn.tailwindcss.com\"></script>\n<script>\ntailwind.config = { theme: { extend: { colors: { brandingOrange: '#E85002', darkBlack: '#171717', lightGray: '#F9F9F9' } } } }\n</script>\n<link rel=\"preconnect\" href=\"https://fonts.googleapis.com\">\n<link href=\"https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap\" rel=\"stylesheet\">\n<style>body { font-family: 'Inter', sans-serif; }</style>\n</head>\n<body class=\"bg-white text-darkBlack\">\n<nav class=\"sticky top-0 bg-white z-50 border-b border-gray-100\">\n<div class=\"max-w-7xl mx-auto px-6 py-6 flex justify-between items-center\">\n<a href=\"index.html\" class=\"text-2xl font-bold tracking-tighter\">Iuventus, gaude!</a>\n<button class=\"lg:hidden text-2xl\" onclick=\"document.getElementById('mobileMenu').classList.toggle('open')\">☰</button>\n<div class=\"hidden lg:flex space-x-6 text-sm font-medium items-center\">\n<a href=\"index.html\" class=\"hover:text-brandingOrange transition\">Domů</a>\n<a href=\"o-sboru.html\" class=\"hover:text-brandingOrange transition\">O sboru</a>\n<a href=\"galerie.html\" class=\"hover:text-brandingOrange transition\">Galerie</a>\n<a href=\"vedeni.html\" class=\"hover:text-brandingOrange transition\">Sbormistr a vedení</a>\n<a href=\"koncerty.html\" class=\"hover:text-brandingOrange transition\">Koncerty a akce</a>\n<a href=\"pridej-se.html\" class=\"hover:text-brandingOrange transition\">Přidej se k nám!</a>\n<a href=\"pro-rodice.html\" class=\"hover:text-brandingOrange transition\">Pro rodiče</a>\n<a href=\"podpora.html\" class=\"hover:text-brandingOrange transition\">Chci podpořit</a>\n<a href=\"kontakt.html\" class=\"bg-darkBlack text-white px-5 py-2.5 rounded-full\">Kontakt</a>\n</div>\n</div>\n</nav>\n<main class=\"max-w-7xl mx-auto px-6 py-32 text-center\">\n<h1 class=\"text-6xl font-bold tracking-tighter mb-6\">Připravujeme</h1>\n<p class=\"text-xl text-gray-500 max-w-xl mx-auto mb-10\">Tato stránka je ještě ve vývoji. Vraťte se prosím později.</p>\n<a href=\"index.html\" class=\"bg-brandingOrange text-white px-8 py-4 rounded-xl font-bold hover:bg-black transition\">Zpět na úvod</a>\n</main>\n</body>\n</html>";

const CONTACT_PAGE = `<!DOCTYPE html>
<html lang="cs" class="scroll-smooth">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kontakt | Iuventus, gaude!</title>
<meta name="description" content="Kontaktujte sbor Iuventus, gaude! — koncerty, členství, spolupráce.">
<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = {
    theme: {
        extend: {
            colors: {
                brandingOrange: '#E85002',
                darkBlack: '#171717',
                lightGray: '#F9F9F9'
            }
        }
    }
}
</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap" rel="stylesheet">
<style>
body { font-family:'Inter', sans-serif; }
.gradient-text {
    background: linear-gradient(135deg,#E85002 0%,#000000 100%);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}
.no-scrollbar::-webkit-scrollbar { display:none; }
.no-scrollbar { scrollbar-width:none; }
.mobile-menu { max-height: 0; overflow: hidden; transition: max-height 0.3s ease-in-out; }
.mobile-menu.open { max-height: 500px; }
</style>
</head>
<body class="bg-white text-darkBlack">

<!-- NAVIGACE -->
<nav class="sticky top-0 bg-white z-50 border-b border-gray-100">
<div class="max-w-7xl mx-auto px-6 py-6 flex justify-between items-center">
<a href="index.html" class="text-2xl font-bold tracking-tighter">
Iuventus, gaude!
</a>
<button id="menuBtn" class="lg:hidden text-2xl" onclick="document.getElementById('mobileMenu').classList.toggle('open')">
☰
</button>
<div class="hidden lg:flex space-x-6 text-sm font-medium items-center">
<a href="index.html" class="hover:text-brandingOrange transition">Domů</a>
<a href="o-sboru.html" class="hover:text-brandingOrange transition">O sboru</a>
<a href="galerie.html" class="hover:text-brandingOrange transition">Galerie</a>
<a href="vedeni.html" class="hover:text-brandingOrange transition">Sbormistr a vedení</a>
<a href="koncerty.html" class="hover:text-brandingOrange transition">Koncerty a akce</a>
<a href="pridej-se.html" class="hover:text-brandingOrange transition">Přidej se k nám!</a>
<a href="pro-rodice.html" class="hover:text-brandingOrange transition">Pro rodiče</a>
<a href="podpora.html" class="hover:text-brandingOrange transition">Chci podpořit</a>
<a href="kontakt.html" class="bg-darkBlack text-white px-5 py-2.5 rounded-full">Kontakt</a>
</div>
</div>
<div id="mobileMenu" class="mobile-menu lg:hidden">
<div class="flex flex-col gap-4 px-6 pb-6 text-sm font-medium">
<a href="index.html" class="hover:text-brandingOrange transition">Domů</a>
<a href="o-sboru.html" class="hover:text-brandingOrange transition">O sboru</a>
<a href="galerie.html" class="hover:text-brandingOrange transition">Galerie</a>
<a href="vedeni.html" class="hover:text-brandingOrange transition">Sbormistr a vedení</a>
<a href="koncerty.html" class="hover:text-brandingOrange transition">Koncerty a akce</a>
<a href="pridej-se.html" class="hover:text-brandingOrange transition">Přidej se k nám!</a>
<a href="pro-rodice.html" class="hover:text-brandingOrange transition">Pro rodiče</a>
<a href="podpora.html" class="hover:text-brandingOrange transition">Chci podpořit</a>
<a href="kontakt.html" class="bg-darkBlack text-white px-5 py-2.5 rounded-full text-center">Kontakt</a>
</div>
</div>
</nav>

<main class="max-w-7xl mx-auto px-6 py-24">

<!-- HLAVIČKA -->
<header class="flex justify-between items-end mb-16">
<div>
<h1 class="text-6xl font-bold tracking-tighter mb-5">
Náš tým
</h1>
<p class="text-xl text-gray-500 max-w-xl">
Poznejte lidi, kteří tvoří sbor Iuventus, gaude!
</p>
</div>
<div class="flex gap-4">
<button onclick="document.getElementById('slider').scrollBy({left:-350,behavior:'smooth'})"
class="w-12 h-12 rounded-full bg-lightGray hover:bg-gray-200 transition text-xl">
←
</button>
<button onclick="document.getElementById('slider').scrollBy({left:350,behavior:'smooth'})"
class="w-12 h-12 rounded-full bg-lightGray hover:bg-gray-200 transition text-xl">
→
</button>
</div>
</header>

<!-- SLIDER -->
<section id="slider" class="flex gap-8 overflow-x-auto no-scrollbar snap-x pb-10">

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Mgr. Anežka Šebová</h3>
<p class="text-gray-500 mb-3">Sbormistryně koncertního sboru Iuventus, gaude!</p>
<p class="text-sm text-gray-600">774 762 228</p>
<a href="mailto:sebova@zusjbc.cz" class="text-sm text-brandingOrange hover:underline">sebova@zusjbc.cz</a>
</div>

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Jitka Melicheríková</h3>
<p class="text-gray-500 mb-3">Sbormistryně předkoncertního sboru Amici, gaudete! a přípravného sboru Liberi, gaudete!</p>
<p class="text-sm text-gray-600">777 579 071</p>
<a href="mailto:melicherikova@zusjbc.cz" class="text-sm text-brandingOrange hover:underline">melicherikova@zusjbc.cz</a>
</div>

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Blanka Šubrtová</h3>
<p class="text-gray-500 mb-3">Sbormistryně přípravného sboru Pueri, gaudete!</p>
<p class="text-sm text-gray-600">605 806 642</p>
<a href="mailto:subrtova@zusjbc.cz" class="text-sm text-brandingOrange hover:underline">subrtova@zusjbc.cz</a>
</div>

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Donika Krasniqi</h3>
<p class="text-gray-500 mb-3">Hlasová poradkyně</p>
<p class="text-sm text-gray-600">774 417 707</p>
<a href="mailto:krasniqi@zusjbc.cz" class="text-sm text-brandingOrange hover:underline">krasniqi@zusjbc.cz</a>
</div>

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Veronika Devine</h3>
<p class="text-gray-500 mb-3">Hlasová poradkyně</p>
<p class="text-sm text-gray-600">733 747 891</p>
<a href="mailto:devina@zusjbc.cz" class="text-sm text-brandingOrange hover:underline">devina@zusjbc.cz</a>
</div>

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Jarmila Klokočníková</h3>
<p class="text-gray-500 mb-3">Hlasová poradkyně</p>
<p class="text-sm text-gray-600">774 762 229</p>
<a href="mailto:klokocnikova@zusjbc.cz" class="text-sm text-brandingOrange hover:underline">klokocnikova@zusjbc.cz</a>
</div>

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Zuzana Růžičková</h3>
<p class="text-gray-500 mb-3">Hlasová poradkyně</p>
<p class="text-sm text-gray-600">606 583 281</p>
<a href="mailto:ruzickova.zuzana12@gmail.com" class="text-sm text-brandingOrange hover:underline">ruzickova.zuzana12@gmail.com</a>
</div>

<div class="min-w-[280px] snap-start">
<div class="aspect-[3/4] bg-lightGray rounded-3xl mb-6"></div>
<h3 class="font-bold text-xl">Jitka Holová</h3>
<p class="text-gray-500 mb-3">Předsedkyně SRPDŠ a hlavní koordinátorka</p>
<p class="text-sm text-gray-600">607 762 226</p>
<a href="mailto:iuventus@zusjbc.cz" class="text-sm text-brandingOrange hover:underline">iuventus@zusjbc.cz</a>
</div>

</section>

<!-- KONTAKT -->
<div class="border-t border-gray-100 pt-24 mt-20 grid md:grid-cols-12 gap-16">
<div class="md:col-span-5">
<h2 class="text-5xl font-bold tracking-tighter mb-8">
Kontaktujte nás
</h2>
<p class="text-lg text-gray-500">
Máte otázku ohledně koncertů, členství nebo spolupráce?
Rádi vám odpovíme.
</p>
<br>
<a href="mailto:iuventus@zusjbc.cz" class="text-brandingOrange text-2xl font-bold underline">
iuventus@zusjbc.cz
</a>
<div class="mt-10 pt-10 border-t border-gray-100 text-sm text-gray-500 space-y-1">
<p class="font-bold text-darkBlack text-base mb-2">Spolek rodičů a přátel dětí a školy při ZUŠ</p>
<p>IČO: 04033264</p>
<p>Podhorská 47, 466 01 Jablonec nad Nisou, ČR</p>
<p>Číslo účtu: 2000802432/2010 (Fio banka)</p>
<p class="pt-3 font-bold text-darkBlack text-base mb-1">Zkušebna</p>
<p>Horní náměstí 800/1, Jablonec nad Nisou, ČR</p>
</div>
</div>
<div class="md:col-span-7 bg-lightGray p-12 rounded-3xl">
<form id="contactForm" method="POST" class="space-y-8">
<input type="text" name="name" placeholder="Jméno a příjmení" required
class="w-full bg-transparent border-b border-gray-300 py-3 text-lg outline-none focus:border-brandingOrange">
<input type="email" name="email" placeholder="E-mail" required
class="w-full bg-transparent border-b border-gray-300 py-3 text-lg outline-none focus:border-brandingOrange">
<textarea name="message" placeholder="Zpráva" rows="3" required
class="w-full bg-transparent border-b border-gray-300 py-3 text-lg outline-none focus:border-brandingOrange"></textarea>
<button type="submit"
class="bg-brandingOrange text-white px-10 py-4 rounded-xl font-bold hover:bg-black transition">
Odeslat
</button>
<div id="formStatus" class="hidden text-lg font-medium"></div>
</form>
</div>
</div>
</main>

<script>
document.getElementById('contactForm').addEventListener('submit', async (e) => {
    e.preventDefault();
    const status = document.getElementById('formStatus');
    const btn = e.target.querySelector('button[type="submit"]');
    btn.disabled = true;
    btn.textContent = 'Odesílám...';

    const formData = new FormData(e.target);
    try {
        const res = await fetch(window.location.pathname, {
            method: 'POST',
            body: JSON.stringify({
                name: formData.get('name'),
                email: formData.get('email'),
                message: formData.get('message')
            }),
            headers: { 'Content-Type': 'application/json' }
        });
        if (res.ok) {
            status.textContent = '✓ Děkujeme! Vaše zpráva byla odeslána.';
            status.className = 'text-lg font-medium text-green-600';
            e.target.reset();
        } else {
            throw new Error();
        }
    } catch (err) {
        status.textContent = '✗ Omlouváme se, odeslání se nezdařilo. Zkuste to prosím znovu.';
        status.className = 'text-lg font-medium text-red-600';
    }
    status.classList.remove('hidden');
    btn.disabled = false;
    btn.textContent = 'Odeslat';
});
</script>
</body>
</html>`;
// ============================================================
// NOVÉ/UPRAVENÉ konstanty pro worker.js
// Vložte je vedle stávajících (INDEX_PAGE, CONTACT_PAGE, ...)
// a doplňte routy dole podle návodu na konci souboru.
// ============================================================

const NAV = `
<nav class="sticky top-0 bg-white z-50 border-b border-gray-100">
    <div class="max-w-7xl mx-auto px-6 py-6 flex justify-between items-center">
        <a href="index.html" class="text-2xl font-bold tracking-tighter">Iuventus, gaude!</a>
        <button class="lg:hidden text-2xl" onclick="document.getElementById('mobileMenu').classList.toggle('open')">☰</button>
        <div class="hidden lg:flex space-x-6 text-sm font-medium items-center">
            <a href="index.html" class="hover:text-brandingOrange transition">Domů</a>
            <a href="o-sboru.html" class="hover:text-brandingOrange transition">O sboru</a>
            <a href="galerie.html" class="hover:text-brandingOrange transition">Galerie</a>
            <a href="vedeni.html" class="hover:text-brandingOrange transition">Sbormistr a vedení</a>
            <a href="koncerty.html" class="hover:text-brandingOrange transition">Koncerty a akce</a>
            <a href="pridej-se.html" class="hover:text-brandingOrange transition">Přidej se k nám!</a>
            <a href="pro-rodice.html" class="hover:text-brandingOrange transition">Pro rodiče</a>
            <a href="podpora.html" class="hover:text-brandingOrange transition">Chci podpořit</a>
            <a href="kontakt.html" class="bg-darkBlack text-white px-5 py-2.5 rounded-full hover:bg-brandingOrange transition">Kontakt</a>
        </div>
    </div>
    <div id="mobileMenu" class="mobile-menu lg:hidden">
        <div class="flex flex-col gap-4 px-6 pb-6 text-sm font-medium">
            <a href="index.html" class="hover:text-brandingOrange transition">Domů</a>
            <a href="o-sboru.html" class="hover:text-brandingOrange transition">O sboru</a>
            <a href="galerie.html" class="hover:text-brandingOrange transition">Galerie</a>
            <a href="vedeni.html" class="hover:text-brandingOrange transition">Sbormistr a vedení</a>
            <a href="koncerty.html" class="hover:text-brandingOrange transition">Koncerty a akce</a>
            <a href="pridej-se.html" class="hover:text-brandingOrange transition">Přidej se k nám!</a>
            <a href="pro-rodice.html" class="hover:text-brandingOrange transition">Pro rodiče</a>
            <a href="podpora.html" class="hover:text-brandingOrange transition">Chci podpořit</a>
            <a href="kontakt.html" class="bg-darkBlack text-white px-5 py-2.5 rounded-full text-center">Kontakt</a>
        </div>
    </div>
</nav>`;

const HEAD = (title, desc) => `
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>${title} | Iuventus, gaude!</title>
<meta name="description" content="${desc}">
<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = { theme: { extend: { colors: { brandingOrange: '#E85002', darkBlack: '#171717', lightGray: '#F9F9F9' } } } }
</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap" rel="stylesheet">
<style>
body { font-family: 'Inter', sans-serif; }
.mobile-menu { max-height: 0; overflow: hidden; transition: max-height 0.3s ease-in-out; }
.mobile-menu.open { max-height: 500px; }
</style>`;

// ------------------------------------------------------------
// O SBORU  (zdroj: Wix "O nás")
// ------------------------------------------------------------
const O_SBORU_PAGE = `<!DOCTYPE html>
<html lang="cs" class="scroll-smooth">
<head>${HEAD('O sboru', 'Historie a úspěchy dětského pěveckého sboru Iuventus, gaude! od jeho založení v roce 2005.')}</head>
<body class="bg-white text-darkBlack">
${NAV}
<main class="max-w-4xl mx-auto px-6 py-24">
<h1 class="text-6xl font-bold tracking-tighter mb-12">O sboru</h1>

<div class="prose max-w-none space-y-6 text-lg text-gray-700 leading-relaxed">
<p>Dětský pěvecký sbor Iuventus, gaude! byl založen v září 2005 při Základní umělecké škole v Jablonci nad Nisou. Sbormistryní je Bc. Anežka Šebová. Za svou existenci se sbor stal významnou a ceněnou součástí severočeského kulturního života, získal si mnoho příznivců a mimořádně brzy po svém vzniku začal sbírat ocenění na soutěžích v České republice i v zahraničí.</p>

<p>Úspěchy sboru jsou zásluhou velké pracovitosti, nadšení a talentu dětí i vynikající práce pedagogů za podpory Základní umělecké školy a Statutárního města Jablonec nad Nisou, ale také nezištné pomoci mnoha příznivců a rodičů. Za dlouhodobé úspěchy vyhlásila Unie českých pěveckých sborů Iuventus, gaude! nejúspěšnějším českým sborem roku 2012. V roce 2015 byl sbor pozván na prestižní festival Pražské jaro.</p>

<h2 class="text-3xl font-bold tracking-tighter pt-6">2018</h2>
<p>Rok se nesl v duchu příprav na celosvětovou sborovou olympiádu World Choir Games v jihoafrickém Tshwane, odkud koncertní sbor přivezl zlatou medaili z kategorie duchovní hudby a stříbrnou ze spirituálů. Přípravný sbor Amici, gaudete! získal zlato na Svátcích písní Olomouc. Sborové děti se podílely na albu Ondřeje Rumla Zapomenuté světlo za účasti Boleslava Polívky.</p>

<h2 class="text-3xl font-bold tracking-tighter pt-6">2017</h2>
<p>Sbor nastudoval projekt Otvírání studánek v rámci ZUŠ OPEN, v červenci koncertoval na Mezinárodním hudebním festivalu v Provence a Aveyronu ve Francii a na podzim vystoupil společně s houslistou Jaroslavem Svěceným na benefičním koncertu pro liberecký hospic.</p>

<h2 class="text-3xl font-bold tracking-tighter pt-6">2016</h2>
<p>Hlavní náplní byla příprava koncertního sboru na samostatný koncert v rámci festivalu Pražské jaro, který se uskutečnil 28. května v kostele sv. Šimona a Judy v Praze. Na mezinárodní soutěži Per Musicam ad Astra v polské Toruni zvítězil sbor v kategorii Grand Prix napříč všemi věkovými kategoriemi.</p>

<h2 class="text-3xl font-bold tracking-tighter pt-6">2015</h2>
<p>Hlavní sbor slavnostně provedl absolventskou skladbu sbormistra Tomáše Pospíšila Liturgické obrazy ze života Šimona Petra. Amici, gaudete! získali zlaté pásmo na mezinárodním festivalu písní v Olomouci, koncertní sbor přivezl zlaté pásmo a 2. místo v Grand Prix ze soutěže Musica Sacra a Roma.</p>

<h2 class="text-3xl font-bold tracking-tighter pt-6">2014</h2>
<p>Sbor vystoupil v lotyšské Rize a získal dvě zlaté medaile. V Praze na AMU provedl skladby Jana Vičara ke skladatelovým 65. narozeninám a v listopadu vystoupil s houslistou Alexandrem Shonertem s programem Shalom – pokoj.</p>

<h2 class="text-3xl font-bold tracking-tighter pt-6">2013</h2>
<p>Sbor se s velkým úspěchem zúčastnil festivalu sborového zpěvu Festival choral v jižní Francii, kterého se účastnilo přes 30 000 diváků ve čtyřiceti městech Provence, spolu se sbory z Itálie, Bulharska, Lotyšska, Tchaj-wanu a Jižní Afriky.</p>
</div>
</main>
</body>
</html>`;

// ------------------------------------------------------------
// GALERIE  (zdroj: Wix "Fotogalerie" — fotky jsou v Google Photos albech)
// ------------------------------------------------------------
const GALERIE_PAGE = `<!DOCTYPE html>
<html lang="cs" class="scroll-smooth">
<head>${HEAD('Galerie', 'Fotogalerie z koncertů, zkoušek a zájezdů sboru Iuventus, gaude!.')}</head>
<body class="bg-white text-darkBlack">
${NAV}
<main class="max-w-5xl mx-auto px-6 py-24">
<h1 class="text-6xl font-bold tracking-tighter mb-6">Fotogalerie</h1>
<p class="text-xl text-gray-500 mb-16">Fotky z našich akcí najdete v albech Google Photos — stačí kliknout na rok a akci.</p>

<div class="space-y-10">
<div>
<h2 class="text-2xl font-bold mb-3">2026</h2>
<a href="https://photos.app.goo.gl/FU9LxLaxcBW8fhRQ6" class="text-brandingOrange underline font-medium">Kompletní archiv (461 snímků)</a>
</div>

<div>
<h2 class="text-2xl font-bold mb-3">2025</h2>
<ul class="space-y-2 text-gray-700">
<li><a href="https://photos.app.goo.gl/vB4KDbZJ8fkP2mSB8" class="text-brandingOrange underline">Děti zpívají dětem aneb putování za sborovou pohádkou</a></li>
<li><a href="https://photos.app.goo.gl/VTC7jdTSVkY69Lz29" class="text-brandingOrange underline">28. dubna 2025</a></li>
<li><a href="https://photos.app.goo.gl/3dVZjzQsE91bGXJQ8" class="text-brandingOrange underline">Fotogalerie</a></li>
<li><a href="https://photos.app.goo.gl/v3Nothk1A2bXxnzXA" class="text-brandingOrange underline">Fotogalerie</a></li>
<li><a href="https://photos.app.goo.gl/uoxGWABwhf4Ukheq8" class="text-brandingOrange underline">IG! 20 let</a></li>
</ul>
</div>

<div>
<h2 class="text-2xl font-bold mb-3">2024</h2>
<ul class="space-y-2 text-gray-700">
<li><a href="https://photos.app.goo.gl/tjCS3su2uwQK1sRT8" class="text-brandingOrange underline">Rozsvícení vánočního stromu — 1. prosince 2024, Jablonec n. N.</a></li>
<li><a href="https://photos.app.goo.gl/Z3eNFw1v6kDs18cS6" class="text-brandingOrange underline">Festival Alta Pusteria, Itálie</a></li>
<li><a href="https://photos.app.goo.gl/sWnwyJ1LJtJQW8nx8" class="text-brandingOrange underline">Jablonecké tóny — Jiří Pavlica & Hradišťan & IG!</a></li>
<li><a href="https://photos.app.goo.gl/HFEVJBEzgKaXS5gz6" class="text-brandingOrange underline">31. května 2024</a></li>
<li><a href="https://photos.app.goo.gl/D2V4H3DdcjaPXgCd7" class="text-brandingOrange underline">Tříkrálový koncert IG! 2024</a></li>
<li><a href="https://photos.app.goo.gl/JGcFJEkn2UAt1dWY6" class="text-brandingOrange underline">Fotogalerie</a></li>
</ul>
</div>

<div>
<h2 class="text-2xl font-bold mb-3">2023</h2>
<ul class="space-y-2 text-gray-700">
<li><a href="https://photos.app.goo.gl/FESbXVCHUXnEhg6q9" class="text-brandingOrange underline">Rozsvícení vánočního stromu, Zbrankov</a></li>
<li><a href="https://photos.app.goo.gl/j5DUzMBE6uk6zh6K6" class="text-brandingOrange underline">Řasnice</a></li>
<li><a href="https://photos.app.goo.gl/nwGFGNdPhLMutwmW8" class="text-brandingOrange underline">Jarní zpívání s IG! 2023</a></li>
</ul>
</div>
</div>
</main>
</body>
</html>`;

// ------------------------------------------------------------
// KONCERTY  (zdroj: Wix "Koncerty")
// ------------------------------------------------------------
const KONCERTY_PAGE = `<!DOCTYPE html>
<html lang="cs" class="scroll-smooth">
<head>${HEAD('Koncerty a akce', 'Kalendář koncertů a záznamy vystoupení sboru Iuventus, gaude!.')}</head>
<body class="bg-white text-darkBlack">
${NAV}
<main class="max-w-4xl mx-auto px-6 py-24">
<h1 class="text-6xl font-bold tracking-tighter mb-6">Koncerty a akce</h1>
<p class="text-xl text-gray-500 mb-16">Kalendář koncertů, představení a soustředění je plný zajímavých akcí. A náš YouTube kanál je naplněný videi ze všeho dění kolem sboru.</p>

<div class="grid md:grid-cols-2 gap-8">
<div class="glass-card border border-gray-100 p-10 rounded-3xl">
<h2 class="text-2xl font-bold mb-3">Video</h2>
<p class="text-gray-600 mb-6">Nahrávky máme uložené na našem YouTube kanále — výběr videí z koncertů a vystoupení.</p>
<a href="https://www.youtube.com/user/Iuventusgaude/" class="bg-brandingOrange text-white px-6 py-3 rounded-xl font-bold inline-block hover:bg-black transition">Vstoupit na YouTube</a>
</div>

<div class="glass-card border border-gray-100 p-10 rounded-3xl">
<h2 class="text-2xl font-bold mb-3">Poslechnout na Spotify</h2>
<p class="text-gray-600 mb-6">Nahrávky "Gaudete et exultate" a "Cantate Domino" (Live) najdete i na Spotify.</p>
<a href="https://open.spotify.com/artist/4oJC1Fq7ptGa88Vvzpx883" class="bg-brandingOrange text-white px-6 py-3 rounded-xl font-bold inline-block hover:bg-black transition">Otevřít na Spotify</a>
</div>

<div class="glass-card border border-gray-100 p-10 rounded-3xl">
<h2 class="text-2xl font-bold mb-3">Akce</h2>
<p class="text-gray-600 mb-6">Koncerty, soustředění a další akce ve spolupráci se ZUŠ nebo s hosty najdete ve sborovém Google kalendáři.</p>
<a href="https://calendar.google.com/calendar/embed?src=iuventus%40zusjbc.cz&ctz=Europe%2FPrague" class="bg-brandingOrange text-white px-6 py-3 rounded-xl font-bold inline-block hover:bg-black transition">Otevřít kalendář</a>
</div>
</div>
</main>
</body>
</html>`;

// ------------------------------------------------------------
// PODPORA  (zdroj: Wix "Podporují nás")
// ------------------------------------------------------------
const PODPORA_PAGE = `<!DOCTYPE html>
<html lang="cs" class="scroll-smooth">
<head>${HEAD('Chci podpořit', 'Partneři a sponzoři, kteří podporují dětský sbor Iuventus, gaude!.')}</head>
<body class="bg-white text-darkBlack">
${NAV}
<main class="max-w-5xl mx-auto px-6 py-24">
<h1 class="text-6xl font-bold tracking-tighter mb-6">Děkujeme za podporu</h1>
<p class="text-xl text-gray-500 mb-10">Bez našich partnerů a sponzorů by řada projektů, zájezdů a soutěží nebyla možná.</p>

<div class="bg-lightGray rounded-3xl p-10 mb-16">
<h2 class="text-2xl font-bold mb-2">Aktuální sbírka: Iuventus letí do Španělska</h2>
<p class="text-gray-600 mb-6">Pomozte nám pokrýt náklady na cestu, ubytování a soutěžní poplatky, aby mohly odletět skutečně všechny děti.</p>
<div data-darujme-widget-token="ahdiu8hj0k96rmms"></div>
</div>

<div class="grid grid-cols-2 md:grid-cols-4 gap-6 items-center mb-20">
<a href="https://www.koop.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Kooperativa</a>
<a href="http://www.kbs-security.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">KBS Security</a>
<a href="https://www.jablotron.com/cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Jablotron</a>
<a href="https://ceskamincovna.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Česká mincovna</a>
<a href="http://www.geosa.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Geosa</a>
<a href="http://www.miton.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Miton</a>
<a href="https://www.kitl.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Kitl</a>
<a href="https://www.atrea.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Atrea</a>
<a href="https://www.zf.com/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">ZF</a>
<a href="https://unitherm.cz/cs" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Unitherm</a>
<a href="http://www.evosa.cz/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Evosa</a>
<a href="https://www.valbek.cz/cs/" class="border border-gray-100 rounded-2xl p-6 text-center font-medium hover:bg-lightGray transition">Valbek</a>
</div>

<div class="bg-lightGray rounded-3xl p-12">
<h2 class="text-3xl font-bold tracking-tighter mb-4">Chcete nás podpořit i vy?</h2>
<p class="text-gray-600 mb-6">Podpora sboru je možná finančně i formou partnerství. Napište nám na e-mail nebo zavolejte.</p>
<a href="mailto:iuventus@zusjbc.cz" class="text-brandingOrange text-xl font-bold underline">iuventus@zusjbc.cz</a>
</div>
</main>

<script type="text/javascript">
+function(w,d,s,u,a,b){w['DarujmeObject']=u;w[u]=w[u]||function(){(w[u].q=w[u].q||[]).push(arguments)};a=d.createElement(s);b=d.getElementsByTagName(s)[0];a.async=1;a.src="https://www.darujme.cz/assets/scripts/widget.js";b.parentNode.insertBefore(a,b)}(window,document,'script','Darujme');
Darujme(1,"ahdiu8hj0k96rmms",'render',"https://www.darujme.cz/widget?token=ahdiu8hj0k96rmms","270px");
</script>
</body>
</html>`;

// ------------------------------------------------------------
// PRO RODIČE  (zdroj: Wix "Pro rodiče" — podstránky IG!/AG! jsou heslované)
// ------------------------------------------------------------
const PRO_RODICE_PAGE = `<!DOCTYPE html>
<html lang="cs" class="scroll-smooth">
<head>${HEAD('Pro rodiče', 'Informace pro rodiče členů sborů Iuventus, gaude! a Amici, gaudete!.')}</head>
<body class="bg-white text-darkBlack">
${NAV}
<main class="max-w-4xl mx-auto px-6 py-24">
<h1 class="text-6xl font-bold tracking-tighter mb-16">Pro rodiče</h1>

<div class="grid md:grid-cols-2 gap-8">
<div class="glass-card border border-gray-100 p-10 rounded-3xl">
<h2 class="text-2xl font-bold mb-4">Iuventus, gaude!</h2>
<p class="text-gray-600 mb-6">koncertní sbor</p>
<a href="#" class="bg-darkBlack text-white px-6 py-3 rounded-xl font-bold inline-block hover:bg-brandingOrange transition">Vstup pro rodiče IG!</a>
</div>
<div class="glass-card border border-gray-100 p-10 rounded-3xl">
<h2 class="text-2xl font-bold mb-4">Amici, gaudete!</h2>
<p class="text-gray-600 mb-6">předkoncertní sbor</p>
<a href="#" class="bg-darkBlack text-white px-6 py-3 rounded-xl font-bold inline-block hover:bg-brandingOrange transition">Vstup pro rodiče AG!</a>
</div>
</div>
<p class="text-sm text-gray-400 mt-10">Pozn.: sekce pro rodiče jsou chráněné heslem — odkazy je potřeba doplnit po zprovoznění přihlašování.</p>
</main>
</body>
</html>`;

export default {
  async fetch(request) {
    const url = new URL(request.url);

    if (request.method === 'POST') {
      try {
        const data = await request.json();
        console.log('Kontakt:', JSON.stringify(data));
        return new Response(JSON.stringify({ success: true }), {
          status: 200,
          headers: { 'Content-Type': 'application/json' }
        });
      } catch (err) {
        return new Response(JSON.stringify({ success: false }), {
          status: 500,
          headers: { 'Content-Type': 'application/json' }
        });
      }
    }

    const path = url.pathname;

    if (path === '/' || path === '/index.html') {
      return new Response(INDEX_PAGE, { headers: { 'Content-Type': 'text/html; charset=utf-8' } });
    }
    if (path === '/kontakt.html') {
      return new Response(CONTACT_PAGE, { headers: { 'Content-Type': 'text/html; charset=utf-8' } });
    }
    if (path === '/o-sboru.html') {
      return new Response(O_SBORU_PAGE, { headers: { 'Content-Type': 'text/html; charset=utf-8' } });
    }
    if (path === '/galerie.html') {
      return new Response(GALERIE_PAGE, { headers: { 'Content-Type': 'text/html; charset=utf-8' } });
    }
    if (path === '/koncerty.html') {
      return new Response(KONCERTY_PAGE, { headers: { 'Content-Type': 'text/html; charset=utf-8' } });
    }
    if (path === '/podpora.html') {
      return new Response(PODPORA_PAGE, { headers: { 'Content-Type': 'text/html; charset=utf-8' } });
    }
    if (path === '/pro-rodice.html') {
      return new Response(PRO_RODICE_PAGE, { headers: { 'Content-Type': 'text/html; charset=utf-8' } });
    }

    return new Response(COMING_SOON_PAGE, {
      status: 200,
      headers: { 'Content-Type': 'text/html; charset=utf-8' }
    });
  }
};
