<template>
    <div class="flex flex-col md:flex-row items-center w-full mx-auto">
        <div class="flex-1">
            <h1 class="text-4xl md:text-5xl lg:text-6xl mt-4 mx-auto text-center font-bold couleur-bleue">
                Neopass, logiciel pour Particuliers / ESAT / Entreprises
            </h1>
            <h2 class="text-3xl md:text-4xl lg:text-5xl mt-4 mx-auto text-center font-bold couleur-rose">
                Parcours socio-professionnel et Gestion des compétences
            </h2>
            <div class="flex flex-row mx-auto justify-around ml-4 mr-4 mt-6">
                <button 
                class=" 
                hover:bg-[rgba(53,36,200,0.68)]
                text-[#21b8c8] font-semibold 
                hover:text-white 
                py-2 
                px-4 
                border-2 
                border-[#21b8c8] 
                rounded
                transition duration-500 ease-in-out"
                style="font-size:14px"
                >
                    ESSAYER GRATUITEMENT
                </button>
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
                ml-4
                flex flex-row"
                style="font-size:14px"
                >
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-6 h-6 pr-2">
                        <path d="M4.5 4.5a3 3 0 00-3 3v9a3 3 0 003 3h8.25a3 3 0 003-3v-9a3 3 0 00-3-3H4.5zM19.94 18.75l-2.69-2.69V7.94l2.69-2.69c.944-.945 2.56-.276 2.56 1.06v11.38c0 1.336-1.616 2.005-2.56 1.06z" />
                    </svg>
                    VIDEO
                </button>
            </div>
        </div>
        <div class="flex-1">
            <img 
                src="../assets/images/iphone-tablet-mockup-blanc-2-768x604.png" 
                alt="Neopass - sur tous supports (tablettes, ios, android, pc, mac)"
                class="object-scale-down"
            />
        </div>
    </div>
</template>