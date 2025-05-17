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
        <h2>Vrganj</h2>
        <img
          src="https://images.unsplash.com/photo-1727897707224-c9a1af98428f?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt=""
          width="400"
          height="auto"
        />
        <p>
          Pravi vrganj je jedna od najcjenjenijih jestivih gljiva. Klobuk mu je mesnat, promjera od
          8 do 25 cm, a može biti smećkast, kestenjast ili svijetlo smeđi. Površina klobuka je suha,
          glatka, a kod starijih primjeraka može biti lagano ispucana. Cjevčice su bijele kod mladih
          gljiva, a kasnije postaju žućkaste do maslinasto-zelene. Spore su maslinastosmeđe. Stručak
          je debeljuškast, valjkast ili bačvast, najčešće zadebljan pri dnu. Na površini ima
          karakterističnu bijelu mrežicu, osobito u gornjem dijelu stručka. Meso je bijelo, čvrsto,
          ugodnog mirisa i okusa, bez promjene boje pri oštećenju.
        </p>

        <h3>Stanište:</h3>
        <p>
          Vrganj raste u bjelogoričnim i crnogoričnim šumama, često ispod hrasta, bukve, kestena,
          ali i bora i smreke. Preferira kisela i humusna tla. Sezona rasta mu je od lipnja do
          listopada, ovisno o klimatskim uvjetima.
        </p>

        <h3>Jestivost:</h3>
        <p>
          Pravi vrganj je izvrsna jestiva gljiva, iznimno cijenjena u kulinarstvu. Koristi se svjež,
          sušen ili mariniran. Odličan je za juhe, umake, rižota i razna jela s mesom ili
          tjesteninom.
        </p>

        <h3>Slične vrste:</h3>
        <ul>
          <li>
            Ljetni vrganj (Boletus reticulatus) – sličan, ali mu klobuk često ima ispucalu površinu.
          </li>
          <li>vrganj (Boletus pinophilus) – tamnijeg klobuka, više vezan uz crnogoricu.</li>
          <li>Lažni vrganji (Tylopilus, Xerocomus) – neki su nejestivi ili slabije kvalitete.</li>
        </ul>

        <p>
          <b>Napomena:</b> Vrganj se lako može zamijeniti s nejestivim vrstama ako se ne pazi, stoga
          je preporučljivo brati ga samo ako ste sigurni u determinaciju.
        </p>
      </article>
    </section>
  </main>
</template>

<style scoped></style>
