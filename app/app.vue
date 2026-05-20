<template>
  <div class="page">
    <div class="orb orb-1"></div>
    <div class="orb orb-2"></div>
    <div class="orb orb-3"></div>

    <main class="container">

      <!-- ── PROFIL ── -->
      <section class="profile">
        <div class="avatar-ring">
          <div class="avatar">
            <img :src="logo" alt="Logo" class="w-full h-full object-cover rounded-full" />
          </div>
        </div>
        <h1 class="name">SMK Tamansiswa Jetis - Yogyakarta</h1>
        <p class="bio">Desainer · Developer · Engineer</p>
        <div class="badges">
          <span class="badge">Desain Komunikasi Visual</span>
          <span class="badge">Rekayasa Perangkat Lunak</span>
          <span class="badge">Teknik Instalasi Tenaga Listrik</span>
          <span class="badge">Teknik Kendaraan Ringan</span>
          <span class="badge">Teknik Sepeda Motor</span>
          <span class="badge">SMK Pusat Keunggulan</span>
          <span class="badge">Teaching Factory</span>
        </div>
      </section>

      <!-- ── LINK CARDS ── -->


      <section class="links">

        <a href="https://www.instagram.com/smktamsisjetis_yk/" target="_blank" rel="noopener"
          class="link-card secondary">
          <span class="link-icon">📸</span>
          <span class="link-label">Instagram</span>
          <span class="link-arrow">↗</span>
        </a>

        <a href="https://www.tiktok.com/@smktamansiswajetisyk" target="_blank" rel="noopener"
          class="link-card secondary">
          <span class="link-icon">🎵</span>
          <span class="link-label">TikTok</span>
          <span class="link-arrow">↗</span>
        </a>

        <a href="https://www.youtube.com/channel/UCNlnrmRvfH4XsJsjp7XUO1w" target="_blank" rel="noopener"
          class="link-card secondary">
          <span class="link-icon">▶️</span>
          <span class="link-label">YouTube</span>
          <span class="link-arrow">↗</span>
        </a>

        <a href="https://wa.me/6288232128784" target="_blank" rel="noopener" class="link-card secondary">
          <span class="link-icon">💬</span>
          <span class="link-label">WhatsApp</span>
          <span class="link-arrow">↗</span>
        </a>

      </section>

      <footer class="footer">
        <span>Copyright RPL Team· {{ new Date().getFullYear() }}</span>
      </footer>

    </main>
  </div>
</template>

<script setup>
import { computed } from 'vue'
import logo from '~/assets/img/logo.webp'

// ──────────────────────────────────────────────────────────
//  GANTI NAMA DI SINI untuk inisial avatar fallback
// ──────────────────────────────────────────────────────────
const namaLengkap = 'SMK Tamansiswa Jetis'

const initials = computed(() =>
  namaLengkap.split(' ').map(w => w[0]).join('').slice(0, 2).toUpperCase()
)

useHead({
  title: `${namaLengkap} — Links`,
  meta: [{ name: 'description', content: 'Semua link dalam satu tempat.' }],
  link: [
    { rel: 'preconnect', href: 'https://fonts.googleapis.com' },
    { rel: 'preconnect', href: 'https://fonts.gstatic.com', crossorigin: '' },
    { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,400;0,9..40,500;0,9..40,600;0,9..40,700&display=swap' },
  ],
})
</script>

<style>
/* ── Reset ─────────────────────────────────────────── */
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  background: #0a1a0d;
  color: #e8f5eb;
  font-family: 'DM Sans', 'Segoe UI', sans-serif;
}

a {
  text-decoration: none;
  color: inherit;
}

img {
  display: block;
  max-width: 100%;
}

/* ── Halaman ────────────────────────────────────────── */
.page {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  padding: 3rem 1rem 4rem;
  position: relative;
  overflow: hidden;
}

/* ── Orb background ─────────────────────────────────── */
.orb {
  position: fixed;
  border-radius: 50%;
  pointer-events: none;
  z-index: 0;
}

.orb-1 {
  width: 480px;
  height: 480px;
  background: radial-gradient(circle, #1a5c2a 0%, transparent 70%);
  top: -140px;
  right: -80px;
  opacity: 0.5;
  filter: blur(72px);
}

.orb-2 {
  width: 380px;
  height: 380px;
  background: radial-gradient(circle, #0d3d1a 0%, transparent 70%);
  bottom: -90px;
  left: -60px;
  opacity: 0.6;
  filter: blur(60px);
}

.orb-3 {
  width: 280px;
  height: 280px;
  background: radial-gradient(circle, #2d7a3e 0%, transparent 70%);
  top: 42%;
  left: 50%;
  transform: translateX(-50%);
  opacity: 0.12;
  filter: blur(48px);
}

/* ── Container utama ────────────────────────────────── */
.container {
  position: relative;
  z-index: 1;
  width: 100%;
  max-width: 460px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

/* ── Profil ─────────────────────────────────────────── */
.profile {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  gap: 0.45rem;
  animation: fadeUp 0.6s ease both;
}

.avatar-ring {
  padding: 3px;
  border-radius: 50%;
  background: linear-gradient(135deg, #3dca6a, #1a7a3a, #0f4d22);
  margin-bottom: 0.2rem;
}

.avatar {
  width: 88px;
  height: 88px;
  border-radius: 50%;
  background: #1a3d20;
  border: 3px solid #0a1a0d;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}

.avatar-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.avatar-initials {
  font-size: 1.75rem;
  font-weight: 700;
  color: #5ee87e;
  letter-spacing: -0.02em;
}

.name {
  font-size: 1.5rem;
  font-weight: 700;
  color: #e8f5eb;
  letter-spacing: -0.02em;
  line-height: 1.2;
}

.username {
  font-size: 0.875rem;
  color: #4dae65;
  font-weight: 500;
  letter-spacing: 0.02em;
}

.bio {
  font-size: 0.9rem;
  color: #8ab898;
  max-width: 320px;
  line-height: 1.65;
}

.badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.45rem;
  justify-content: center;
  margin-top: 0.15rem;
}

.badge {
  font-size: 0.72rem;
  font-weight: 600;
  color: #3dca6a;
  background: rgba(61, 202, 106, 0.1);
  border: 1px solid rgba(61, 202, 106, 0.22);
  border-radius: 100px;
  padding: 0.22rem 0.7rem;
  letter-spacing: 0.01em;
}

/* ── Link cards ─────────────────────────────────────── */
.links {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 0.7rem;
}

.link-card {
  position: relative;
  display: flex;
  align-items: center;
  gap: 0.9rem;
  padding: 1rem 1.2rem;
  border-radius: 14px;
  border: 1px solid rgba(255, 255, 255, 0.07);
  transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  animation: fadeUp 0.6s ease both;
  overflow: hidden;
}

/* Shimmer overlay */
.link-card::before {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(135deg, rgba(255, 255, 255, 0.04) 0%, transparent 55%);
  pointer-events: none;
}

.link-card:hover {
  transform: translateY(-2px) scale(1.01);
  border-color: rgba(61, 202, 106, 0.4);
  box-shadow: 0 8px 28px rgba(0, 0, 0, 0.3), 0 0 0 1px rgba(61, 202, 106, 0.08);
}

.link-card:active {
  transform: translateY(0) scale(0.99);
}

/* Variasi warna card */
.link-card.primary {
  background: linear-gradient(135deg, #1d5928 0%, #153d1c 100%);
  border-color: rgba(61, 202, 106, 0.28);
}

.link-card.secondary {
  background: rgba(255, 255, 255, 0.04);
}

.link-card.accent {
  background: rgba(61, 202, 106, 0.08);
  border-color: rgba(61, 202, 106, 0.2);
}

.link-card.ghost {
  background: transparent;
}

/* Bagian dalam card */
.link-icon {
  font-size: 1.2rem;
  width: 36px;
  height: 36px;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgba(255, 255, 255, 0.06);
  border-radius: 10px;
}

.link-label {
  flex: 1;
  font-size: 0.95rem;
  font-weight: 600;
  color: #dff0e3;
  letter-spacing: -0.01em;
}

.link-tag {
  font-size: 0.62rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: #3dca6a;
  background: rgba(61, 202, 106, 0.15);
  border-radius: 100px;
  padding: 2px 8px;
  flex-shrink: 0;
}

.link-arrow {
  font-size: 1rem;
  color: #4dae65;
  flex-shrink: 0;
  transition: transform 0.2s ease;
}

.link-card:hover .link-arrow {
  transform: translate(2px, -2px);
}

/* Delay animasi per kartu (stagger manual) */
.links .link-card:nth-child(1) {
  animation-delay: 0.05s;
}

.links .link-card:nth-child(2) {
  animation-delay: 0.10s;
}

.links .link-card:nth-child(3) {
  animation-delay: 0.15s;
}

.links .link-card:nth-child(4) {
  animation-delay: 0.20s;
}

.links .link-card:nth-child(5) {
  animation-delay: 0.25s;
}

.links .link-card:nth-child(6) {
  animation-delay: 0.30s;
}

/* ── Sosial Media ────────────────────────────────────── */
.socials {
  display: flex;
  gap: 0.65rem;
  flex-wrap: wrap;
  justify-content: center;
  animation: fadeUp 0.6s ease 0.38s both;
}

.social-btn {
  width: 44px;
  height: 44px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.08);
  display: flex;
  align-items: center;
  justify-content: center;
  color: #8ab898;
  transition: background 0.2s, border-color 0.2s, color 0.2s, transform 0.2s;
}

.social-btn:hover {
  background: rgba(61, 202, 106, 0.12);
  border-color: rgba(61, 202, 106, 0.38);
  color: #3dca6a;
  transform: translateY(-2px);
}

.social-btn svg {
  display: block;
}

/* ── Footer ──────────────────────────────────────────── */
.footer {
  font-size: 0.76rem;
  color: #3d5e42;
  animation: fadeUp 0.6s ease 0.45s both;
}

/* ── Animasi ─────────────────────────────────────────── */
@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(16px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* ── Responsive ──────────────────────────────────────── */
@media (max-width: 480px) {
  .page {
    padding: 2rem 1rem 3rem;
  }

  .name {
    font-size: 1.3rem;
  }

  .link-card {
    padding: 0.875rem 1rem;
  }

  .avatar {
    width: 78px;
    height: 78px;
  }
}
</style>