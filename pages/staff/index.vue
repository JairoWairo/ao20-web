<template>
  <div class="container">
    <section>
        <br>
        <br>
        <h1 class="section-title text-center mb-4 uppercase">Nosotros</h1>
        <h2>Staff de Argentum 20</h2>
        <h3>Líderes de Proyecto</h3>
        <p>
            «Gulfas Morgolock»<br>
            Horacio Garofalo «Haracin»<br>
            Alejandro Cordara «Animal»
        </p>
        <h3>Líder de Programación</h3>
        <p>
            «Gulfas Morgolock»<br>
        </p>
        <h3>Programación</h3>
        <p>
            Lucas Recoaro «RecoX»<br>
            Matias Calegaris «Tute»
        </p>
        <h3>Desarrollo de Herramientas</h3>
        <p>
            «ReyarB»
        </p>
        <h3>Diseño y Arte Gráfico</h3>
        <p>
            Alejandro Cordara «Animal»
        </p>
        <h3>Indexación</h3>
        <p>
            «ReyarB»
        </p>
        <h3>Mapeo</h3>
        <p>
            Horacio Garofalo «Haracin»<br>
            «ReyarB»
        </p>
        <h3>Diseño y Desarrollo Web</h3>
        <p>
            Lucas Recoaro «RecoX»<br>
            Alejandro Cordara «Animal»
        </p>
        <h3>Arquitecto DevOps</h3>
        <p>
            Lucas Recoaro «RecoX»
        </p>
        <h3>Musicalización</h3>
        <p>
            Jorge Gabriel Leni «Sonic»
        </p>
        <h3>Lider soporte y Game Masters</h3>
        <p>
            «ReyarB»
        </p>
        <h3>Game Masters</h3>
        <p>
        </p>
        <h3>Moderación de Comunidad</h3>
        <p>
        </p>
        <h3>Wiki</h3>
        <p>
            Lucas Recoaro «RecoX»<br>
            Alejandro Cordara «Animal»
        </p>

    </section>

    <div class="section-divider my-8"></div>

    <section>

        <h2>Proyecto Argentum Online en SourceForge</h2>
        <p>Argentum20 está basado en el juego Argentum Online original: <a href="https://sourceforge.net/projects/morgoao/" rel="noopener" target="_blank" class="text-primary underline">https://sourceforge.net/projects/morgoao/</a>.</p>
        <p>Mucha gente ha colaborado a este proyecto y si considerás que aportaste de alguna manera a la creación de AO20 por favor contactanos así te agregamos en la sección de créditos.</p>
        <p>Para ver los créditos del AO original, <a href="/aostaff.txt" target="_blank" class="text-primary underline">ingrese aquí.</a></p>

    </section>

    <div class="section-divider my-8"></div>

    <section class="agradecimientos">

        <h2>Agradecimientos Especiales</h2>
        <p>A Alexis Caraballo «WyroX» por su dedicación y aporte de conocimientos que ayudaron a que Argentum 20 sea lo que es hoy en día.</p>
        <p>A todos los ex miembros que cumplieron un rol dentro del staff cuyo trabajo fue muy importante para poder sacar adelante este proyecto:</p>
        <ul>
            <li>A Pablo Mercavides «Ladder» y a su staff de Revolución AO por ceder los códigos originales de servidor y cliente los cuales fueron tomados de base para encarar Argentum 20.</li>
            <li>Xavier Viger Navarro «Sensui» (Idea original, Mapeo, Dateo, Game Design)</li>
            <li>Sergio Perez «Neosefirot» (Idea original y Coordinación)</li>
            <li>Bruno De Angelis «SimP» (Diseño y desarrollo web)</li>
            <li>Martín Trionfetti «HarThaoS» (Programación)</li>
            <li>Fernando Quinteros «Lord Fers» (Programación)</li>
            <li>Joaquín Ortíz «Jopi» (Programación)</li>
            <li>Emiliano Mancuso «Emancu» (Programación)</li>
            <li>Agustín Pagani «Daylight» (Balance y armado de NPC)</li>
            <li>Brian «About» (Programación)</li>
            <li>Gabriel Aulicino «Ruthnar» (Programación)</li>
            <li>Lucho «VanCleff» (Balance)</li>
            <li>Sebastián Avena «Linqen» (Balance)</li>
            <li>Nicolás «Aikhio» (Redes Sociales)</li>
            <li>Erik Eleusippi «Ronin» (Balance y Mapeo)</li>
            <li>Alejo «Centorios» (Programación)</li>
            <li>Joaquín Ortíz «Jopi» (Programación)</li>
        </ul>
        <p class="italic">(No recordamos los apellidos de todos, si alguno quiere figurar con su apellido por favor contactarse con el staff)</p>

    </section>

    <div class="section-divider my-8"></div>

    <section>
        <p>Agradecemos al portal <a href="https://sketchfab.com/" target="_blank" class="text-primary underline">SketchFab.com</a> por los <a  class="text-primary underline" href="/staff/recursos-de-terceros" title="Recursos de terceros">recursos gratuitos</a> que utilizamos en algunos de nuestros gráficos.</p>
    </section>

  </div>
</template>

<script>
export default {};
</script>

<style>
    h2, h3, p {
        @apply text-center;
    }

    h2 {
        @apply uppercase text-3xl mb-4;
    }
    h3 {
        @apply text-3xl text-primary mb-4;
    }
    p {
        @apply text-xl mb-6;
    }

    .agradecimientos ul {
        @apply mx-16 list-disc mb-6;
    }

    .agradecimientos ul li {
        @apply mb-2 text-xl;
    }


</style>
