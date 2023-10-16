<script lang="ts">
import tasks from "./assets/tasks.json";

export default {
  name: "App",

  methods: {
    // Erstellen Sie eine Methode "addTask", die eine neue Aufgabe hinzufügt
    // Erstellen Sie eine Methode "toggleTask", die eine Aufgabe öffnet oder schließt
  },

  computed: {
    // Erstellen Sie eine computed property "openTasks", die alle offenen Aufgaben zurückgibt
    // Erstellen Sie eine computed property "closedTasks", die alle geschlossenen Aufgaben zurückgibt
  }
  
}
</script>

<template>
  <div class="bg-gray-100 overflow-hidden min-h-screen">
    
    <header class="bg-gray-800 p-8">
      <div class="md:flex md:items-center md:justify-between">
        <div class="min-w-0 flex-1">
          <h2 class="text-2xl font-bold leading-7 text-white sm:truncate sm:text-3xl sm:tracking-tight app-title">vue3-grundkurs</h2>
        </div>
      </div>
    </header>

    <main class="mx-auto max-w-3xl px-4 py-4 sm:px-6 sm:py-6 lg:max-w-7xl lg:px-8 lg:py-8">
      
      <div class="grid grid-cols-1 items-start gap-4 lg:grid-cols-2 lg:gap-8">


        <div class="grid grid-cols-1 gap-4">

          <div class="border-b border-gray-200 bg-white px-4 py-5 sm:px-6 sm:rounded-lg sm:shadow">
            <div class="-ml-4 -mt-2 flex flex-wrap items-center justify-between sm:flex-nowrap">
              <div class="ml-4 mt-2">
                <h3 class="text-lg font-medium leading-6 text-gray-900">Offene Aufgaben</h3>
              </div>
              <div class="ml-4 mt-2 flex-shrink-0">
                <button id="newTask" type="button" class="relative inline-flex items-center rounded-md border border-transparent bg-indigo-600 px-4 py-2 text-sm font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2">Neue Aufgabe</button>
              </div>
            </div>
          </div>

          <div>Geben Sie hier die offenen Aufgaben aus</div>

        </div>


        <div class="grid grid-cols-1 gap-4">
          
          <div class="border-b border-gray-200 bg-white px-4 py-5 sm:px-6 sm:rounded-lg sm:shadow">
            <div class="-ml-4 -mt-2 flex flex-wrap items-center justify-between sm:flex-nowrap">
              <div class="ml-4 mt-2">
                <h3 class="text-lg font-medium leading-6 text-gray-900">Geschlossene Aufgaben</h3>
              </div>
            </div>
          </div>

          <div>Geben Sie hier die fertiggestellten Aufgaben aus</div>

        </div>

      </div>

    </main>

  </div>
</template>

<style scoped>
</style>
