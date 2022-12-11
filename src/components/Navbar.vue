<template>
    <div class="bg-white">
        <nav
            class="
            container
            px-4
            py-8
            mx-auto
            md:flex md:justify-between md:items-center
            "
            style="font-family: 'roboto', sans-serif;"
        >
            <div class="flex items-center justify-between">
                <router-link
                    to="/"
                    class="
                    text-xl
                    font-bold
                    couleur-bleue
                    md:text-2xl
                    
                    "
                    ><img src="../assets/images/logo-neopass-header.png" alt="Logo Neopass" style="min-width: 130px; max-width: 176px;">
                </router-link>
                <!-- Mobile menu button -->
                <div @click="toggleNav" class="flex md:hidden">
                    <button
                    type="button"
                    class="
                        couleur-bleue
                        hover:text-gray-400
                        focus:outline-none focus:text-gray-400
                    "
                    >
                    <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                        <path
                        fill-rule="evenodd"
                        d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
                        ></path>
                    </svg>
                    </button>
                </div>
            </div>

            <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
            <div class="flex md:flex-col lg:flex-row-reverse ">
                <div class="flex justify-end invisible md:visible">
                    <div class="">
                        <button 
                            class="bg-transparent 
                            hover:bg-[rgba(53,36,200,0.68)]
                            couleur-bleue font-semibold 
                            hover:text-white 
                            py-2 
                            px-4 
                            border-2 
                            border-[#3524c8] 
                            rounded
                            transition duration-500 ease-in-out
                            whitespace-nowrap
                            ml-4"
            
                            style="font-size:14px"
                        >
                        ESSAI GRATUIT
                        </button>
                    </div>
                    <div class="">
                        <button 
                            class="bg-transparent 
                            hover:bg-[rgba(53,36,200,0.68)]
                            text-[#21b8c8] font-semibold 
                            hover:text-white 
                            py-2 
                            px-4 
                            border-2 
                            border-[#21b8c8] 
                            rounded
                            transition duration-500 ease-in-out
                            ml-4"
            
                            style="font-size:14px"
                        >
                        CONNEXION
                        </button>
                    </div>
                </div>
                <ul
                :class="showMenu ? 'flex' : 'hidden'"
                class="
                    flex-col
                    mt-8
                    space-y-4
                    md:flex md:space-y-0 md:flex-row md:items-center md:space-x-5 md:mt-0
                    font-normal
                "
                >
                    <li class="couleur-rose active">Accueil</li>
                    <li>
                        <span class="group relative inline-block">
                            <button class="inline-flex items-center rounded py-2 px-4 couleur-bleue">Nos Solutions</button>
                            <ul class="absolute hidden pt-1 group-hover:block couleur-rose">
                                <li class="w-32">
                                    <a class="whitespace-nowrap block rounded-t-lg bg-gray-100 py-2 px-4 hover:bg-gray-200 hover:text-[#3524c8]" href="#">Particulier</a>
                                </li>
                                <li class="">
                                    <a class="whitespace-nowrap block rounded-b-lg bg-gray-100 py-2 px-4 hover:bg-gray-200 hover:text-[#3524c8]" href="#">Structure</a>
                                </li>
                            </ul>
                        </span>
                    </li>
                    <li class="couleur-bleue">Modules</li>
                    <li class="couleur-bleue">Tarifs</li>
                    <li class="couleur-bleue">Contact</li>
                    <li class="couleur-bleue md:hidden">Essai Gratuit</li>
                    <li class="couleur-bleue md:hidden">Connexion</li>
                </ul>
            </div>
        </nav>
    </div>

</template>

<script>
    import { ref } from 'vue';
    export default {
        setup() {
            let showMenu = ref(false);
            const toggleNav = () => (showMenu.value = !showMenu.value);
            return { showMenu, toggleNav };
        },
    };
</script>