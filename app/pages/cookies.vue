<template>
    <div class="container mx-auto px-4 py-10">
        <div class="card bg-base-100 shadow-xl">
            <div class="card-body space-y-6">
                <!-- Titre principal -->
                <h1 class="card-title text-3xl font-bold text-primary">
                    Politique de cookies
                </h1>
                <p class="text-sm text-gray-500">
                    Dernière mise à jour : 17 septembre 2025
                </p>

                <!-- Section 1 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">1. Qu’est-ce qu’un cookie ?</h2>
                    <p>
                        Un cookie est un petit fichier texte enregistré sur votre appareil lorsque
                        vous visitez notre site. Il permet de reconnaître votre appareil et de
                        mémoriser vos préférences.
                    </p>
                </section>

                <!-- Section 2 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">2. Types de cookies utilisés</h2>
                    <ul class="list-disc list-inside space-y-1">
                        <li>Cookies strictement nécessaires au fonctionnement du site</li>
                        <li>Cookies de performance et d’analyse</li>
                        <li>Cookies de personnalisation</li>
                        <li>Cookies publicitaires et de réseaux sociaux</li>
                    </ul>
                </section>

                <!-- Section 3 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">3. Gestion des cookies</h2>
                    <p>
                        Vous pouvez configurer votre navigateur pour bloquer ou supprimer les
                        cookies. Cependant, certaines fonctionnalités de notre site pourraient ne
                        pas fonctionner correctement si les cookies sont désactivés.
                    </p>
                </section>

                <!-- Section 4 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">4. Consentement</h2>
                    <p>
                        En continuant à utiliser notre site, vous acceptez l’utilisation des
                        cookies conformément à cette politique.
                    </p>
                </section>

                <!-- Section 5 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">5. Mise à jour de la politique</h2>
                    <p>
                        Nous pouvons modifier cette politique de cookies à tout moment. Les
                        changements seront publiés sur cette page.
                    </p>
                </section>

                <!-- Bouton retour -->
                <div class="pt-6">
                    <router-link to="/" class="btn btn-primary">
                        ← Retour à l'accueil
                    </router-link>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
// Pas de logique spécifique
</script>

<style scoped>
/* DaisyUI + Tailwind s’occupent du style */
</style>