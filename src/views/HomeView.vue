<script setup lang="ts">
import { ref, onMounted } from 'vue'

const introVisible = ref(true)

onMounted(() => {
  setTimeout(() => {
    introVisible.value = false
  }, 2400)
})

const techStack = [
  {
    name: 'Vue.js',
    site: 'https://vuejs.org',
    icon: 'https://cdn.simpleicons.org/vuedotjs/42b883',
  },
  {
    name: 'Nuxt',
    site: 'https://nuxt.com',
    icon: 'https://cdn.simpleicons.org/nuxt/00dc82',
  },
  {
    name: 'React',
    site: 'https://react.dev',
    icon: 'https://cdn.simpleicons.org/react/61dafb',
  },
  {
    name: 'Tailwind CSS',
    site: 'https://tailwindcss.com',
    icon: 'https://cdn.simpleicons.org/tailwindcss/06b6d4',
  },
  {
    name: 'FastAPI',
    site: 'https://fastapi.tiangolo.com',
    icon: 'https://cdn.simpleicons.org/fastapi/009688',
  },
  {
    name: 'Django',
    site: 'https://www.djangoproject.com',
    icon: 'https://cdn.simpleicons.org/django/092e20',
  },
  {
    name: 'Node.js',
    site: 'https://nodejs.org',
    icon: 'https://cdn.simpleicons.org/nodedotjs/339933',
  },
  {
    name: 'PostgreSQL',
    site: 'https://www.postgresql.org',
    icon: 'https://cdn.simpleicons.org/postgresql/4169e1',
  },
  {
    name: 'Linux',
    site: 'https://kernel.org',
    icon: 'https://cdn.simpleicons.org/linux/fcc624',
  },
  {
    name: 'Nginx',
    site: 'https://nginx.org',
    icon: 'https://cdn.simpleicons.org/nginx/009639',
  },
  {
    name: 'Stripe',
    site: 'https://stripe.com',
    icon: 'https://cdn.simpleicons.org/stripe/635bff',
  },
  {
    name: 'Git',
    site: 'https://git-scm.com',
    icon: 'https://cdn.simpleicons.org/git/f05032',
  },
]
</script>

<template>
  <!-- INTRO SPLASH -->
  <Transition name="intro-fade">
    <div
      v-if="introVisible"
      class="intro-overlay fixed inset-0 z-[100] flex flex-col items-center justify-center bg-[var(--accent-200)]"
    >
      <div class="intro-logo text-6xl font-black tracking-tight text-white sm:text-8xl">RG</div>
      <div
        class="intro-tagline mt-4 text-sm font-semibold uppercase tracking-[0.25em] text-[var(--primary-300)] sm:text-base"
      >
        Senior Full Stack Developer
      </div>
      <div class="intro-bar mt-8 h-[3px] w-20 rounded-full bg-[var(--accent-100)]"></div>
    </div>
  </Transition>

  <main class="relative overflow-hidden bg-[var(--bg-200)] text-[var(--text-100)]">
    <div class="pointer-events-none absolute inset-0">
      <div
        class="floating-aura absolute -top-32 -left-24 h-96 w-96 rounded-full bg-[var(--primary-300)] blur-3xl opacity-70"
      ></div>
      <div
        class="floating-aura-delayed absolute top-1/3 -right-20 h-80 w-80 rounded-full bg-[var(--primary-200)] blur-3xl opacity-35"
      ></div>
      <div
        class="floating-aura-slow absolute bottom-0 left-1/3 h-72 w-72 rounded-full bg-[var(--accent-100)] blur-3xl opacity-20"
      ></div>
    </div>

    <div class="relative mx-auto max-w-6xl px-6 py-10 sm:px-8 lg:px-10">
      <div class="glow-border-wrap reveal-step-1 relative mb-14 rounded-3xl p-[2px]">
        <header
          class="relative rounded-3xl bg-white/90 p-6 shadow-[0_20px_60px_-35px_var(--accent-200)] backdrop-blur md:p-10"
        >
          <div class="grid gap-8 md:grid-cols-[1.5fr_1fr] md:items-center">
            <div>
              <p
                class="inline-flex rounded-full border border-[var(--primary-200)] bg-[var(--primary-300)]/60 px-4 py-1 text-xs font-semibold uppercase tracking-[0.18em] text-[var(--accent-200)]"
              >
                Montevideo, Uruguay · Remoto
              </p>
              <h1
                class="name-shimmer mt-5 text-4xl font-black leading-tight sm:text-5xl md:text-6xl"
              >
                Rodolfo Groero
              </h1>
              <p class="mt-3 text-lg font-semibold text-[var(--primary-100)] sm:text-xl">
                Ingeniero Informatico | Senior Full Stack Developer
              </p>
              <p class="mt-5 max-w-2xl text-sm leading-relaxed text-[var(--text-200)] sm:text-base">
                Ingeniero Informatico Senior Full Stack con experiencia construyendo plataformas web
                completas de punta a punta: frontend, backend, bases de datos, despliegue y
                optimizacion para negocio. He liderado equipos, tomado decisiones de arquitectura e
                integrado IA en proyectos reales en produccion.
              </p>
              <p
                class="mt-4 max-w-2xl rounded-xl border border-[var(--primary-200)]/40 bg-[var(--primary-300)]/35 px-4 py-3 text-sm font-semibold leading-relaxed text-[var(--accent-200)]"
              >
                Capaz de crear cualquier aplicacion a medida: desde la captura de requerimientos
                hasta el despliegue, configuracion de dominios, puesta en produccion y optimizacion
                SEO.
              </p>
              <div class="mt-7 flex flex-wrap gap-3">
                <a
                  href="mailto:rodolfogroero2@gmail.com"
                  class="rounded-xl bg-[var(--primary-100)] px-5 py-3 text-sm font-semibold text-white transition hover:bg-[var(--accent-200)]"
                >
                  Contactar por email
                </a>
                <a
                  href="https://github.com/Rodolf-GitHub"
                  target="_blank"
                  rel="noopener noreferrer"
                  class="rounded-xl border border-[var(--primary-100)] px-5 py-3 text-sm font-semibold text-[var(--primary-100)] transition hover:bg-[var(--primary-100)] hover:text-white"
                >
                  Ver GitHub
                </a>
              </div>
              <div class="mt-6 flex flex-wrap gap-x-5 gap-y-2 text-sm text-[var(--text-200)]">
                <span>rodolfogroero2@gmail.com</span>
                <span>+598 91854 199</span>
              </div>
            </div>

            <div class="mx-auto w-full max-w-xs">
              <div
                class="photo-frame relative rounded-3xl bg-gradient-to-br from-[var(--primary-200)] via-[var(--accent-100)] to-[var(--accent-200)] p-[3px] shadow-2xl shadow-[var(--accent-200)]/20 transition duration-500 hover:scale-[1.03] hover:shadow-[0_30px_80px_-30px_var(--accent-200)]"
              >
                <img
                  src="/foto_rodolfo.jpg"
                  alt="Rodolfo Groero"
                  class="aspect-[4/5] w-full rounded-[22px] object-cover transition duration-500 hover:brightness-105"
                  loading="eager"
                />
              </div>
            </div>
          </div>
        </header>
      </div>

      <section class="mb-10 grid gap-5 md:grid-cols-3">
        <article
          class="reveal-step-2 rounded-2xl border border-[var(--bg-300)] bg-white p-5 shadow-sm transition duration-300 hover:-translate-y-1 hover:shadow-lg"
        >
          <p class="text-xs font-semibold uppercase tracking-[0.16em] text-[var(--primary-100)]">
            Anios experiencia
          </p>
          <p class="mt-3 text-3xl font-black text-[var(--accent-200)]">+4</p>
          <p class="mt-2 text-sm text-[var(--text-200)]">
            Construyendo productos y sistemas reales en produccion.
          </p>
        </article>
        <article
          class="reveal-step-2 rounded-2xl border border-[var(--bg-300)] bg-white p-5 shadow-sm transition duration-300 hover:-translate-y-1 hover:shadow-lg"
        >
          <p class="text-xs font-semibold uppercase tracking-[0.16em] text-[var(--primary-100)]">
            Entrega
          </p>
          <p class="mt-3 text-3xl font-black text-[var(--accent-200)]">1-3 semanas</p>
          <p class="mt-2 text-sm text-[var(--text-200)]">
            Desarrollo rapido sin comprometer estabilidad ni calidad.
          </p>
        </article>
        <article
          class="reveal-step-2 rounded-2xl border border-[var(--bg-300)] bg-white p-5 shadow-sm transition duration-300 hover:-translate-y-1 hover:shadow-lg"
        >
          <p class="text-xs font-semibold uppercase tracking-[0.16em] text-[var(--primary-100)]">
            Especialidad
          </p>
          <p class="mt-3 text-3xl font-black text-[var(--accent-200)]">Full Stack</p>
          <p class="mt-2 text-sm text-[var(--text-200)]">
            Arquitectura, permisos, pagos e integraciones inteligentes.
          </p>
        </article>
      </section>

      <section
        class="reveal-step-3 mb-10 rounded-3xl border border-[var(--primary-200)]/40 bg-white p-6 shadow-sm md:p-8"
      >
        <h2 class="text-2xl font-black text-[var(--accent-200)] md:text-3xl">
          Experiencia profesional
        </h2>
        <div class="mt-6 rounded-2xl bg-[var(--bg-200)] p-5">
          <p class="text-xs font-semibold uppercase tracking-[0.16em] text-[var(--primary-100)]">
            2021 - Presente
          </p>
          <h3 class="mt-2 text-xl font-extrabold text-[var(--text-100)]">
            Desarrollador Full Stack Senior - Freelance
          </h3>
          <ul class="mt-4 space-y-3 text-sm leading-relaxed text-[var(--text-200)] sm:text-base">
            <li class="flex items-start gap-2">
              <span
                class="mt-1.5 inline-block h-2 w-2 shrink-0 rounded-full bg-[var(--primary-100)]"
              ></span
              >Desarrollo de aplicaciones web completas desde cero hasta produccion.
            </li>
            <li class="flex items-start gap-2">
              <span
                class="mt-1.5 inline-block h-2 w-2 shrink-0 rounded-full bg-[var(--primary-100)]"
              ></span
              >Diseno de arquitectura escalable en frontend y backend.
            </li>
            <li class="flex items-start gap-2">
              <span
                class="mt-1.5 inline-block h-2 w-2 shrink-0 rounded-full bg-[var(--primary-100)]"
              ></span
              >Sistemas con multiples roles, autenticacion, autorizacion y control de permisos.
            </li>
            <li class="flex items-start gap-2">
              <span
                class="mt-1.5 inline-block h-2 w-2 shrink-0 rounded-full bg-[var(--primary-100)]"
              ></span
              >Integracion de pasarelas de pago con Stripe.
            </li>
            <li class="flex items-start gap-2">
              <span
                class="mt-1.5 inline-block h-2 w-2 shrink-0 rounded-full bg-[var(--primary-100)]"
              ></span
              >Despliegue en Linux VPS, configuracion de dominios y entornos productivos.
            </li>
            <li class="flex items-start gap-2">
              <span
                class="mt-1.5 inline-block h-2 w-2 shrink-0 rounded-full bg-[var(--primary-100)]"
              ></span
              >Optimizacion SEO y mejora de rendimiento web.
            </li>
            <li class="flex items-start gap-2">
              <span
                class="mt-1.5 inline-block h-2 w-2 shrink-0 rounded-full bg-[var(--primary-100)]"
              ></span
              >Sistemas activos en uso por clientes reales.
            </li>
          </ul>
        </div>
      </section>

      <section class="mb-10 grid gap-6 lg:grid-cols-[1.2fr_1fr]">
        <article
          class="reveal-step-4 rounded-3xl border border-[var(--bg-300)] bg-white p-6 md:p-8"
        >
          <h2 class="text-2xl font-black text-[var(--accent-200)] md:text-3xl">
            Proyectos publicos destacados
          </h2>
          <div class="mt-6 space-y-4">
            <a
              href="https://pin-tin-tin.com"
              target="_blank"
              rel="noopener noreferrer"
              class="group block rounded-2xl border border-[var(--primary-200)]/30 bg-[var(--bg-200)] p-4 transition hover:border-[var(--primary-100)]"
            >
              <p
                class="text-sm font-bold text-[var(--primary-100)] group-hover:text-[var(--accent-200)]"
              >
                pin-tin-tin.com
              </p>
              <p class="mt-1 text-sm text-[var(--text-200)]">
                Juego de domino online multijugador con pagos y autenticacion.
              </p>
              <span
                class="mt-2 inline-flex items-center gap-1 text-xs font-semibold text-[var(--accent-100)] opacity-0 transition group-hover:opacity-100"
                >Visitar sitio <span class="text-base leading-none">&nearr;</span></span
              >
            </a>
            <a
              href="https://refrigeracionroberto.com"
              target="_blank"
              rel="noopener noreferrer"
              class="group block rounded-2xl border border-[var(--primary-200)]/30 bg-[var(--bg-200)] p-4 transition hover:border-[var(--primary-100)]"
            >
              <p
                class="text-sm font-bold text-[var(--primary-100)] group-hover:text-[var(--accent-200)]"
              >
                refrigeracionroberto.com
              </p>
              <p class="mt-1 text-sm text-[var(--text-200)]">
                Taller de refrigeracion y aire acondicionado con enfoque comercial y SEO local.
              </p>
              <span
                class="mt-2 inline-flex items-center gap-1 text-xs font-semibold text-[var(--accent-100)] opacity-0 transition group-hover:opacity-100"
                >Visitar sitio <span class="text-base leading-none">&nearr;</span></span
              >
            </a>
            <a
              href="https://bbtito.com"
              target="_blank"
              rel="noopener noreferrer"
              class="group block rounded-2xl border border-[var(--primary-200)]/30 bg-[var(--bg-200)] p-4 transition hover:border-[var(--primary-100)]"
            >
              <p
                class="text-sm font-bold text-[var(--primary-100)] group-hover:text-[var(--accent-200)]"
              >
                bbtito.com
              </p>
              <p class="mt-1 text-sm text-[var(--text-200)]">
                Tienda de moda con experiencia ecommerce fluida.
              </p>
              <span
                class="mt-2 inline-flex items-center gap-1 text-xs font-semibold text-[var(--accent-100)] opacity-0 transition group-hover:opacity-100"
                >Visitar sitio <span class="text-base leading-none">&nearr;</span></span
              >
            </a>
          </div>
        </article>

        <article
          class="reveal-step-5 rounded-3xl border border-[var(--bg-300)] bg-white p-6 md:p-8"
        >
          <h2 class="text-2xl font-black text-[var(--accent-200)]">Tecnologias</h2>
          <p class="mt-2 text-sm text-[var(--text-200)]">
            Cada icono te lleva al sitio oficial de la tecnologia.
          </p>
          <div class="mt-5 grid grid-cols-1 gap-3 text-sm sm:grid-cols-2">
            <a
              v-for="tech in techStack"
              :key="tech.name"
              :href="tech.site"
              target="_blank"
              rel="noopener noreferrer"
              class="group flex items-center gap-3 rounded-xl border border-[var(--primary-200)]/30 bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)] transition duration-300 hover:-translate-y-0.5 hover:border-[var(--primary-100)] hover:bg-white"
            >
              <img
                :src="tech.icon"
                :alt="`Icono oficial de ${tech.name}`"
                class="h-5 w-5"
                loading="lazy"
              />
              <span>{{ tech.name }}</span>
              <span
                class="ml-auto text-xs text-[var(--primary-100)] opacity-0 transition group-hover:opacity-100"
              >
                Oficial
              </span>
            </a>
          </div>
        </article>
      </section>

      <section
        class="reveal-step-6 mb-10 rounded-3xl border border-[var(--primary-200)]/40 bg-gradient-to-r from-[var(--primary-300)]/45 to-white p-6 md:p-8"
      >
        <h2 class="text-2xl font-black text-[var(--accent-200)] md:text-3xl">
          Formacion y enfoque
        </h2>
        <p class="mt-4 text-sm leading-relaxed text-[var(--text-200)] sm:text-base">
          Ingeniero Informatico por la Universidad de las Ciencias Informaticas de La Habana (UCI),
          2018-2023. Enfocado en construir software estable, mantenible y orientado a resultados de
          negocio, con especial interes en arquitectura de sistemas, desarrollo de APIs,
          inteligencia artificial aplicada y mejora continua.
        </p>
      </section>

      <footer class="reveal-step-6 pb-8 text-center text-sm text-[var(--text-200)]">
        <div
          class="mx-auto mb-5 h-px w-24 bg-gradient-to-r from-transparent via-[var(--primary-200)] to-transparent"
        ></div>
        <p>Disponible para proyectos freelance y colaboraciones remotas.</p>
        <p class="mt-1 font-semibold text-[var(--primary-100)]">
          <a
            href="https://github.com/Rodolf-GitHub"
            target="_blank"
            rel="noopener noreferrer"
            class="transition hover:text-[var(--accent-200)]"
            >github.com/Rodolf-GitHub</a
          >
        </p>
      </footer>
    </div>

    <a
      href="https://wa.me/59891854199?text=Hola%20Rodolfo%2C%20vi%20tu%20portafolio%20y%20quiero%20consultarte%20por%20un%20proyecto."
      target="_blank"
      rel="noopener noreferrer"
      aria-label="Contactar por WhatsApp"
      class="whatsapp-float fixed right-5 bottom-5 z-50 inline-flex h-14 w-14 items-center justify-center gap-0 rounded-full bg-[#25D366] p-0 text-sm font-bold text-white shadow-2xl transition hover:scale-105 hover:bg-[#1ea952] sm:right-8 sm:bottom-8 sm:h-auto sm:w-auto sm:gap-2 sm:px-4 sm:py-3"
    >
      <img
        src="https://cdn.simpleicons.org/whatsapp/ffffff"
        alt="WhatsApp"
        class="h-5 w-5"
        loading="lazy"
      />
      <span class="hidden sm:inline">WhatsApp</span>
    </a>
  </main>
</template>

<style scoped>
/* ── INTRO SPLASH ── */
.intro-overlay {
  overflow: hidden;
}

.intro-logo {
  opacity: 0;
  animation: introZoomIn 0.8s cubic-bezier(0.16, 1, 0.3, 1) 0.2s forwards;
}

.intro-tagline {
  opacity: 0;
  animation: introSlideUp 0.6s ease-out 0.7s forwards;
}

.intro-bar {
  opacity: 0;
  animation: introExpand 0.5s ease-out 1.1s forwards;
}

.intro-fade-leave-active {
  transition: opacity 0.6s ease-out;
}

.intro-fade-leave-to {
  opacity: 0;
}

@keyframes introZoomIn {
  from {
    opacity: 0;
    transform: scale(0.6);
    letter-spacing: 0.3em;
  }

  to {
    opacity: 1;
    transform: scale(1);
    letter-spacing: -0.02em;
  }
}

@keyframes introSlideUp {
  from {
    opacity: 0;
    transform: translateY(14px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes introExpand {
  from {
    opacity: 0;
    width: 0;
  }

  to {
    opacity: 1;
    width: 5rem;
  }
}

/* ── NAME SHIMMER ── */
.name-shimmer {
  background: linear-gradient(
    90deg,
    var(--accent-200) 0%,
    var(--primary-100) 40%,
    var(--accent-100) 60%,
    var(--accent-200) 100%
  );
  background-size: 200% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shimmer 4s linear infinite;
}

@keyframes shimmer {
  to {
    background-position: 200% center;
  }
}

/* ── GLOW BORDER ── */
.glow-border-wrap {
  background: var(--bg-200);
  overflow: hidden;
}

.glow-border-wrap::before {
  content: '';
  position: absolute;
  inset: -80%;
  background: conic-gradient(
    from 0deg,
    transparent 0%,
    transparent 30%,
    var(--accent-100) 38%,
    var(--primary-200) 42%,
    var(--primary-300) 50%,
    var(--primary-200) 58%,
    var(--accent-100) 62%,
    transparent 70%,
    transparent 100%
  );
  animation: borderSpin 6s linear infinite;
  z-index: 0;
}

.glow-border-wrap > header {
  position: relative;
  z-index: 1;
}

@keyframes borderSpin {
  to {
    transform: rotate(360deg);
  }
}

/* ── REVEAL STEPS ── */
.reveal-step-1,
.reveal-step-2,
.reveal-step-3,
.reveal-step-4,
.reveal-step-5,
.reveal-step-6 {
  opacity: 0;
  animation: fadeUp 0.75s ease-out forwards;
}

.reveal-step-2 {
  animation-delay: 0.08s;
}

.reveal-step-3 {
  animation-delay: 0.14s;
}

.reveal-step-4 {
  animation-delay: 0.2s;
}

.reveal-step-5 {
  animation-delay: 0.26s;
}

.reveal-step-6 {
  animation-delay: 0.32s;
}

.floating-aura {
  animation: drift 12s ease-in-out infinite;
}

.floating-aura-delayed {
  animation: drift 15s ease-in-out infinite reverse;
}

.floating-aura-slow {
  animation: drift 18s ease-in-out infinite;
}

.whatsapp-float {
  animation: pulseSoft 2.2s ease-in-out infinite;
}

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

@keyframes drift {
  0%,
  100% {
    transform: translate3d(0, 0, 0) scale(1);
  }

  50% {
    transform: translate3d(0, -12px, 0) scale(1.03);
  }
}

@keyframes pulseSoft {
  0%,
  100% {
    box-shadow: 0 10px 30px -14px rgba(37, 211, 102, 0.85);
  }

  50% {
    box-shadow: 0 14px 36px -12px rgba(37, 211, 102, 0.95);
  }
}

@media (prefers-reduced-motion: reduce) {
  .reveal-step-1,
  .reveal-step-2,
  .reveal-step-3,
  .reveal-step-4,
  .reveal-step-5,
  .reveal-step-6,
  .floating-aura,
  .floating-aura-delayed,
  .floating-aura-slow,
  .whatsapp-float,
  .intro-logo,
  .intro-tagline,
  .intro-bar,
  .name-shimmer,
  .glow-border-wrap::before {
    animation: none;
    opacity: 1;
    transform: none;
  }

  .name-shimmer {
    -webkit-text-fill-color: var(--accent-200);
  }

  .glow-border-wrap::before {
    display: none;
  }
}
</style>
