<template>
  <div class="container">
    <div
      v-if="rankingGuilds.length"
      class="bg-gray-900 border-2 border-gr border-gr-primary"
    >
      <h1>Ranking Clanes</h1>
      <div class="xl:col-span-10 text-xs overflow-x-auto">
        <table class="text-gray-400">
          <thead>
            <tr>
              <th>Nombre</th>
              <th>Fundador</th>
              <th>Fecha Creacion</th>
              <th>Alineacion</th>
              <th>Ultimas Elecciones</th>
              <th>Descripcion</th>
              <th>Novedades</th>
              <th>Lider</th>
              <th>Nivel</th>
              <th>Miembros</th>
              <th>Cantidad Miembros</th>
              <th>Cantidad Solicitudes para Ingreso</th>
              <!-- <th>Oro total de todos los miembros</th> -->
            </tr>
          </thead>

          <tbody>
            <tr v-for="guild in rankingGuilds" :key="guild.item_id">
              <td class="text-right">{{ guild.GuildName }}</td>
              <td class="text-right">{{ guild.Founder }}</td>
              <td class="text-right">{{ guild.Date }}</td>
              <td class="text-right">{{ guild.Alineacion }}</td>
              <td class="text-right">{{ guild.UltimasElecciones }}</td>
              <td class="text-right">{{ guild.Desc }}</td>
              <td class="text-right">{{ guild.GuildNews }}</td>
              <td class="text-right">{{ guild.Leader }}</td>
              <td class="text-right">{{ guild.NivelDeClan }}</td>
              <td class="text-right">{{ guild.MEMBERS }}</td>
              <td class="text-right">{{ guild.QTY_MEMBERS }}</td>
              <td class="text-right">{{ guild.QTY_SOLICITUDES_INGRESO }}</td>
              <!-- <td class="text-right">{{ guild.TOTAL_GOLD_FROM_MEMBERS }}</td> -->
            </tr>
          </tbody>
        </table>
      </div>
    </div>
    <section v-else class="text-center mt-24">
      <p class="text-2xl">Cargando Ranking Clanes.</p>
      <p class="text-l">Por favor se paciente, esta pagina puede tardar varios minutos en cargar...</p>
    </section>
  </div>
</template>

<script>

export default {
  data() {
    return {
      rankingGuilds: [],
    };
  },
  async fetch() {
    this.rankingGuilds = await this.$axios.$get("https://api-staging.ao20.com.ar:11812/guilds/getAll");
  },
  head() {
    return {
      title: "Ranking - Clanes",
    };
  },
};
</script>

<style>

select:required:invalid {
  color: gray;
}

option[value=""][disabled] {
  display: none;
}

td {
  @apply bg-gray-900 p-4 border border-gray-200;
}

</style>
