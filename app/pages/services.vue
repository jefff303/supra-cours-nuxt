<template>
    <div class="container mx-auto px-4 py-10">
        <!-- Titre principal -->
        <div class="text-center mb-10">
            <h1 class="text-4xl font-bold text-primary">Nos Services</h1>
            <p class="text-gray-500 mt-2">
                Découvrez ce que nous proposons pour vous accompagner.
            </p>
        </div>

        <!-- Grille de services -->
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
            <div v-for="(service, index) in services" :key="index"
                class="card bg-base-100 shadow-xl hover:shadow-2xl transition duration-300">
                <figure class="px-10 pt-10">
                    <!-- On affiche l'icône -->
                    <!-- <i :is="service.icon" class="w-16 h-16 text-primary" /> -->
                </figure>
                <div class="card-body items-center text-center">
                    <h2 class="card-title text-xl font-semibold">{{ service.title }}</h2>
                    <p class="text-gray-600">{{ service.description }}</p>
                    <div class="card-actions justify-center mt-4">
                        <!-- <NuxtLink :to="service.link" class="btn btn-primary btn-sm">
                            En savoir plus
                        </NuxtLink> -->
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
// Ici on utilise @nuxt/icon :
// Les noms des icônes dépendent du pack que tu as choisi (ex: heroicons:solid/home, heroicons:outline/user, etc.)
const services = [
    {
        title: 'Développement Web',
        description:
            'Des applications modernes et performantes avec Nuxt, Vue.js et Tailwind.',
        icon: 'arrow-right-circle-16-solid',
        link: '/services/web'
    },
    {
        title: 'Design & UI/UX',
        description:
            'Des interfaces centrées utilisateur, accessibles et esthétiques.',
        icon: 'heroicons:paint-brush',
        link: '/services/design'
    },
    {
        title: 'Sécurité & Audits',
        description:
            'Analyse, tests de sécurité et audits pour protéger vos données.',
        icon: 'heroicons:shield-check',
        link: '/services/security'
    },
    {
        title: 'Accompagnement & Formation',
        description:
            'Ateliers et formations sur mesure pour vos équipes techniques.',
        icon: 'heroicons:users',
        link: '/services/training'
    },
    {
        title: 'Gestion de données',
        description:
            'Solutions complètes de gestion et d’analyse de données à grande échelle.',
        icon: 'heroicons:database',
        link: '/services/data'
    },
    {
        title: 'Lancement de projets',
        description:
            'De l’idée au produit final, nous accompagnons vos projets innovants.',
        icon: 'heroicons:rocket-launch',
        link: '/services/launch'
    }
]
</script>

<style scoped>
/* DaisyUI et Tailwind gèrent déjà le style */
</style>