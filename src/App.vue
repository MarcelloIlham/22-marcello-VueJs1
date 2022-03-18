<template>
  <v-app>
    <v-main>
        <div class="mt-5">
            <p>===============================</p>
            <p>MARCELLO ILHAM | XII RPL B | 22</p>
            <p>===============================</p>
            <h1>Sekian dan Terima Gaji ^_^</h1>
        </div>

        <div class="container color mt-5">
            <div class="content" id="red" style="background-color: red;"></div>
            <div class="content" id="green" style="background-color: green;"></div>
            <div class="content" id="blue" style="background-color: blue;"></div>
            <div class="content" id="yellow" style="background-color: yellow;"></div>
            <div class="content" id="purple" style="background-color: purple;"></div>
            <div class="content" id="grey" style="background-color: grey;"></div>
        </div>
    </v-main>

    <v-footer padless>
      <v-col class="text-center" cols="12">
        {{ new Date().getFullYear() }} — <strong>vueJs1 - Fontend Fundamental</strong>
      </v-col>
    </v-footer>
  </v-app>
</template>

<script>

</script>

<style>
    .color {
        display: flex;
    }

    @media (max-width: 599px) {
        .content {
            padding: 100px;
            display: flex;
            flex: 100%;
        }
        .color {
            flex-direction: column;
        }
    }

    @media (min-width: 600px) and (max-width: 959px) {
        .content {
            height: 50px;
            display: flex; 
            flex: 50%;            
        }
        .color {
            flex-direction: row;
            flex-wrap: wrap;            
        }
    }

    @media (min-width: 960px) {
        .content {
            height: 50px;
            display: flex; 
            flex: 30%;            
        }
        .color {
            flex-direction: row;
            flex-wrap: wrap;            
        }
    }

    p , h1 {
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        text-align: center;
    }
</style>