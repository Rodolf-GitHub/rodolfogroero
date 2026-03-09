<template>
  <main class="relative overflow-hidden bg-[var(--bg-200)] text-[var(--text-100)]">
    <div class="pointer-events-none absolute inset-0">
      <div
        class="absolute -top-32 -left-24 h-96 w-96 rounded-full bg-[var(--primary-300)] blur-3xl opacity-70"
      ></div>
      <div
        class="absolute top-1/3 -right-20 h-80 w-80 rounded-full bg-[var(--primary-200)] blur-3xl opacity-35"
      ></div>
      <div
        class="absolute bottom-0 left-1/3 h-72 w-72 rounded-full bg-[var(--accent-100)] blur-3xl opacity-20"
      ></div>
    </div>

    <div class="relative mx-auto max-w-6xl px-6 py-10 sm:px-8 lg:px-10">
      <header
        class="mb-14 rounded-3xl border border-[var(--primary-200)]/35 bg-white/85 p-6 shadow-[0_20px_60px_-35px_var(--accent-200)] backdrop-blur md:p-10"
      >
        <div class="grid gap-8 md:grid-cols-[1.5fr_1fr] md:items-center">
          <div>
            <p
              class="inline-flex rounded-full border border-[var(--primary-200)] bg-[var(--primary-300)]/60 px-4 py-1 text-xs font-semibold uppercase tracking-[0.18em] text-[var(--accent-200)]"
            >
              Montevideo, Uruguay · Remoto
            </p>
            <h1
              class="mt-5 text-4xl font-black leading-tight text-[var(--accent-200)] sm:text-5xl md:text-6xl"
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
              class="relative rounded-3xl bg-gradient-to-br from-[var(--primary-200)] via-[var(--accent-100)] to-[var(--accent-200)] p-[3px] shadow-2xl shadow-[var(--accent-200)]/20"
            >
              <img
                src="/foto_rodolfo.jpg"
                alt="Rodolfo Groero"
                class="aspect-[4/5] w-full rounded-[22px] object-cover"
                loading="eager"
              />
            </div>
          </div>
        </div>
      </header>

      <section class="mb-10 grid gap-5 md:grid-cols-3">
        <article class="rounded-2xl border border-[var(--bg-300)] bg-white p-5 shadow-sm">
          <p class="text-xs font-semibold uppercase tracking-[0.16em] text-[var(--primary-100)]">
            Anios experiencia
          </p>
          <p class="mt-3 text-3xl font-black text-[var(--accent-200)]">+4</p>
          <p class="mt-2 text-sm text-[var(--text-200)]">
            Construyendo productos y sistemas reales en produccion.
          </p>
        </article>
        <article class="rounded-2xl border border-[var(--bg-300)] bg-white p-5 shadow-sm">
          <p class="text-xs font-semibold uppercase tracking-[0.16em] text-[var(--primary-100)]">
            Entrega
          </p>
          <p class="mt-3 text-3xl font-black text-[var(--accent-200)]">1-3 semanas</p>
          <p class="mt-2 text-sm text-[var(--text-200)]">
            Desarrollo rapido sin comprometer estabilidad ni calidad.
          </p>
        </article>
        <article class="rounded-2xl border border-[var(--bg-300)] bg-white p-5 shadow-sm">
          <p class="text-xs font-semibold uppercase tracking-[0.16em] text-[var(--primary-100)]">
            Especialidad
          </p>
          <p class="mt-3 text-3xl font-black text-[var(--accent-200)]">Full Stack + IA</p>
          <p class="mt-2 text-sm text-[var(--text-200)]">
            Arquitectura, permisos, pagos e integraciones inteligentes.
          </p>
        </article>
      </section>

      <section
        class="mb-10 rounded-3xl border border-[var(--primary-200)]/40 bg-white p-6 shadow-sm md:p-8"
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
          <ul class="mt-4 space-y-2 text-sm leading-relaxed text-[var(--text-200)] sm:text-base">
            <li>Desarrollo de aplicaciones web completas desde cero hasta produccion.</li>
            <li>Diseno de arquitectura escalable en frontend y backend.</li>
            <li>
              Sistemas con multiples roles, autenticacion, autorizacion y control de permisos.
            </li>
            <li>Integracion de pasarelas de pago con Stripe.</li>
            <li>Despliegue en Linux VPS, configuracion de dominios y entornos productivos.</li>
            <li>Optimizacion SEO y mejora de rendimiento web.</li>
            <li>Sistemas activos en uso por clientes reales.</li>
          </ul>
        </div>
      </section>

      <section class="mb-10 grid gap-6 lg:grid-cols-[1.2fr_1fr]">
        <article class="rounded-3xl border border-[var(--bg-300)] bg-white p-6 md:p-8">
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
                Sitio comercial optimizado para conversion y presencia online.
              </p>
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
            </a>
          </div>
        </article>

        <article class="rounded-3xl border border-[var(--bg-300)] bg-white p-6 md:p-8">
          <h2 class="text-2xl font-black text-[var(--accent-200)]">Tecnologias</h2>
          <div class="mt-5 grid grid-cols-2 gap-3 text-sm">
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Vue.js</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Nuxt</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >React</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Tailwind CSS</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >FastAPI</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Django</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Node.js</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >PostgreSQL</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Linux & VPS</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Nginx</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >Stripe</span
            >
            <span
              class="rounded-xl bg-[var(--bg-200)] px-3 py-2 font-semibold text-[var(--text-100)]"
              >SEO tecnico</span
            >
          </div>
        </article>
      </section>

      <section
        class="mb-10 rounded-3xl border border-[var(--primary-200)]/40 bg-gradient-to-r from-[var(--primary-300)]/45 to-white p-6 md:p-8"
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

      <footer class="pb-8 text-center text-sm text-[var(--text-200)]">
        <p>Disponible para proyectos freelance y colaboraciones remotas.</p>
        <p class="mt-1 font-semibold text-[var(--primary-100)]">GitHub: github.com/Rodolf-GitHub</p>
      </footer>
    </div>
  </main>
</template>
