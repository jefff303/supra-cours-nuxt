<template>
    <div class="container mx-auto px-4 py-10">
        <div class="card bg-base-100 shadow-xl">
            <div class="card-body space-y-6">
                <!-- Titre principal -->
                <h1 class="card-title text-3xl font-bold text-primary">
                    Politique de confidentialité
                </h1>
                <p class="text-sm text-gray-500">
                    Dernière mise à jour : 17 septembre 2025
                </p>

                <!-- Section 1 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">1. Collecte des informations</h2>
                    <p>
                        Nous collectons des informations lorsque vous vous inscrivez sur notre
                        site, lorsque vous vous connectez à votre compte, effectuez un achat,
                        participez à un concours, et/ou lorsque vous vous déconnectez. Les
                        informations collectées incluent votre nom, votre adresse e-mail, votre
                        numéro de téléphone et/ou carte de crédit.
                    </p>
                </section>

                <!-- Section 2 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">2. Utilisation des informations</h2>
                    <p>
                        Toutes les informations que nous recueillons auprès de vous peuvent être
                        utilisées pour :
                    </p>
                    <ul class="list-disc list-inside space-y-1">
                        <li>Personnaliser votre expérience</li>
                        <li>Améliorer notre site web</li>
                        <li>Améliorer le service client et vos besoins de prise en charge</li>
                        <li>Vous contacter par e-mail</li>
                        <li>Administrer un concours, une promotion ou une enquête</li>
                    </ul>
                </section>

                <!-- Section 3 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">3. Confidentialité des informations</h2>
                    <p>
                        Nous sommes les seuls propriétaires des informations recueillies sur ce
                        site. Vos informations personnelles ne seront ni vendues, échangées,
                        transférées ou données à une autre société sans votre consentement, en
                        dehors de ce qui est nécessaire pour répondre à une demande et/ou une
                        transaction.
                    </p>
                </section>

                <!-- Section 4 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">4. Protection des informations</h2>
                    <p>
                        Nous mettons en œuvre une variété de mesures de sécurité pour préserver la
                        sécurité de vos informations personnelles. Nous utilisons un
                        cryptage avancé pour protéger les informations sensibles transmises en
                        ligne.
                    </p>
                </section>

                <!-- Section 5 -->
                <section>
                    <h2 class="text-xl font-semibold mb-2">5. Consentement</h2>
                    <p>
                        En utilisant notre site, vous consentez à notre politique de
                        confidentialité.
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
/* DaisyUI + Tailwind gèrent le style */
</style>