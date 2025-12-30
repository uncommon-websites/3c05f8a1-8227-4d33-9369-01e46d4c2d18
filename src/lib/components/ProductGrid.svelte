<script lang="ts">
    import ProductCard from './ProductCard.svelte';

    const products = [
        {
            badge: "Most Popular",
            code: "01",
            title: "Birth Doula Support",
            image: "/generated/image-professional-doula-supporting-pregnant-w-1767054104946-1.webp", 
            price: "Custom"
        },
        {
            badge: "Essential",
            code: "02",
            title: "Postpartum Planning",
            image: "/generated/image-confident-expecting-mother-preparing-nur-1767054107550-2.webp", 
            price: "Custom"
        },
        {
            badge: "New",
            code: "03",
            title: "Virtual Courses",
            image: "/generated/image-pregnant-woman-doing-prenatal-yoga-in-br-1767054115437-5.webp",
            price: "Coming Soon"
        },
        {
            badge: "Comprehensive",
            code: "04",
            title: "Fair Play Facilitation",
            image: "/generated/image-expecting-couple-planning-together-at-ho-1767054118051-6.webp",
            price: "Custom"
        }
    ];
</script>

<section class="bg-primary-950 py-24">
    <div class="container mx-auto px-6 md:px-12">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 text-white">
            <div class="max-w-xl">
                <h2 class="text-4xl md:text-[44px] leading-tight font-serif tracking-tight mb-6">Comprehensive support for your journey to parenthood.</h2>
                <p class="text-[17px] text-white/80 font-light max-w-md leading-relaxed">From birth preparation to postpartum planning, we provide strategic support covering every detail of your transition to parenthood.</p>
            </div>
            <a href="/" class="hidden md:inline-flex items-center text-[13px] font-bold border-b border-white/30 pb-0.5 hover:border-white transition-colors mt-6 md:mt-0 tracking-wide uppercase">
                View All Services <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
            {#each products as product}
                <ProductCard {...product} isDark={true} />
            {/each}
        </div>

        <div class="mt-12 text-center md:hidden">
            <a href="/" class="inline-flex items-center text-[13px] font-bold border-b border-white/30 pb-0.5 hover:border-white transition-colors text-white tracking-wide uppercase">
                View All Services <span class="ml-2">→</span>
            </a>
        </div>
    </div>
</section>
