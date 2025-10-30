# Asesoría en Mecánica Automotriz — Advisor

> Onboarding público con GitHub Pages + pagos seguros con Stripe + backend en Firebase Functions (v2).

[🔗 Sitio en vivo (GitHub Pages)](https://asesoria-en-mecanica-automotriz.github.io/Asesoria-en-Mecanica-Automotriz/)  
[🔗 API base (Functions v2)](https://us-central1-asesor-automotriz-a06b7.cloudfunctions.net/api2)  
Región: **us-central1**

---

## 🎯 Qué ofrece
- **Atención 100% por WhatsApp** del cliente (sin chat web).
- **Planes mensuales**: Básico ($399, 6 consultas), Avanzado ($499, 10 consultas), PRO ($999, ilimitado).
- **Stripe** para cobro seguro, portal del cliente y cancelación en un clic.

---

## 🧩 Estructura rápida
- `index.html` → landing + CTAs WhatsApp + pago Stripe + Portal.
- Backend: Firebase Functions v2 → endpoint `api2`
- Secrets: `STRIPE_SECRET_KEY` en Secret Manager (habilitado).

---

## 🚀 Puesta en marcha (Frontend)
1. Coloca `index.html` en el root del repo **Asesoria-en-Mecanica-Automotriz**.
2. Activa **GitHub Pages** (Branch: `main` → `/ (root)`).
3. Verifica la URL pública:  
   `https://asesoria-en-mecanica-automotriz.github.io/Asesoria-en-Mecanica-Automotriz/`
4. En `index.html` confirma:
   ```js
   const API_BASE = "https://us-central1-asesor-automotriz-a06b7.cloudfunctions.net/api2";
   const PRICE_IDS = {
     basic: "price_1SEO1MHhTrAfLf1eXUPOP5VW",
     adv:   "price_1SEO1vHhTrAfLf1ezeReW7mFu",
     pro:   "price_1SENdDHhTrAfLf1eTnywP9m6"
   };
