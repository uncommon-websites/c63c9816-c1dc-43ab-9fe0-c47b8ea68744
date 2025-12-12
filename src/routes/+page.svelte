<script>
    import Navbar from '$lib/components/Navbar.svelte';
    import Footer from '$lib/components/Footer.svelte';
    import FeatureRow from '$lib/components/FeatureRow.svelte';
</script>

<div class="bg-[var(--color-ifirma-dark)] min-h-screen flex flex-col">
    <Navbar />

    <main class="flex-grow">
        <!-- Hero Section -->
        <section class="relative pt-32 pb-20 overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="max-w-4xl mx-auto text-center">
                    <!-- Badge -->
                    <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm border border-white/10 rounded-full px-4 py-1.5 mb-8">
                        <span class="w-2 h-2 rounded-full bg-[var(--color-ifirma-primary)]"></span>
                        <span class="text-white text-sm font-medium">50+ Professionals</span>
                        <span class="text-gray-400 text-sm">across Flanders</span>
                    </div>

                    <h1 class="text-5xl md:text-7xl font-bold text-white tracking-tight mb-6 text-balance">
                        Complete property services. One trusted partner.
                    </h1>
                    
                    <p class="text-lg md:text-xl text-gray-400 mb-10 max-w-2xl mx-auto leading-relaxed text-balance">
                        IFIRMA delivers fast, flexible property services for Belgian real estate professionals. From photography to inspections, we handle everything so you can focus on closing deals.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                        <a href="tel:093200020" class="bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Call 09 320 00 20
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path>
                            </svg>
                        </a>
                        <a href="#services" class="bg-transparent border border-white/20 hover:bg-white/10 text-white px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Explore Services
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14M12 5l7 7-7 7"/>
                            </svg>
                        </a>
                    </div>
                </div>
            </div>

            <!-- Hero Images/Cards -->
            <div class="mt-20 relative">
                <div class="flex justify-center gap-6 overflow-hidden px-6">
                    <!-- Card 1 - Photography -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 transform -rotate-2 mt-8">
                        <img src="/generated/image-professional-real-estate-photographer-ta-1765572968984-0.webp" alt="Real estate photography" class="w-full h-full object-cover" />
                    </div>

                    <!-- Card 2 (Center) - Inspection -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 z-10">
                        <img src="/generated/image-electrical-inspector-examining-a-residen-1765572971846-1.webp" alt="Electrical inspection" class="w-full h-full object-cover" />
                    </div>

                    <!-- Card 3 - Property -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 transform rotate-2 mt-8">
                        <img src="/generated/image-beautiful-exterior-shot-of-a-modern-belg-1765572978428-4.webp" alt="Belgian property" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>
        </section>

        <!-- Stats Section -->
        <section class="py-12 border-y border-white/5 bg-black/20">
            <div class="container mx-auto px-6">
                <div class="grid grid-cols-2 md:grid-cols-4 gap-8 md:gap-12">
                    <div class="text-center">
                        <div class="text-4xl md:text-5xl font-bold text-white mb-2">50+</div>
                        <div class="text-sm text-gray-400">Team Members</div>
                    </div>
                    <div class="text-center">
                        <div class="text-4xl md:text-5xl font-bold text-white mb-2">150</div>
                        <div class="text-sm text-gray-400">Years Combined Experience</div>
                    </div>
                    <div class="text-center">
                        <div class="text-4xl md:text-5xl font-bold text-white mb-2">4</div>
                        <div class="text-sm text-gray-400">Office Locations</div>
                    </div>
                    <div class="text-center">
                        <div class="text-4xl md:text-5xl font-bold text-white mb-2">2014</div>
                        <div class="text-sm text-gray-400">Founded</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- IFIRMA Services Section -->
        <section class="py-32 relative overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="text-center mb-24">
                    <h2 class="text-[var(--color-ifirma-primary)] font-mono text-xs tracking-[0.2em] uppercase mb-6">Complete Solutions</h2>
                    <h3 class="text-4xl md:text-6xl font-bold text-white mb-2 tracking-tight">Property services.</h3>
                    <h3 class="text-4xl md:text-6xl font-bold text-gray-600 tracking-tight">Delivered with care.</h3>
                </div>

                <div class="grid md:grid-cols-2 gap-16 items-center max-w-6xl mx-auto">
                    <!-- Image Card -->
                    <div class="rounded-3xl overflow-hidden shadow-2xl border border-white/10">
                        <img src="/generated/image-team-of-diverse-property-service-profess-1765572976213-3.webp" alt="IFIRMA team" class="w-full h-full object-cover aspect-[4/3]" />
                    </div>

                    <!-- Text Content -->
                    <div class="space-y-8">
                        <h3 class="text-4xl md:text-5xl font-bold text-white tracking-tight">We care, so you can be carefree.</h3>
                        <p class="text-gray-400 text-lg leading-relaxed max-w-lg">
                            With 50+ professionals and 150 years of combined experience, IFIRMA delivers fast, flexible property services across Flanders. From photography to inspections, we handle everything.
                        </p>
                        <div class="flex flex-col gap-4">
                            <div class="flex items-center gap-3 text-white">
                                <div class="w-10 h-10 rounded-full bg-[var(--color-ifirma-primary)]/20 flex items-center justify-center">
                                    <svg class="w-5 h-5 text-[var(--color-ifirma-primary)]" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                                </div>
                                <span class="text-lg">MyIFIRMA Digital Platform</span>
                            </div>
                            <div class="flex items-center gap-3 text-white">
                                <div class="w-10 h-10 rounded-full bg-[var(--color-ifirma-primary)]/20 flex items-center justify-center">
                                    <svg class="w-5 h-5 text-[var(--color-ifirma-primary)]" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                                </div>
                                <span class="text-lg">4 Locations Across Flanders</span>
                            </div>
                            <div class="flex items-center gap-3 text-white">
                                <div class="w-10 h-10 rounded-full bg-[var(--color-ifirma-primary)]/20 flex items-center justify-center">
                                    <svg class="w-5 h-5 text-[var(--color-ifirma-primary)]" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                                </div>
                                <span class="text-lg">Dedicated Account Management</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- White Section -->
        <div class="bg-[#F9FAFB] text-black rounded-t-[4rem] relative z-20 mt-[-2rem] pt-32 pb-32">
            <div class="container mx-auto px-6">
                <!-- Header -->
                <div class="max-w-4xl mb-24" id="services">
                    <div class="flex items-center gap-4 mb-6">
                        <div class="h-px w-12 bg-gray-300"></div>
                        <span class="text-gray-500 font-mono text-xs tracking-[0.2em] uppercase">Our Services</span>
                    </div>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-900 mb-2 tracking-tight">Everything you need for property documentation.</h2>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-400 tracking-tight mb-8">Fast and flexible.</h2>
                    
                    <a href="tel:093200020" class="inline-flex items-center gap-2 text-sm font-semibold border-b border-black pb-0.5 hover:text-gray-600 transition-colors">
                        Contact us today
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </a>
                </div>

                <!-- Features Grid -->
                <div class="flex flex-col lg:flex-row gap-12">
                    <!-- Sidebar Navigation (Sticky) -->
                    <div class="hidden lg:block w-64 flex-shrink-0">
                        <div class="sticky top-32 space-y-4">
                            <div class="flex items-center gap-2 text-sm font-semibold text-black border-l-2 border-black pl-4 py-1">
                                <span class="w-1.5 h-1.5 rounded-full bg-[var(--color-ifirma-primary)]"></span>
                                Real Estate Photography
                            </div>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Electricity Inspections</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">EPC Certificates</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Floor Plans</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Virtual Tours</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Property Documentation</a>
                        </div>
                    </div>

                    <!-- Feature Cards -->
                    <div class="flex-grow space-y-8">
                        <FeatureRow 
                            title="Real Estate Photography" 
                            description="Professional property images that sell. Our team of 8 expert photographers capture stunning visuals that showcase properties at their best, helping agents close deals faster."
                            icon="camera"
                            image="photography"
                        />
                         <FeatureRow 
                            title="Electricity Inspections" 
                            description="Certified electrical safety reports. Our 5 qualified inspectors provide thorough electrical inspections that meet all Belgian regulatory requirements for property transactions."
                            icon="electric"
                            image="inspection"
                        />
                         <FeatureRow 
                            title="EPC Certificates" 
                            description="Energy performance documentation. We handle all EPC certification requirements quickly and accurately, ensuring your properties meet mandatory energy performance standards."
                            icon="certificate"
                            image="epc"
                        />
                         <FeatureRow 
                            title="Floor Plans & Measurements" 
                            description="Accurate property layouts. Professional floor plans and precise measurements that help buyers visualize spaces and make informed decisions about properties."
                            icon="floorplan"
                            image="floorplan"
                        />
                         <FeatureRow 
                            title="Virtual Tours" 
                            description="Immersive property experiences. Create engaging 360° virtual tours that allow potential buyers to explore properties remotely, expanding your reach and saving time."
                            icon="virtual"
                            image="virtual"
                        />
                         <FeatureRow 
                            title="Complete Documentation" 
                            description="All-in-one property services. From initial photography to final certifications, we coordinate all documentation needs through our MyIFIRMA platform for seamless service delivery."
                            icon="docs"
                            image="documentation"
                        />
                    </div>
                </div>

                <!-- MyIFIRMA Platform Section -->
                <div class="mt-32 text-center max-w-4xl mx-auto mb-24">
                    <div class="w-24 h-24 mx-auto bg-gradient-to-br from-purple-100 to-blue-100 rounded-full flex items-center justify-center mb-8 relative">
                        <div class="absolute inset-0 bg-white/50 blur-xl rounded-full"></div>
                        <svg class="w-10 h-10 text-[var(--color-ifirma-primary)] relative z-10" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                    </div>
                    <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8 leading-tight">
                        Order services online with MyIFIRMA — whether you're a real estate professional or private individual.
                    </h2>
                    <a href="#" class="bg-white border border-gray-200 hover:border-gray-400 text-black px-6 py-3 rounded-full font-medium transition-colors inline-flex items-center gap-2">
                        Access MyIFIRMA Platform
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </a>
                </div>

                <!-- Trusted By Section -->
                <div class="mb-32">
                    <p class="text-xl text-gray-500 mb-12">Trusted by real estate professionals across Flanders.</p>
                    
                    <div class="grid md:grid-cols-3 gap-6">
                        <!-- Main Testimonial Card -->
                        <div class="md:col-span-2 bg-[#0A0A0A] rounded-3xl p-10 relative overflow-hidden group min-h-[400px] flex flex-col justify-end">
                            <div class="absolute inset-0 opacity-30">
                                <img src="/generated/image-real-estate-agent-smiling-confidently-wh-1765572974068-2.webp" alt="Real estate agent" class="w-full h-full object-cover" />
                            </div>
                            <div class="absolute inset-0 bg-gradient-to-t from-black via-black/70 to-transparent"></div>
                            
                            <div class="relative z-10">
                                <div class="flex items-center gap-4 mb-6">
                                    <div class="w-12 h-12 rounded-full bg-[var(--color-ifirma-primary)] flex items-center justify-center text-white font-bold text-xl">
                                        IF
                                    </div>
                                </div>
                                <h3 class="text-3xl font-bold text-white mb-4 max-w-md">
                                    "IFIRMA handles everything so we can focus on what matters — closing deals."
                                </h3>
                                <p class="text-gray-300 mb-4">Real estate agents in Flanders save hours every week by partnering with IFIRMA for all their property documentation needs.</p>
                                <div class="w-10 h-10 rounded-full bg-white/10 backdrop-blur-md border border-white/20 flex items-center justify-center text-white group-hover:bg-white group-hover:text-black transition-colors">
                                    <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
                                </div>
                            </div>
                        </div>

                        <!-- Smaller Cards -->
                        <div class="space-y-6">
                            <!-- Card 2 - Fast Service -->
                            <div class="bg-[#0A0A0A] rounded-3xl p-8 relative overflow-hidden group h-[240px] flex flex-col justify-between">
                                <div class="absolute inset-0 bg-gradient-to-br from-purple-900/40 to-black"></div>
                                <div class="relative z-10">
                                    <div class="text-4xl font-bold text-white mb-2">24h</div>
                                    <p class="text-gray-300 text-sm">Average turnaround time for property photography</p>
                                </div>
                                <div class="relative z-10 flex justify-end">
                                    <div class="w-10 h-10 rounded-full bg-white/10 backdrop-blur-md border border-white/20 flex items-center justify-center text-white group-hover:bg-white group-hover:text-black transition-colors">
                                        <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
                                    </div>
                                </div>
                            </div>
                            <!-- Card 3 - Coverage -->
                            <div class="bg-[#0A0A0A] rounded-3xl p-8 relative overflow-hidden group h-[240px] flex flex-col justify-between">
                                <div class="absolute inset-0 bg-gradient-to-br from-blue-900/40 to-black"></div>
                                <div class="relative z-10">
                                    <div class="text-4xl font-bold text-white mb-2">100%</div>
                                    <p class="text-gray-300 text-sm">Flanders coverage with 4 office locations</p>
                                </div>
                                <div class="relative z-10 flex justify-end">
                                    <div class="w-10 h-10 rounded-full bg-white/10 backdrop-blur-md border border-white/20 flex items-center justify-center text-white group-hover:bg-white group-hover:text-black transition-colors">
                                        <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Banner -->
                <div class="bg-[#0A0A0A] rounded-3xl p-12 md:p-20 relative overflow-hidden mb-32 text-center">
                    <div class="absolute inset-0 bg-[url('/grid-pattern.svg')] opacity-10"></div>
                    <div class="absolute left-0 top-0 w-64 h-64 bg-purple-500/10 blur-[100px] rounded-full"></div>
                    <div class="absolute right-0 bottom-0 w-64 h-64 bg-blue-500/10 blur-[100px] rounded-full"></div>
                    
                    <div class="relative z-10 max-w-3xl mx-auto">
                        <h2 class="text-4xl md:text-6xl font-bold text-white mb-6 tracking-tight">
                            Complete property services. <span class="text-[var(--color-ifirma-primary)]">Delivered fast.</span>
                        </h2>
                        <p class="text-gray-400 mb-10">
                            Built for real estate professionals, our integrated platform and expert teams handle everything from photography to inspections.
                        </p>
                        <a href="tel:093200020" class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-md border border-white/10 rounded-full px-6 py-3 text-white text-sm hover:bg-white/20 transition-colors">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path></svg>
                            Contact Us: 09 320 00 20
                        </a>
                    </div>
                </div>

                <!-- Services Overview -->
                <div class="text-center mb-32">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
                        Photography. Inspections. Certifications.<br>
                        <span class="text-gray-400">Everything you need for<br>property documentation.</span>
                    </h2>
                    <a href="mailto:klantendienst@ifirma.be" class="bg-gray-100 hover:bg-gray-200 text-black px-6 py-2 rounded-full text-sm font-medium transition-colors inline-flex items-center gap-2 mx-auto mb-16 mt-8">
                        Get in touch
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </a>

                    <div class="grid grid-cols-2 md:grid-cols-4 gap-px bg-gray-200 border border-gray-200 rounded-2xl overflow-hidden">
                        {#each [
                            {name: 'Photography', icon: 'camera'},
                            {name: 'Inspections', icon: 'clipboard'},
                            {name: 'EPC Certificates', icon: 'certificate'},
                            {name: 'Floor Plans', icon: 'layout'},
                            {name: 'Virtual Tours', icon: 'video'},
                            {name: 'Documentation', icon: 'file'},
                            {name: 'MyIFIRMA', icon: 'monitor'},
                            {name: 'Support', icon: 'headphones'}
                        ] as service}
                        <div class="bg-[#F9FAFB] p-12 flex flex-col items-center justify-center hover:bg-white transition-all duration-300 group">
                            <div class="w-12 h-12 mb-3 rounded-full bg-gray-100 group-hover:bg-[var(--color-ifirma-primary)]/10 flex items-center justify-center transition-colors">
                                <svg class="w-6 h-6 text-gray-400 group-hover:text-[var(--color-ifirma-primary)] transition-colors" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    {#if service.icon === 'camera'}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 9a2 2 0 012-2h.93a2 2 0 001.664-.89l.812-1.22A2 2 0 0110.07 4h3.86a2 2 0 011.664.89l.812 1.22A2 2 0 0018.07 7H19a2 2 0 012 2v9a2 2 0 01-2 2H5a2 2 0 01-2-2V9z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 13a3 3 0 11-6 0 3 3 0 016 0z"></path>
                                    {:else if service.icon === 'clipboard'}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-6 9l2 2 4-4"></path>
                                    {:else if service.icon === 'certificate'}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                    {:else if service.icon === 'layout'}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 5a1 1 0 011-1h4a1 1 0 011 1v7a1 1 0 01-1 1H5a1 1 0 01-1-1V5zM14 5a1 1 0 011-1h4a1 1 0 011 1v7a1 1 0 01-1 1h-4a1 1 0 01-1-1V5zM4 16a1 1 0 011-1h4a1 1 0 011 1v3a1 1 0 01-1 1H5a1 1 0 01-1-1v-3zM14 16a1 1 0 011-1h4a1 1 0 011 1v3a1 1 0 01-1 1h-4a1 1 0 01-1-1v-3z"></path>
                                    {:else if service.icon === 'video'}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 10l4.553-2.276A1 1 0 0121 8.618v6.764a1 1 0 01-1.447.894L15 14M5 18h8a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v8a2 2 0 002 2z"></path>
                                    {:else if service.icon === 'file'}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21h10a2 2 0 002-2V9.414a1 1 0 00-.293-.707l-5.414-5.414A1 1 0 0012.586 3H7a2 2 0 00-2 2v14a2 2 0 002 2z"></path>
                                    {:else if service.icon === 'monitor'}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                                    {:else}
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M18.364 5.636l-3.536 3.536m0 5.656l3.536 3.536M9.172 9.172L5.636 5.636m3.536 9.192l-3.536 3.536M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-5 0a4 4 0 11-8 0 4 4 0 018 0z"></path>
                                    {/if}
                                </svg>
                            </div>
                            <span class="font-semibold text-sm text-gray-700">{service.name}</span>
                        </div>
                        {/each}
                    </div>
                </div>

                <!-- Blog Section -->
                <div class="mb-12">
                    <h2 class="text-4xl font-bold text-gray-900 mb-12">Insights for real estate professionals.</h2>
                    <div class="grid md:grid-cols-2 gap-8">
                        <!-- Post 1 -->
                        <div class="group cursor-pointer">
                            <div class="rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden">
                                <img src="/generated/image-beautiful-exterior-shot-of-a-modern-belg-1765572978428-4.webp" alt="Belgian property" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Property Marketing</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-[var(--color-ifirma-primary)] transition-colors">How professional photography increases property sales by 30%</h3>
                        </div>
                        <!-- Post 2 -->
                        <div class="group cursor-pointer">
                            <div class="rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden">
                                <img src="/generated/image-close-up-of-hands-holding-an-energy-perf-1765572980615-5.webp" alt="EPC certificate" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" />
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Compliance</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-[var(--color-ifirma-primary)] transition-colors">Understanding EPC requirements in Belgian real estate</h3>
                        </div>
                    </div>
                </div>


    </main>

    <Footer />
</div>

