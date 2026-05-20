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
            <!-- Ganti src dengan path foto kamu, atau hapus tag img untuk pakai inisial -->
            <span class="avatar-initials">{{ initials }}</span>
          </div>
        </div>
        <h1 class="name">Nama Kamu</h1>
        <p class="username">@namakamu</p>
        <p class="bio">Desainer · Developer · Kreator konten digital yang suka eksplorasi hal-hal baru 🌿</p>
        <div class="badges">
          <span class="badge">Available for work</span>
          <span class="badge">Yogyakarta, ID</span>
        </div>
      </section>

      <!-- ── LINK CARDS ── -->
      <section class="links">

        <a href="" target="_blank" rel="noopener" class="link-card secondary">
          <span class="link-icon">🌿</span>
          <span class="link-label">Portfolio &amp; Karya</span>
          <span class="link-tag">Featured</span>
          <span class="link-arrow">↗</span>
        </a>

        <!-- Tipe: secondary (transparan subtle) -->
        <a href="" target="_blank" rel="noopener" class="link-card secondary">
          <span class="link-icon">📝</span>
          <span class="link-label">Blog &amp; Tulisan</span>
          <span class="link-arrow">↗</span>
        </a>

        <a href="" target="_blank" rel="noopener" class="link-card secondary">
          <span class="link-icon">🤝</span>
          <span class="link-label">Jasa &amp; Kolaborasi</span>
          <span class="link-arrow">↗</span>
        </a>

        <a href="" target="_blank" rel="noopener" class="link-card secondary">
          <span class="link-icon">⚡</span>
          <span class="link-label">GitHub — Proyek Open Source</span>
          <span class="link-arrow">↗</span>
        </a>

        <a href="" target="_blank" rel="noopener" class="link-card secondary">
          <span class="link-icon">💌</span>
          <span class="link-label">Newsletter Mingguan</span>
          <span class="link-arrow">↗</span>
        </a>

        <a href="" class="link-card secondary">
          <span class="link-icon">✉️</span>
          <span class="link-label">Hubungi Saya</span>
          <span class="link-arrow">↗</span>
        </a>
      </section>

      <!-- ── SOSIAL MEDIA ── -->
      <section class="socials">

        <a href="https://instagram.com/namakamu" target="_blank" rel="noopener" class="social-btn" title="Instagram">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
            <rect x="2" y="2" width="20" height="20" rx="5"/>
            <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/>
            <line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/>
          </svg>
        </a>

        <a href="https://twitter.com/namakamu" target="_blank" rel="noopener" class="social-btn" title="X / Twitter">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor">
            <path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/>
          </svg>
        </a>

        <a href="https://linkedin.com/in/namakamu" target="_blank" rel="noopener" class="social-btn" title="LinkedIn">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
            <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/>
            <rect x="2" y="9" width="4" height="12"/>
            <circle cx="4" cy="4" r="2"/>
          </svg>
        </a>

        <a href="https://youtube.com/@namakamu" target="_blank" rel="noopener" class="social-btn" title="YouTube">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
            <path d="M22.54 6.42a2.78 2.78 0 0 0-1.95-1.96C18.88 4 12 4 12 4s-6.88 0-8.59.46a2.78 2.78 0 0 0-1.95 1.96A29 29 0 0 0 1 12a29 29 0 0 0 .46 5.58A2.78 2.78 0 0 0 3.41 19.6C5.12 20 12 20 12 20s6.88 0 8.59-.46a2.78 2.78 0 0 0 1.95-1.95A29 29 0 0 0 23 12a29 29 0 0 0-.46-5.58z"/>
            <polygon points="9.75 15.02 15.5 12 9.75 8.98 9.75 15.02"/>
          </svg>
        </a>

        <a href="https://tiktok.com/@namakamu" target="_blank" rel="noopener" class="social-btn" title="TikTok">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor">
            <path d="M19.59 6.69a4.83 4.83 0 0 1-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 0 1-2.88 2.5 2.89 2.89 0 0 1-2.89-2.89 2.89 2.89 0 0 1 2.89-2.89c.28 0 .54.04.79.1V9.01a6.34 6.34 0 0 0-.79-.05 6.34 6.34 0 0 0-6.34 6.34 6.34 6.34 0 0 0 6.34 6.34 6.34 6.34 0 0 0 6.33-6.34V8.69a8.18 8.18 0 0 0 4.78 1.52V6.76a4.85 4.85 0 0 1-1.01-.07z"/>
          </svg>
        </a>

      </section>

      <footer class="footer">
        <span>Dibuat dengan ♡ · {{ new Date().getFullYear() }}</span>
      </footer>

    </main>
  </div>
</template>

<script setup>
import { computed } from 'vue'

// ──────────────────────────────────────────────────────────
//  GANTI NAMA DI SINI untuk inisial avatar fallback
// ──────────────────────────────────────────────────────────
const namaLengkap = 'Nama Kamu'

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
*, *::before, *::after {
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
.links .link-card:nth-child(1) { animation-delay: 0.05s; }
.links .link-card:nth-child(2) { animation-delay: 0.10s; }
.links .link-card:nth-child(3) { animation-delay: 0.15s; }
.links .link-card:nth-child(4) { animation-delay: 0.20s; }
.links .link-card:nth-child(5) { animation-delay: 0.25s; }
.links .link-card:nth-child(6) { animation-delay: 0.30s; }

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