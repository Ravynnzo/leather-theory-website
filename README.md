# leather-theory-website
Add file → Upload files
export default function LeatherCleaningWebsite() { const services = [ { title: 'Deep Cleaning', text: 'Remove dirt, oils, and buildup without drying or cracking leather.', icon: '🧼', }, { title: 'Stain Removal', text: 'Target tough stains and discoloration with safe restoration methods.', icon: '✨', }, { title: 'Conditioning', text: 'Keep leather soft, rich, and protected against future wear.', icon: '🛡️', }, { title: 'Interior Detailing', text: 'Luxury treatment for leather car seats and vehicle interiors.', icon: '🚘', }, ];

const reviews = [ { name: 'Amanda R.', text: 'My leather couch looked brand new again. Super professional and easy to work with.', }, { name: 'Marcus T.', text: 'The car interior cleanup was incredible. You can tell they actually care about quality.', }, { name: 'Jasmine L.', text: 'Fast service, great communication, and the results honestly shocked me.', }, ];

const gallery = [ 'https://images.unsplash.com/photo-1505693416388-ac5ce068fe85?q=80&w=1200&auto=format&fit=crop', 'https://images.unsplash.com/photo-1555041469-a586c61ea9bc?q=80&w=1200&auto=format&fit=crop', 'https://images.unsplash.com/photo-1493666438817-866a91353ca9?q=80&w=1200&auto=format&fit=crop', 'https://images.unsplash.com/photo-1513694203232-719a280e022f?q=80&w=1200&auto=format&fit=crop', ];

return ( <div className="min-h-screen bg-[#120d09] text-white font-sans overflow-hidden selection:bg-amber-400 selection:text-black"> {/* Floating Buttons */} <div className="fixed bottom-5 right-5 z-50 flex flex-col gap-3"> <button className="bg-green-500 text-white px-6 py-4 rounded-2xl font-bold shadow-2xl hover:scale-105 transition-transform"> 📱 Text For Instant Quote </button>

<button className="bg-amber-400 text-black px-6 py-4 rounded-2xl font-black shadow-2xl hover:scale-105 transition-transform">
      ⚡ Same-Day Estimates
    </button>
  </div>

  {/* Hero */}
  <section className="relative overflow-hidden border-b border-white/10">
    <div className="absolute inset-0 bg-gradient-to-br from-amber-900/30 via-[#120d09] to-black"></div>

    <div className="relative max-w-7xl mx-auto px-6 py-24 lg:py-32 grid lg:grid-cols-2 gap-14 items-center">
      <div>
        <div className="inline-flex items-center gap-2 bg-white/10 border border-white/10 px-4 py-2 rounded-full text-sm mb-6 backdrop-blur-sm">
          ✨ PREMIUM LEATHER RESTORATION
        </div>

        <h1 className="text-6xl lg:text-8xl font-black leading-[0.95] tracking-tight uppercase">
          Bring Your
          <span className="block text-amber-400">Leather Back</span>
          To Life.
        </h1>

        <p className="mt-8 text-lg text-stone-300 max-w-xl leading-relaxed">
          Deep cleaning, stain removal, conditioning, and restoration for couches, car interiors, jackets, bags, and more.
        </p>

        <div className="mt-10 flex flex-wrap gap-4">
          <button className="bg-amber-400 hover:bg-amber-300 text-black font-bold px-7 py-4 rounded-2xl transition-all shadow-2xl shadow-amber-500/20">
            Book Cleaning
          </button>

          <button className="border border-white/20 hover:border-white/50 bg-white/5 px-7 py-4 rounded-2xl transition-all">
            View Services
          </button>
        </div>

        <div className="mt-12 grid grid-cols-3 gap-6 text-center">
          <div>
            <h3 className="text-3xl font-black text-amber-400">500+</h3>
            <p className="text-stone-400 text-sm mt-1">Items Restored</p>
          </div>

          <div>
            <h3 className="text-3xl font-black text-amber-400">4.9★</h3>
            <p className="text-stone-400 text-sm mt-1">Customer Rating</p>
          </div>

          <div>
            <h3 className="text-3xl font-black text-amber-400">100%</h3>
            <p className="text-stone-400 text-sm mt-1">Satisfaction</p>
          </div>
        </div>
      </div>

      <div className="relative">
        <div className="absolute -inset-4 bg-amber-500/20 blur-3xl rounded-full"></div>

        <img
          src="https://images.unsplash.com/photo-1505693416388-ac5ce068fe85?q=80&w=1200&auto=format&fit=crop"
          alt="Luxury leather couch"
          className="relative rounded-[32px] shadow-2xl border border-white/10 object-cover h-[650px] w-full"
        />
      </div>
    </div>
  </section>

  {/* Services */}
  <section className="max-w-7xl mx-auto px-6 py-24">
    <div className="text-center max-w-3xl mx-auto">
      <p className="text-amber-400 font-semibold uppercase tracking-[0.3em] text-sm">
        What We Do
      </p>

      <h2 className="mt-4 text-4xl lg:text-6xl font-black">
        Serious Results. Clean Style.
      </h2>
    </div>

    <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6 mt-16">
      {services.map((service) => (
        <div
          key={service.title}
          className="bg-white/5 border border-white/10 backdrop-blur-sm rounded-3xl p-8 hover:-translate-y-2 transition-all duration-300 hover:border-amber-400/30"
        >
          <div className="text-5xl mb-5">{service.icon}</div>
          <h3 className="text-2xl font-bold mb-4">{service.title}</h3>
          <p className="text-stone-400 leading-relaxed">{service.text}</p>
        </div>
      ))}
    </div>
  </section>

  {/* Instagram Gallery */}
  <section className="max-w-7xl mx-auto px-6 py-24 border-y border-white/10">
    <div className="flex flex-wrap items-center justify-between gap-6">
      <div>
        <p className="text-amber-400 uppercase tracking-[0.3em] text-sm font-semibold">
          Instagram Results
        </p>

        <h2 className="mt-4 text-4xl lg:text-5xl font-black">
          Clean Leather Looks Better.
        </h2>
      </div>

      <button className="border border-white/10 bg-white/5 px-6 py-4 rounded-2xl hover:bg-white/10 transition-all">
        Follow @FreshLeatherCare
      </button>
    </div>

    <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-5 mt-14">
      {gallery.map((img, index) => (
        <img
          key={index}
          src={img}
          alt="Leather cleaning showcase"
          className="rounded-3xl h-[320px] w-full object-cover border border-white/10 hover:scale-[1.02] transition-transform"
        />
      ))}
    </div>
  </section>

  {/* Booking Form */}
  <section className="bg-stone-900 py-24 border-y border-white/10">
    <div className="max-w-6xl mx-auto px-6 grid lg:grid-cols-2 gap-14 items-center">
      <div>
        <p className="text-amber-400 uppercase tracking-[0.3em] text-sm font-semibold">
          Fast Booking
        </p>

        <h2 className="mt-4 text-5xl lg:text-6xl font-black leading-tight">
          Get Your Free Quote
          <span className="block text-amber-400">In Minutes.</span>
        </h2>

        <p className="mt-6 text-stone-400 text-lg leading-relaxed">
          Send photos of your leather item or interior and get a same-day estimate.
        </p>
      </div>

      <div className="bg-white/5 border border-white/10 rounded-[32px] p-8 backdrop-blur-sm space-y-5">
        <input type="text" placeholder="Full Name" className="w-full bg-black/30 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-amber-400" />
        <input type="text" placeholder="Phone Number" className="w-full bg-black/30 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-amber-400" />
        <input type="email" placeholder="Email Address" className="w-full bg-black/30 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-amber-400" />
        <textarea rows={5} placeholder="Tell us about your leather item..." className="w-full bg-black/30 border border-white/10 rounded-2xl px-5 py-4 outline-none focus:border-amber-400"></textarea>

        <button className="w-full bg-amber-400 text-black py-5 rounded-2xl font-black uppercase tracking-wide hover:scale-[1.02] transition-transform">
          Request Free Quote
        </button>
      </div>
    </div>
  </section>

  {/* Testimonials */}
  <section className="max-w-7xl mx-auto px-6 py-24">
    <div className="text-center">
      <p className="text-amber-400 uppercase tracking-[0.3em] text-sm font-semibold">
        Customer Reviews
      </p>

      <h2 className="mt-4 text-4xl lg:text-5xl font-black">
        Trusted By Leather Lovers
      </h2>
    </div>

    <div className="grid lg:grid-cols-3 gap-6 mt-16">
      {reviews.map((review) => (
        <div
          key={review.name}
          className="bg-white/5 border border-white/10 rounded-3xl p-8"
        >
          <div className="text-amber-400 text-2xl mb-4">★★★★★</div>
          <p className="text-stone-300 leading-relaxed text-lg">“{review.text}”</p>
          <p className="mt-6 font-bold">{review.name}</p>
        </div>
      ))}
    </div>
  </section>

  {/* Service Areas */}
  <section className="max-w-7xl mx-auto px-6 py-24 border-t border-white/10">
    <div className="grid lg:grid-cols-2 gap-12 items-center">
      <div>
        <p className="text-amber-400 uppercase tracking-[0.3em] text-sm font-semibold">
          Service Areas
        </p>

        <h2 className="mt-4 text-5xl font-black leading-tight">
          Local Leather Cleaning Experts
        </h2>

        <p className="mt-6 text-stone-400 text-lg leading-relaxed">
          Premium leather cleaning and restoration services for homes, offices, vehicles, and luxury furniture.
        </p>

        <div className="mt-8 flex flex-wrap gap-3">
          {['Watertown', 'Syracuse', 'Carthage', 'Fort Drum', 'Lowville'].map((city) => (
            <div key={city} className="bg-white/5 border border-white/10 rounded-full px-5 py-3 text-sm">
              {city}
            </div>
          ))}
        </div>
      </div>

      <div className="bg-gradient-to-r from-amber-500 to-yellow-300 rounded-[40px] p-12 text-black shadow-2xl">
        <p className="uppercase tracking-[0.3em] text-sm font-bold">
          Ready To Refresh Your Leather?
        </p>

        <h2 className="mt-4 text-4xl lg:text-6xl font-black leading-tight">
          Let’s Make It Look Expensive Again.
        </h2>

        <button className="mt-10 bg-black text-white px-8 py-5 rounded-2xl text-lg font-bold hover:scale-105 transition-transform">
          Get A Free Quote
        </button>

        <p className="mt-5 text-black/70 font-medium">
          Please text: 315-526-5959
        </p>
      </div>
    </div>
  </section>
</div>

); }