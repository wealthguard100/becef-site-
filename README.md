‎resources.html, thank-you.html, moi.html
‎
‎export default function BICEFWebsite() { const services = [ { title: "1-Day Business Bootcamp", price: "15,000 RWF", description: "Practical training for small business owners on finance, customer service, and growth strategies.", }, { title: "Digital Kiosk Setup", price: "50,000 RWF", description: "Simple digital systems using WhatsApp, Excel, and MoMo to improve operations.", }, { title: "Business Redesign", price: "100,000 RWF", description: "Business improvement plans to increase efficiency and reduce losses.", }, { title: "Market Survey", price: "75,000 RWF", description: "Affordable customer and market research for local businesses.", }, ];
‎
‎const team = [ { name: "BYIRINGIRO Eduard", role: "CEO & Head of Partnerships", phone: "+250 795 431 925", }, { name: "MASEGESHO Comfiance", role: "Chief Product Officer", phone: "+250 796 226 255", }, { name: "IZIBYOSE Patrick", role: "Chief Technology Officer", phone: "+250 793 125 226", }, { name: "HAKIZIMANA Fidel", role: "COO & Head of Growth", phone: "+250 794 961 256", }, ];
‎
‎return ( <div className="min-h-screen bg-gray-50 text-gray-800 font-sans"> {/* Header */} <header className="bg-gradient-to-r from-blue-700 via-green-600 to-orange-500 text-white shadow-lg"> <div className="max-w-7xl mx-auto px-6 py-6 flex flex-col md:flex-row justify-between items-center"> <div> <h1 className="text-3xl font-bold">BICEF</h1> <p className="italic text-sm mt-1"> Business Innovation & Consulting Enterprise Firm Ltd </p> </div>
‎
‎<nav className="flex gap-6 mt-4 md:mt-0 text-sm font-medium">
‎        <a href="#home" className="hover:underline">
‎          Home
‎        </a>
‎        <a href="#about" className="hover:underline">
‎          About
‎        </a>
‎        <a href="#services" className="hover:underline">
‎          Services
‎        </a>
‎        <a href="#team" className="hover:underline">
‎          Team
‎        </a>
‎        <a href="#contact" className="hover:underline">
‎          Contact
‎        </a>
‎      </nav>
‎    </div>
‎  </header>
‎
‎  {/* Hero Section */}
‎  <section
‎    id="home"
‎    className="bg-white py-20 px-6 text-center border-b"
‎  >
‎    <div className="max-w-4xl mx-auto">
‎      <h2 className="text-5xl font-extrabold leading-tight text-blue-800">
‎        Building Businesses That Build Communities
‎      </h2>
‎
‎      <p className="mt-6 text-lg text-gray-600 leading-relaxed">
‎        BICEF helps micro and small businesses in Kigali grow through
‎        affordable consulting, practical training, and digital business
‎        solutions.
‎      </p>
‎
‎      <div className="mt-8 flex flex-col sm:flex-row justify-center gap-4">
‎        <button className="bg-blue-700 hover:bg-blue-800 text-white px-6 py-3 rounded-2xl shadow-md font-semibold">
‎          Explore Services
‎        </button>
‎        <button className="bg-green-600 hover:bg-green-700 text-white px-6 py-3 rounded-2xl shadow-md font-semibold">
‎          Contact Us
‎        </button>
‎      </div>
‎    </div>
‎  </section>
‎
‎  {/* About Section */}
‎  <section id="about" className="py-16 px-6 bg-gray-100">
‎    <div className="max-w-6xl mx-auto grid md:grid-cols-2 gap-10 items-center">
‎      <div>
‎        <h3 className="text-3xl font-bold text-blue-800 mb-4">
‎          About BICEF
‎        </h3>
‎        <p className="text-gray-700 leading-relaxed text-lg">
‎          Business Innovation & Consulting Enterprise Firm Ltd (BICEF)
‎          provides low-cost and practical consulting solutions for
‎          micro-SMEs in Rwanda. Our mission is to empower local businesses
‎          with modern tools, business knowledge, and strategic support.
‎        </p>
‎
‎        <p className="mt-4 text-gray-700 leading-relaxed">
‎          We focus on business growth, digital transformation, and community
‎          impact through youth-led innovation.
‎        </p>
‎      </div>
‎
‎      <div className="bg-white rounded-3xl shadow-lg p-8 border-l-8 border-orange-500">
‎        <h4 className="text-2xl font-bold mb-4 text-green-700">
‎          Our Goals
‎        </h4>
‎        <ul className="space-y-3 text-gray-700">
‎          <li>✔ Serve 100 SMEs in the first 6 months</li>
‎          <li>✔ Generate 2.3M RWF revenue</li>
‎          <li>✔ Register officially with RDB</li>
‎          <li>✔ Expand across Kigali sectors</li>
‎        </ul>
‎      </div>
‎    </div>
‎  </section>
‎
‎  {/* Services */}
‎  <section id="services" className="py-20 px-6 bg-white">
‎    <div className="max-w-7xl mx-auto">
‎      <div className="text-center mb-14">
‎        <h3 className="text-4xl font-bold text-blue-800">
‎          Our Services
‎        </h3>
‎        <p className="mt-4 text-gray-600 text-lg">
‎          Affordable business solutions designed for micro-SMEs.
‎        </p>
‎      </div>
‎
‎      <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
‎        {services.map((service, index) => (
‎          <div
‎            key={index}
‎            className="bg-gray-50 rounded-3xl shadow-md p-6 hover:shadow-xl transition duration-300 border-t-4 border-blue-600"
‎          >
‎            <h4 className="text-xl font-bold text-green-700 mb-2">
‎              {service.title}
‎            </h4>
‎            <p className="text-orange-500 font-semibold mb-3">
‎              {service.price}
‎            </p>
‎            <p className="text-gray-600 leading-relaxed">
‎              {service.description}
‎            </p>
‎          </div>
‎        ))}
‎      </div>
‎    </div>
‎  </section>
‎
‎  {/* Impact Section */}
‎  <section className="py-20 px-6 bg-gradient-to-r from-blue-700 to-green-600 text-white">
‎    <div className="max-w-6xl mx-auto text-center">
‎      <h3 className="text-4xl font-bold mb-6">Our Early Impact</h3>
‎
‎      <div className="grid md:grid-cols-3 gap-8 mt-10">
‎        <div className="bg-white/10 rounded-3xl p-8 shadow-lg">
‎          <h4 className="text-5xl font-bold">10</h4>
‎          <p className="mt-3 text-lg">Pilot Dukas Supported</p>
‎        </div>
‎
‎        <div className="bg-white/10 rounded-3xl p-8 shadow-lg">
‎          <h4 className="text-5xl font-bold">18%</h4>
‎          <p className="mt-3 text-lg">Reduction in Stock Waste</p>
‎        </div>
‎
‎        <div className="bg-white/10 rounded-3xl p-8 shadow-lg">
‎          <h4 className="text-5xl font-bold">100%</h4>
‎          <p className="mt-3 text-lg">Client Recommendation</p>
‎        </div>
‎      </div>
‎    </div>
‎  </section>
‎
‎  {/* Team */}
‎  <section id="team" className="py-20 px-6 bg-gray-100">
‎    <div className="max-w-7xl mx-auto">
‎      <div className="text-center mb-14">
‎        <h3 className="text-4xl font-bold text-blue-800">Meet Our Team</h3>
‎        <p className="mt-4 text-gray-600 text-lg">
‎          Young innovators committed to empowering businesses.
‎        </p>
‎      </div>
‎
‎      <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
‎        {team.map((member, index) => (
‎          <div
‎            key={index}
‎            className="bg-white rounded-3xl shadow-lg p-6 text-center hover:shadow-2xl transition"
‎          >
‎            <div className="w-24 h-24 mx-auto rounded-full bg-gradient-to-r from-blue-600 to-green-500 mb-5 flex items-center justify-center text-white text-3xl font-bold">
‎              {member.name.charAt(0)}
‎            </div>
‎
‎            <h4 className="text-xl font-bold text-gray-800">
‎              {member.name}
‎            </h4>
‎            <p className="text-green-700 mt-2 font-medium">
‎              {member.role}
‎            </p>
‎            <p className="text-gray-500 mt-3 text-sm">{member.phone}</p>
‎          </div>
‎        ))}
‎      </div>
‎    </div>
‎  </section>
‎
‎  {/* Contact */}
‎  <section id="contact" className="py-20 px-6 bg-white">
‎    <div className="max-w-4xl mx-auto text-center">
‎      <h3 className="text-4xl font-bold text-blue-800">
‎        Contact BICEF
‎      </h3>
‎
‎      <p className="mt-6 text-lg text-gray-600">
‎        Ready to improve your business? Reach out today.
‎      </p>
‎
‎      <div className="mt-10 bg-gray-100 rounded-3xl shadow-lg p-10">
‎        <p className="text-xl font-semibold text-gray-800">
‎          📧 bicef.rw@gmail.com
‎        </p>
‎        <p className="text-xl font-semibold text-gray-800 mt-4">
‎          📱 +250 795 431 925
‎        </p>
‎        <p className="text-lg text-gray-600 mt-4">
‎          Kigali, Rwanda
‎        </p>
‎      </div>
‎    </div>
‎  </section>
‎
‎  {/* Footer */}
‎  <footer className="bg-gray-900 text-white py-8 text-center">
‎    <h4 className="text-2xl font-bold">BICEF</h4>
‎    <p className="mt-2 text-gray-400">
‎      Business Innovation & Consulting Enterprise Firm Ltd
‎    </p>
‎    <p className="mt-4 text-sm text-gray-500">
‎      © 2026 BICEF Ltd. All rights reserved.
‎    </p>
‎  </footer>
‎</div>
‎
‎); }
‎