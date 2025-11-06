<template>
    <div class="container mx-auto px-4 py-10">
        <div class="card bg-base-100 shadow-xl">
            <div class="card-body space-y-6">
                <!-- Titre principal -->
                <h1 class="card-title text-3xl font-bold text-primary">
                    Conditions d'utilisation
                </h1>
                <p class="text-sm text-gray-500">
                    Dernière mise à jour : 17 septembre 2025
                </p>

                <!-- Section 1 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">1. Acceptation des conditions</h2>
                    <p>
                        En accédant à notre site ou en l'utilisant, vous acceptez d’être lié par
                        ces conditions d’utilisation et toutes les lois applicables.
                    </p>
                </section>

                <!-- Section 2 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">2. Utilisation du service</h2>
                    <p>
                        Vous vous engagez à ne pas utiliser le service à des fins illégales ou interdites.
                        Toute utilisation abusive pourra entraîner la suspension ou la résiliation de votre compte.
                    </p>
                </section>

                <!-- Section 3 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">3. Propriété intellectuelle</h2>
                    <p>
                        Le contenu, la structure et le design de ce site sont protégés par le droit d’auteur.
                        Vous ne pouvez reproduire ou distribuer sans autorisation.
                    </p>
                </section>

                <!-- Section 4 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">4. Limitation de responsabilité</h2>
                    <p>
                        Nous ne pouvons être tenus responsables des dommages indirects ou consécutifs
                        résultant de l’utilisation ou de l’incapacité à utiliser nos services.
                    </p>
                </section>

                <!-- Section 5 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">5. Modification des conditions</h2>
                    <p>
                        Nous nous réservons le droit de modifier ces conditions à tout moment.
                        Nous vous informerons de tout changement majeur par email ou sur cette page.
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