<script>
    import { onMount } from 'svelte';

    let isScrolled = false;

    onMount(() => {
        const handleScroll = () => {
            isScrolled = window.scrollY > 20;
        };
        window.addEventListener('scroll', handleScroll);
        return () => window.removeEventListener('scroll', handleScroll);
    });
</script>

<nav class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 {isScrolled ? 'bg-black/80 backdrop-blur-md py-4' : 'bg-transparent py-6'}">
    <div class="container mx-auto px-6 flex items-center justify-between">
        <!-- Logo -->
        <a href="/" class="flex items-center gap-2 text-white font-bold text-2xl tracking-tight">
            IFIRMA
        </a>

        <!-- Links -->
        <div class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-300">
            <a href="#" class="hover:text-white transition-colors">Services</a>
            <a href="#" class="hover:text-white transition-colors">For Professionals</a>
            <a href="#" class="hover:text-white transition-colors">MyIFIRMA</a>
            <a href="#" class="hover:text-white transition-colors">About Us</a>
            <a href="#" class="hover:text-white transition-colors">Contact</a>
        </div>

        <!-- CTA -->
        <a href="tel:093200020" class="hidden md:flex items-center gap-2 text-sm font-medium text-white hover:text-[var(--color-ifirma-primary)] transition-colors">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path>
            </svg>
            09 320 00 20
        </a>
        
        <!-- Mobile Menu Button -->
        <button class="md:hidden text-white">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <line x1="3" y1="12" x2="21" y2="12"></line>
                <line x1="3" y1="6" x2="21" y2="6"></line>
                <line x1="3" y1="18" x2="21" y2="18"></line>
            </svg>
        </button>
    </div>
</nav>
