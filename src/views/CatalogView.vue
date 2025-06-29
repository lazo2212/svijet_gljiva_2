<script setup lang="ts"></script>
<template>
  <main>
    <header>
      <h1>Katalog gljiva</h1>
      <p>
        U ovom katalogu možete pronaći informacije o različitim vrstama gljiva, uključujući njihove
        karakteristike, staništa i druge važne podatke.
      </p>
    </header>

    <section class="search-container">
      <input type="text" placeholder="Pretraži gljive..." />
      <button>Pretraži</button>
    </section>

    <section class="catalog-container">
      <article>
        <div class="main-img-container"></div>
        <div class="main-text-container">
          <h2>Vrganj</h2>
          <p>
            Vrganj je jestiva gljiva koja se često koristi u kulinarstvu. Ima karakterističan oblik
            i ukus, a može se naći u šumama širom sveta.
          </p>
        </div>
      </article>
    </section>
  </main>
</template>

<style scoped>
header {
  padding: 40px;
  text-align: center;
}

header h1 {
  font-size: 2.5em;
  margin-bottom: 10px;
}

.search-container {
  display: flex;
  justify-content: center;
  margin-bottom: 20px;
}

.search-container input {
  width: 600px;
  padding: 10px;
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;
  border: 1px solid #ccc;
}

.search-container button {
  padding: 10px 20px;
  border-top-right-radius: 5px;
  border-bottom-right-radius: 5px;
  border: none;
  background-color: forestgreen;
  color: white;
  cursor: pointer;
}
.catalog-container {
  border: 1px solid transparent;
  border-radius: 10px;
  transition: border 0.3s ease-in-out;
}
.catalog-container:hover {
  border: 1px solid #ccc;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  cursor: pointer;
}
.catalog-container a {
  text-decoration: none;
  color: inherit;
}
.catalog-container article {
  display: flex;
  height: 400px;
}
.catalog-container .main-img-container {
  width: 50%;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
  background-image: url('https://images.unsplash.com/photo-1727897707224-c9a1af98428f?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
  background-position: center;
  background-size: 100%;
  transition: background-size 0.3s ease-in-out;
}
.catalog-container:hover .main-img-container {
  background-size: 105%;
}
.catalog-container .main-text-container {
  width: 50%;
  padding: 20px;
}
.catalog-container .main-text-container h2 {
  font-size: 2em;
  margin-bottom: 10px;
}
.catalog-container .main-text-container p {
  font-size: 1.2em;
  margin-bottom: 20px;
}
</style>
