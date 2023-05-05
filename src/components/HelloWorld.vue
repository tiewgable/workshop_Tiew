<template>
<div>
   <br /><br />
   <v-btn
      block
      elevation="2"
      x-large 
   ><card>Profile</card></v-btn>
   <br /><br />
   <h1>Natthapol Imphong</h1>
   <br /><br />
   <v-card
  elevation="2"
  outlined
  shaped
></v-card>
   <h3>การศึกษา</h3>
   <br />
   <template>
  <v-carousel hide-delimiters>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>
   <br /><br />

   <h4>มัธยมต้น : โรงเรียนสตรีสมุทรปราการ</h4>
   <h4>ปวช. : Samtech</h4>
   <h4>ปัจจุบันกำลังศึกษาที่ : มหาวิทยาลัยเทคโนโลยีราชมงคลธัญบุรี</h4>
   <br /><br />

<template>
  <v-footer
    color="primary lighten-1"
    padless
  >
    <v-row
      justify="center"
      no-gutters
    >
      <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link }}
      </v-btn>
      <v-col
        class="primary lighten-2 py-4 text-center white--text"
        cols="12"
      >
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>

</div>
</template>

<script>
export default {
   name: 'HelloWorld',

   data: () => ({
      
   })
}
</script>

<script>
  export default {
    data: () => ({
      links: [
        'Home',
        'Contact',
        'Project',
      ],
    }),
  }
</script>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://www.chulatutor.com/blog/wp-content/uploads/2020/04/exam-streesmutprakan-school.jpg',
          },
          {
            src: 'https://samtech.ac.th/wp-content/uploads/2021/05/cropped-cropped-%E0%B8%9B%E0%B8%8101-1-scaled-1.jpg',
          },
          {
            src: 'https://klonghok.go.th/public/list_upload/backend/list_511/pics_topic_511.jpg',
          }
        ],
      }
    },
  }
</script>