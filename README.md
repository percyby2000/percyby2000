export default function SeniorDeveloperPortfolio() {
  const skills = [
    'Astro',
    'React',
    'Next.js',
    'Tailwind CSS',
    'Spring Boot',
    'Java',
    'Kotlin',
    'SQL Server',
    'Supabase',
    'Docker',
    'IA & Automatización'
  ];

  const projects = [
    {
      title: 'Sistema SaaS Hotelero',
      description:
        'Plataforma moderna para hoteles con reservas, dashboard administrativo, reportes y analíticas en tiempo real.',
      stack: 'React • Spring Boot • PostgreSQL • Docker'
    },
    {
      title: 'Radio Cristiana Online',
      description:
        'Aplicación web responsive para streaming en vivo con diseño glassmorphism y reproductor avanzado.',
      stack: 'Astro • Tailwind • JavaScript'
    },
    {
      title: 'Generador Inteligente de Horarios',
      description:
        'Sistema académico con IA para optimizar horarios universitarios utilizando algoritmos avanzados.',
      stack: 'Next.js • Spring Boot • SQL Server'
    }
  ];

  return (
    <main className="min-h-screen bg-black text-white overflow-hidden">
      <div className="absolute inset-0 bg-[radial-gradient(circle_at_top,rgba(0,255,180,0.15),transparent_40%)]"></div>

      <section className="relative z-10 max-w-7xl mx-auto px-6 py-16">
        <nav className="flex items-center justify-between mb-20">
          <h1 className="text-2xl md:text-3xl font-bold tracking-widest uppercase">
            Percy Dev
          </h1>

          <div className="hidden md:flex gap-8 text-sm text-zinc-300">
            <a href="#about" className="hover:text-white transition">Sobre mí</a>
            <a href="#projects" className="hover:text-white transition">Proyectos</a>
            <a href="#skills" className="hover:text-white transition">Skills</a>
            <a href="#contact" className="hover:text-white transition">Contacto</a>
          </div>
        </nav>

        <div className="grid lg:grid-cols-2 gap-16 items-center min-h-[75vh]">
          <div>
            <span className="inline-flex items-center gap-2 border border-emerald-400/40 bg-emerald-500/10 px-4 py-2 rounded-full text-sm text-emerald-300 mb-6">
              ● Senior Full Stack Developer
            </span>

            <h2 className="text-5xl md:text-7xl font-black leading-tight mb-8">
              Construyo
              <span className="block text-transparent bg-clip-text bg-gradient-to-r from-emerald-400 to-cyan-400">
                experiencias digitales
              </span>
              modernas.
            </h2>

            <p className="text-zinc-400 text-lg leading-relaxed max-w-xl mb-10">
              Ingeniero de sistemas apasionado por crear aplicaciones modernas,
              escalables y visualmente impactantes. Especializado en frontend
              avanzado, backend robusto e integración con inteligencia artificial.
            </p>

            <div className="flex flex-wrap gap-4">
              <a
                href="https://github.com"
                className="px-7 py-4 rounded-2xl bg-white text-black font-semibold hover:scale-105 transition-transform"
              >
                Ver GitHub
              </a>

              <a
                href="#projects"
                className="px-7 py-4 rounded-2xl border border-zinc-700 hover:border-emerald-400 transition"
              >
                Explorar proyectos
              </a>
            </div>
          </div>

          <div className="relative">
            <div className="absolute -inset-8 bg-gradient-to-r from-emerald-500/20 to-cyan-500/20 blur-3xl rounded-full"></div>

            <div className="relative backdrop-blur-xl border border-white/10 bg-white/5 rounded-[2rem] p-8 shadow-2xl">
              <div className="flex items-center gap-3 mb-8">
                <div className="w-3 h-3 rounded-full bg-red-400"></div>
                <div className="w-3 h-3 rounded-full bg-yellow-400"></div>
                <div className="w-3 h-3 rounded-full bg-green-400"></div>
              </div>

              <pre className="text-sm md:text-base overflow-auto text-zinc-300 leading-8">
{`const developer = {
  name: 'Percy Conde',
  role: 'Senior Full Stack Developer',
  stack: ['React', 'Astro', 'Next.js'],
  backend: ['Spring Boot', 'Java'],
  passion: 'Building futuristic apps',
  status: 'Available for projects'
}`}
              </pre>
            </div>
          </div>
        </div>
      </section>

      <section
        id="about"
        className="relative z-10 max-w-6xl mx-auto px-6 py-24"
      >
        <div className="grid md:grid-cols-2 gap-10">
          <div className="bg-white/5 border border-white/10 rounded-3xl p-10 backdrop-blur-xl">
            <h3 className="text-3xl font-bold mb-6">Sobre mí</h3>
            <p className="text-zinc-400 leading-relaxed text-lg">
              Desarrollo aplicaciones web modernas con arquitecturas limpias,
              interfaces premium y experiencias rápidas. Me especializo en
              crear sistemas empresariales, plataformas SaaS y soluciones
              digitales escalables.
            </p>
          </div>

          <div className="bg-gradient-to-br from-emerald-500/10 to-cyan-500/10 border border-emerald-400/20 rounded-3xl p-10">
            <h3 className="text-3xl font-bold mb-6">Experiencia</h3>

            <div className="space-y-6 text-zinc-300">
              <div>
                <p className="font-semibold text-white">Frontend Architecture</p>
                <p className="text-zinc-400">
                  Diseño de interfaces modernas, animaciones avanzadas y UX premium.
                </p>
              </div>

              <div>
                <p className="font-semibold text-white">Backend Engineering</p>
                <p className="text-zinc-400">
                  APIs REST robustas con Spring Boot, seguridad y bases de datos.
                </p>
              </div>

              <div>
                <p className="font-semibold text-white">AI Integration</p>
                <p className="text-zinc-400">
                  Integración de inteligencia artificial en sistemas modernos.
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section
        id="projects"
        className="relative z-10 max-w-7xl mx-auto px-6 py-24"
      >
        <div className="flex items-center justify-between mb-14">
          <div>
            <p className="text-emerald-400 uppercase tracking-[0.3em] text-sm mb-3">
              Portfolio
            </p>
            <h3 className="text-5xl font-black">Proyectos destacados</h3>
          </div>
        </div>

        <div className="grid lg:grid-cols-3 gap-8">
          {projects.map((project, index) => (
            <div
              key={index}
              className="group bg-white/5 border border-white/10 rounded-[2rem] p-8 hover:-translate-y-2 transition-all duration-300 hover:border-emerald-400/30"
            >
              <div className="h-52 rounded-3xl bg-gradient-to-br from-zinc-900 to-zinc-800 mb-8 flex items-center justify-center border border-white/5">
                <span className="text-6xl">🚀</span>
              </div>

              <h4 className="text-2xl font-bold mb-4">{project.title}</h4>

              <p className="text-zinc-400 leading-relaxed mb-6">
                {project.description}
              </p>

              <div className="flex items-center justify-between">
                <span className="text-sm text-emerald-300">
                  {project.stack}
                </span>

                <button className="text-white hover:text-emerald-400 transition">
                  →
                </button>
              </div>
            </div>
          ))}
        </div>
      </section>

      <section
        id="skills"
        className="relative z-10 max-w-6xl mx-auto px-6 py-24"
      >
        <div className="text-center mb-14">
          <p className="text-emerald-400 uppercase tracking-[0.3em] text-sm mb-4">
            Tech Stack
          </p>
          <h3 className="text-5xl font-black">Tecnologías</h3>
        </div>

        <div className="flex flex-wrap justify-center gap-5">
          {skills.map((skill, index) => (
            <div
              key={index}
              className="px-7 py-4 rounded-2xl border border-white/10 bg-white/5 backdrop-blur-lg hover:border-emerald-400/40 hover:scale-105 transition"
            >
              {skill}
            </div>
          ))}
        </div>
      </section>

      <section
        id="contact"
        className="relative z-10 max-w-5xl mx-auto px-6 py-24"
      >
        <div className="rounded-[3rem] border border-white/10 bg-gradient-to-br from-white/5 to-white/[0.02] p-14 text-center backdrop-blur-2xl">
          <p className="text-emerald-400 uppercase tracking-[0.3em] text-sm mb-4">
            Contacto
          </p>

          <h3 className="text-5xl font-black mb-8">
            ¿Tienes un proyecto en mente?
          </h3>

          <p className="text-zinc-400 text-lg max-w-2xl mx-auto mb-10 leading-relaxed">
            Estoy disponible para colaborar en proyectos web modernos,
            plataformas SaaS, aplicaciones empresariales y soluciones impulsadas por IA.
          </p>

          <div className="flex flex-wrap justify-center gap-5">
            <a
              href="mailto:contacto@dev.com"
              className="px-8 py-4 rounded-2xl bg-white text-black font-semibold hover:scale-105 transition-transform"
            >
              Contactarme
            </a>

            <a
              href="https://github.com"
              className="px-8 py-4 rounded-2xl border border-zinc-700 hover:border-emerald-400 transition"
            >
              GitHub
            </a>
          </div>
        </div>
      </section>
    </main>
  );
}
