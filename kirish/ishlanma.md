**Video Mavzusi:** Next.js 15 ga Kirish: Nima, Nega va Qanday Boshlash Kerak?

**Maqsad:** Tomoshabinlarda Next.js nima ekanligi, uning asosiy afzalliklari va qanday qilib birinchi loyihani yaratish mumkinligi haqida dastlabki tushuncha hosil qilish. Ularni keyingi darslarni ko'rishga qiziqtirish.

**Taxminiy Davomiyligi:** 5-10 daqiqa

**Video Rejasi:**

**1. Kirish**
    *   Assalomu Alekum. Mening ismim Muhiddin va men fullstack web developer. Men o'z kanalimda tenxalogiya va dasturlashga oid video darslik va maqolalar yozib boraman.
    *   Video mavzusini e'lon qilish: "Bugun biz zamonaviy web developmentda eng mashhur frameworklardan biri - Next.js ning eng so'nggi, 15-versiyasiga kirish qilamiz."
    *   Next.js nima, nima uchun kerak, asosiy xususiyatlari, o'rnatish va ilk sahifa.
    *   React asoslarini biladiganlar uchun ideal, lekin yangi boshlovchilar ham tushunishi mumkin.
    *   eng so'nggi funksiyalar, optimallashtirishlar, React 19 bilan integratsiya va hkz.

**2. Next.js Nima? (What is Next.js?)**
    *   Oddiy ta'rif: Next.js - bu Vercel tomonidan yaratilgan, production-uchun tayyor React ilovalarini qurishga mo'ljallangan ochiq kodli (open-source) framework.
    *   "React ustiga qurilgan framework" ekanligini tushuntirish: React faqat UI yaratish kutubxonasi, Next.js esa routing, data fetching, rendering kabi ko'plab qo'shimcha imkoniyatlar va strukturani taqdim etadi.
    *   Asosiy maqsadi: Ishlab chiquvchi tajribasini (Developer Experience - DX) yaxshilash va yuqori samarali (performant) web-ilovalar yaratishni osonlashtirish.

**3. Nima Uchun Next.js? (Why Next.js?)**
    *   **Rendering Strategiyalari:**
        *   Server-Side Rendering (SSR): SEO uchun yaxshi, sahifaning ilk yuklanishi tez.
        *   Static Site Generation (SSG): Juda tez yuklanadigan statik saytlar uchun.
        *   Incremental Static Regeneration (ISR): Statik saytlarni belgilangan intervalda qayta generatsiya qilish.
        *   **App Router va Server Components:** Zamonaviy Next.js (13+) ning asosiy qismi. Serverda va klientda ishlash logikasini ajratish imkoniyati. (Bunga keyingi darslarda batafsil to'xtalishni aytish).
    *   **File-Based Routing:** `app` (yoki `pages`) papkasidagi fayl strukturasi asosida avtomatik ravishda route'lar yaratilishi. Juda intuitiv va qulay.
    *   **API Routes:** Backend logikasini frontend loyihasi ichida (`app/api/` orqali) yozish imkoniyati.
    *   **O'rnatilgan Optimallashtirishlar:**
        *   Image Optimization (`next/image`)
        *   Font Optimization (`next/font`)
        *   Script Optimization (`next/script`)
    *   **Developer Experience (DX):** Tezkor yangilanish (Fast Refresh), TypeScript qo'llab-quvvatlashi, ESLint integratsiyasi va hkz.
    *   **React 19 Xususiyatlari bilan Integratsiya (v15):** React Compiler (hozircha experimental), Actions kabi yangiliklarni qo'llab-quvvatlashi (qisqacha aytib o'tish).

**4. Boshlashdan Oldin (Prerequisites) (1 daqiqa)**
    *   HTML, CSS asoslari.
    *   JavaScript (ES6+ sintaksisi).
    *   **Muhim:** React asoslari (Components, Props, State, Hooks - `useState`, `useEffect`).
    *   Kompyuterda Node.js va npm/yarn/pnpm o'rnatilgan bo'lishi kerakligi.
    *   Terminal (command line) bilan ishlash bo'yicha minimal tajriba.

**5. O'rnatish va Loyiha Strukturasi (Installation & Project Structure) (4-5 daqiqa)**
    *   Terminalni ochish va `npx create-next-app@latest` buyrug'ini ishlatish (yoki yarn/pnpm).
    *   O'rnatish jarayonidagi savollarga qisqacha izoh berish (TypeScript?, ESLint?, Tailwind CSS?, `src` directory?, **App Router? (Yes - tavsiya etiladi)**, import alias?). *App Router tanlash muhimligini ta'kidlang.*
    *   O'rnatish tugagach, loyiha papkasiga kirish (`cd my-app`).
    *   Development serverni ishga tushirish (`npm run dev`).
    *   Brauzerda ochilgan standart Next.js sahifasini ko'rsatish.
    *   Asosiy papkalar va fayllarni juda qisqacha tanishtirish:
        *   `app/`: Asosiy ilova logikasi shu yerda (routing, sahifalar).
            *   `layout.tsx` (yoki `.js`): Umumiy sahifa strukturasi (root layout).
            *   `page.tsx` (yoki `.js`): Bosh sahifa komponenti (`/` route).
        *   `public/`: Statik fayllar (rasmlar, ikonlar).
        *   `package.json`: Bog'liqliklar va skriptlar.
        *   `next.config.mjs`: Next.js konfiguratsiya fayli.

**6. Birinchi Sahifani O'zgartirish ("Salom Dunyo!") (1-2 daqiqa)**
    *   `app/page.tsx` faylini ochish.
    *   Mavjud kodni o'chirib, oddiy "Salom Next.js 15!" yoki shunga o'xshash matn chiqaradigan sodda React komponentini yozish.
        ```jsx
        export default function HomePage() {
          return (
            <main>
              <h1>Salom Next.js 15!</h1>
              <p>Bu mening birinchi Next.js sahifam.</p>
            </main>
          );
        }
        ```
    *   Faylni saqlash va brauzerda avtomatik yangilanishni (Fast Refresh) ko'rsatish.
    *   Bu fayl qanday qilib asosiy sahifa (`/`) bo'lib xizmat qilayotganini tushuntirish (file-based routing prinsipi).

**7. Xulosa va Keyingi Qadamlar (Conclusion & What's Next) (1 daqiqa)**
    *   Next.js nima, afzalliklari, o'rnatish, ilk sahifa.
    *   Next.js 15 ning kuchli va zamonaviy framework ekanligini ta'kidlash.
    *   Keyingi videolarda nimalar haqida gaplashilishini aytish (Routing haqida gaplashamiz).
    *   Tomoshabinlarni savollar berishga, fikr bildirishga va keyingi darslarni kutishga undash.

**8. Yakunlash (Outro) (30 soniya)**
    *   Ko'rganlik uchun rahmat aytish.
    *   Kanalga obuna bo'lish, like bosish va qo'ng'iroqchani yoqishni eslatish.
    *   Xayrlashish.

**Vizual Elementlar:**

*   Sizning ekrandagi ko'rinishingiz (agar webcam ishlatsangiz).
*   Kod muharriri (VS Code va hkz.).
*   Terminal oynasi.
*   Web-brauzer.
*   Kerakli joylarda matnli slaydlar yoki grafikalar (masalan, afzalliklarni sanashda).

Ushbu reja sizga Next.js 15 haqidagi birinchi video darsligingizni sifatli va tushunarli qilib tayyorlashga yordam beradi deb umid qilaman. Omad!
