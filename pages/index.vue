<template>
  <div class="container mt-5 sans-pro">
    <div class="d-flex flex-column justify-content-center align-items-center h-100">
      <div class="w-50">
        <img src="~/assets/images/man-3.png" alt="" class="img-fluid rounded-pill border border-dark p-1">
      </div>
      <br>
      <p>
        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-map-pin" width="24" height="24" viewBox="0 0 24 24" stroke-width="1" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
          <circle cx="12" cy="11" r="3"></circle>
          <path d="M17.657 16.657l-4.243 4.243a2 2 0 0 1 -2.827 0l-4.244 -4.243a8 8 0 1 1 11.314 0z"></path>
        </svg>
        KLATEN ID
      </p>
      <h4 class="lobster">Musyaffa El Rumi Shabib</h4>
      <a href="mailto:musyaffaelrumishabib@gmail.com" target="_blank" class="text-muted">musyaffaelrumishabib@gmail.com</a>

      <ul class="d-flex p-0 mt-3">
        <li>
          <a href="#" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-brand-facebook" width="24" height="24" viewBox="0 0 24 24" stroke-width="1" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
              <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
              <path d="M7 10v4h3v7h4v-7h3l1 -4h-4v-2a1 1 0 0 1 1 -1h3v-4h-3a5 5 0 0 0 -5 5v2h-3"></path>
            </svg>
          </a>
        </li>
        <li>
          <a href="#"  target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-mail" width="24" height="24" viewBox="0 0 24 24" stroke-width="1" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
              <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
              <rect x="3" y="5" width="18" height="14" rx="2"></rect>
              <polyline points="3 7 12 13 21 7"></polyline>
            </svg>
          </a>
        </li>
        <li>
          <a href="#" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-brand-twitter" width="24" height="24" viewBox="0 0 24 24" stroke-width="1" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
              <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
              <path d="M22 4.01c-1 .49 -1.98 .689 -3 .99c-1.121 -1.265 -2.783 -1.335 -4.38 -.737s-2.643 2.06 -2.62 3.737v1c-3.245 .083 -6.135 -1.395 -8 -4c0 0 -4.182 7.433 4 11c-1.872 1.247 -3.739 2.088 -6 2c3.308 1.803 6.913 2.423 10.034 1.517c3.58 -1.04 6.522 -3.723 7.651 -7.742a13.84 13.84 0 0 0 .497 -3.753c-.002 -.249 1.51 -2.772 1.818 -4.013z"></path>
            </svg>
          </a>
        </li>
        <li>
          <a href="https://www.instagram.com/elrumi.shabib" target="_blank">
          <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-brand-instagram" width="24" height="24" viewBox="0 0 24 24" stroke-width="1" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
            <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
            <rect x="4" y="4" width="16" height="16" rx="4"></rect>
            <circle cx="12" cy="12" r="3"></circle>
            <line x1="16.5" y1="7.5" x2="16.5" y2="7.501"></line>
          </svg>
          </a>
        </li>
        <li>
          <a href="https://shabib.my.id" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-world" width="24" height="24" viewBox="0 0 24 24" stroke-width="1" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
              <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>
              <circle cx="12" cy="12" r="9"></circle>
              <line x1="3.6" y1="9" x2="20.4" y2="9"></line>
              <line x1="3.6" y1="15" x2="20.4" y2="15"></line>
              <path d="M11.5 3a17 17 0 0 0 0 18"></path>
              <path d="M12.5 3a17 17 0 0 1 0 18"></path>
            </svg>
          </a>
        </li>
      </ul>
      <div>
        I was born {{$moment(this.born, "YYYYMMDD").fromNow()}}
      </div>
      <hr class="border border-dark w-25">

      <div class="row mt-5">
        <div class="col-6">
          <Mom/>
        </div>
        <div class="col-6">
          <Dad/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>


import Mom from "../components/Mom";
import Dad from "../components/Dad";
export default {
  name: 'IndexPage',
  components: {Dad, Mom},
  head:{
    title: "Shabib",
    meta:[
      { name: 'theme-color', content: '#3498db' },
    ],
    link:[
      {
        rel:"stylesheet",
        href:"https://fonts.googleapis.com/css2?family=Lobster&display=swap"
      },
      {
        rel:"stylesheet",
        href:"https://fonts.googleapis.com/css2?family=Source+Sans+Pro&display=swap"
      }
    ]
  },
  data(){
    return{
      born:"20220302"
    }
  }
}
</script>

<style scoped>
li{
  list-style-type: none;
  margin: 0 1em;
}

.lobster{
  font-family: 'Lobster', cursive;
}
.sans-pro{
  font-family: 'Source Sans Pro', sans-serif;
}
@media only screen and (min-width: 767px) {
  .container{
    width: 25% !important;
  }
}


</style>
