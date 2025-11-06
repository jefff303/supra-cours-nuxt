<template>
    <div class="container mx-auto p-6">
        <!-- Titre de la page -->
        <div class="text-center mb-8">
            <h1 class="text-4xl font-bold mb-2">Contactez-nous</h1>
            <p class="text-gray-600 text-lg">
                Vous avez une question ou une remarque ? Envoyez-nous un message !
            </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            <!-- Formulaire de contact -->
            <div class="card bg-base-100 shadow-xl">
                <div class="card-body">
                    <h2 class="text-2xl font-semibold mb-4">Formulaire de Contact</h2>

                    <form @submit.prevent="envoyerMessage" class="space-y-4">
                        <!-- Nom -->
                        <div class="form-control">
                            <label class="label">
                                <span class="label-text">Votre nom</span>
                            </label>
                            <input v-model="form.nom" type="text" placeholder="Votre nom"
                                class="input input-bordered w-full" required />
                        </div>

                        <!-- Email -->
                        <div class="form-control">
                            <label class="label">
                                <span class="label-text">Votre email</span>
                            </label>
                            <input v-model="form.email" type="email" placeholder="email@exemple.com"
                                class="input input-bordered w-full" required />
                        </div>

                        <!-- Sujet -->
                        <div class="form-control">
                            <label class="label">
                                <span class="label-text">Sujet</span>
                            </label>
                            <input v-model="form.sujet" type="text" placeholder="Sujet de votre message"
                                class="input input-bordered w-full" required />
                        </div>

                        <!-- Message -->
                        <div class="form-control">
                            <label class="label">
                                <span class="label-text">Votre message</span>
                            </label>
                            <textarea v-model="form.message" class="textarea textarea-bordered w-full"
                                placeholder="Tapez votre message ici" required></textarea>
                        </div>

                        <!-- Bouton Envoyer -->
                        <button type="submit" class="btn btn-primary w-full">Envoyer</button>
                    </form>
                </div>
            </div>

            <!-- Infos de contact -->
            <div class="card bg-base-100 shadow-xl">
                <div class="card-body">
                    <h2 class="text-2xl font-semibold mb-4">Nos Coordonnées</h2>
                    <p class="mb-4 text-gray-600">
                        Vous pouvez également nous contacter par téléphone ou sur nos réseaux sociaux :
                    </p>

                    <ul class="space-y-3">
                        <li class="flex items-center gap-3">
                            <span class="badge badge-primary">📞</span>
                            <span>+33 6 12 34 56 78</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <span class="badge badge-primary">✉️</span>
                            <span>contact@mon-site.com</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <span class="badge badge-primary">🌐</span>
                            <a href="https://www.mon-site.com" class="link link-primary" target="_blank">
                                www.mon-site.com
                            </a>
                        </li>
                    </ul>

                    <div class="divider my-4">Réseaux Sociaux</div>

                    <div class="flex gap-4">
                        <a href="#" class="btn btn-circle btn-outline">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24"
                                fill="currentColor">
                                <path
                                    d="M22.46 6c-.77.35-1.6.58-2.46.69A4.2 4.2 0 0 0 21.9 4.4c-.8.47-1.68.8-2.62.98A4.18 4.18 0 0 0 16 4c-2.33 0-4.2 1.9-4.2 4.23 0 .33.03.65.1.95-3.49-.18-6.58-1.85-8.64-4.4a4.25 4.25 0 0 0-.57 2.13c0 1.47.73 2.77 1.84 3.53-.68-.02-1.32-.2-1.88-.52v.05c0 2.05 1.44 3.77 3.35 4.16-.35.1-.7.16-1.08.16-.26 0-.52-.03-.76-.07.53 1.65 2.06 2.85 3.87 2.89A8.39 8.39 0 0 1 2 19.54 11.85 11.85 0 0 0 8.29 21c7.55 0 11.68-6.32 11.68-11.8 0-.18 0-.36-.01-.53.8-.6 1.49-1.33 2.05-2.17z" />
                            </svg>
                        </a>
                        <a href="#" class="btn btn-circle btn-outline">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24"
                                fill="currentColor">
                                <path
                                    d="M19.5 3h-15A1.5 1.5 0 0 0 3 4.5v15A1.5 1.5 0 0 0 4.5 21h15a1.5 1.5 0 0 0 1.5-1.5v-15A1.5 1.5 0 0 0 19.5 3zM12 17.25c-2.9 0-5.25-2.35-5.25-5.25S9.1 6.75 12 6.75 17.25 9.1 17.25 12 14.9 17.25 12 17.25zM18 7.5a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0z" />
                            </svg>
                        </a>
                        <a href="#" class="btn btn-circle btn-outline">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 24 24"
                                fill="currentColor">
                                <path
                                    d="M22 12c0-5.52-4.48-10-10-10S2 6.48 2 12c0 4.99 3.66 9.12 8.44 9.88v-6.99h-2.54V12h2.54v-1.7c0-2.5 1.49-3.88 3.77-3.88 1.09 0 2.23.2 2.23.2v2.45h-1.26c-1.24 0-1.63.77-1.63 1.56V12h2.78l-.44 2.89h-2.34v6.99C18.34 21.12 22 16.99 22 12z" />
                            </svg>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'

// Data formulaire
const form = ref({
    nom: '',
    email: '',
    sujet: '',
    message: ''
})

// Méthode envoyer
function envoyerMessage() {
    // Ici tu peux gérer l’envoi réel (fetch, axios, etc.)
    alert(`Merci ${form.value.nom}, votre message a été envoyé !`)
    form.value = { nom: '', email: '', sujet: '', message: '' }
}
</script>

<style scoped>
/* DaisyUI gère déjà la plupart du style */
</style>