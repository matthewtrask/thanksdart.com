<script setup>
// defineProps({
//   msg: {
//     type: String,
//     required: true
//   }
// })
</script>

<template>
  <div>
    <div class="sm:block lg:flex">
      <div class="sm:w-full sm:block lg:w-6/12">
        <img class="w-full" src="../assets/dart/brady.png" alt="">
      </div>
      <div class="content-center mx-auto sm:w-full sm:block md:w-5/12 lg:w-4/12">
        <img src="../assets/dart/ride_easy-2.png" alt="">
      </div>
    </div>
    <div class="flex">
      <img class="w-full object-cover" src="../assets/dart/nationally-uncompetitive.jpg" alt="">
    </div>
    <div class="pt-10 pb-10">
      <div class="w-2/3 mx-auto">
        <h2 class="font-sans font-extrabold antialiased sm:text-1xl lg:text-3xl text-center drop-shadow-lg">The Dart Cycling Team was put together to find the fun in cycle racing. Started in Savannah, GA we have members across the United States. From Nashville, Tennessee to Washington, D.C. you can find someone in a Dart kit riding up front leading the group.</h2>
      </div>
    </div>
    <div class="pt-12 pb-12 bg-black" id="sponsors">
      <div class="w-2/3 mx-auto">
        <h2 class="font-sans text-white sm:text-3xl lg:text-5xl text-wide text-center drop-shadow-2xl uppercase font-bold">Sponsors</h2>
      </div>
    </div>
    <div class="flex">
      <div class="flex-initial mx-auto pt-8 pb-8">
        <a href="https://daddysdogsnash.com" target="_blank">
          <img class="mx-auto" src="../assets/dart/sponsors/daddy.png" alt="">
        </a>
      </div>
    </div>
    <div class="pt-12 pb-12 bg-black" id="team">
      <div class="w-2/3 mx-auto">
        <h2 class="font-sans text-white sm:text-3xl lg:text-5xl text-wide text-center drop-shadow-2xl uppercase font-bold">Team</h2>
      </div>
    </div>
    <div class="pt-10 pb-10">
      <div class="w-2/3 mx-auto">
        <div class="grid sm:grid-cols-1 sm:gap-1 lg:grid-cols-3 lg:gap-3">
          <div v-for="team in founders">
            <img :src="getPic(team.img)" v-bind:alt="team.name + ' image'" class="mx-auto h-32 w-32 rounded-full">
            <h4 class="text-center tracking-wider text-3xl pb-4">{{ team.name }}</h4>
            <p class="text-center tracking-wider font-bold pb-4 lg:h-16">{{ team.role }}</p>
            <div class="socials h-12 sm:mb-12">
              <div v-if="Object.keys(team.socials).length > 0">
                <a :href="team.socials.instagram">
                  <img class="sm:block h-10 w-auto justify-center mx-auto pb-4" src="../assets/instagram-brands.svg" alt="Workflow">
                </a>
              </div>
            </div>
         </div>
        </div> 
        <!-- <h2 class="font-sans font-extrabold antialiased sm:text-1xl lg:text-3xl text-center drop-shadow-lg"></h2> -->
      </div>
    </div>
    <div class="pt-10 pb-10">
      <div class="w-2/3 mx-auto">
        <div class="grid sm:grid-cols-2 sm:gap-2 sm:mb-12 lg:grid-cols-3 lg:gap-3">
          <div v-for="team in teamMembers" class=" pb-12">
            <img :src="getPic(team.img)" v-bind:alt="team.name + ' image'" class="mx-auto h-32 w-32 rounded-full">
            <h4 class="text-center tracking-wider text-3xl pb-4">{{ team.name }}</h4>
            <p class="text-center tracking-wider font-bold lg:h-12">{{ team.role }}</p>
            <div class="socials h-12 sm:mb-12">
              <div v-if="Object.keys(team.socials).length > 0">
                <a :href="team.socials.instagram" class="pb-12">
                  <img class="sm:block h-10 w-auto justify-center mx-auto pb-4" src="../assets/instagram-brands.svg" alt="Workflow">
                </a>
              </div>
            </div>
         </div>
        </div>
        <!-- <h2 class="font-sans font-extrabold antialiased sm:text-1xl lg:text-3xl text-center drop-shadow-lg"></h2> -->
      </div>
    </div>
    <div class="pt-10 pb-10">
      <div class="w-2/3 mx-auto">
        <div class="grid sm:grid-cols-2 sm:gap-2 lg:grid-cols-1 lg:gap-1">
          <a href="https://instagram.com/thanksdart/" target="_blank">
            <img class="sm:block h-36 w-auto justify-center mx-auto pb-4" src="../assets/dart/white-hash.png" alt="Workflow">
          </a>
        </div>
        <!-- <h2 class="font-sans font-extrabold antialiased sm:text-1xl lg:text-3xl text-center drop-shadow-lg"></h2> -->
      </div>
    </div>
  </div>
  
</template>
<script>
  export default {
    methods: {
      getPic(img) {
        return 'team/' + img;
      }
    },
    data() {
      return {
        founders: [
          {
            name: 'Gregg Cannon',
            role: 'Founder/Savannah Leader',
            bio: '',
            img: 'gregg.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/unprotected_rider/',
            }
          },
          {
            name: 'Sid Law',
            role: 'Founder',
            bio: '',
            img: 'sid.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/sidslaw/',
            }
          },
          {
            name: 'Petey Peters',
            role: 'Founder',
            bio: '',
            img: 'pete.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/ptp524/',
            }
          },
          {
            name: 'Tim Spackman',
            role: 'Founder',
            bio: '',
            img: 'tim.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/spackersss/',
            }
          },
          {
            name: 'JP Moncada',
            role: 'Founder/ Nashville Leader',
            bio: '',
            img: 'jp.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/jpmoncada/',
            },
          },
        ],
        teamMembers: [
          {
            name: 'Brady Whicker',
            role: 'Crit Racer',
            bio: '',
            img: 'brady.png',
            shavedLegs: true,
            socials: {}
          },
          {
            name: 'Aubrey Moore',
            role: 'Crit Racer | Stache Chief',
            bio: '',
            img: 'aubrey.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/bigaubreezy/',
            },
          },
          {
            name: 'Andrew Hodges',
            role: 'Crit Racer | Cross Racer | Mullet Grower',
            bio: '',
            shavedLegs: false,
            img: 'hodges.png',
            socials: {
              instagram: 'https://www.instagram.com/hodgeshodges/',
            }
          },
          {
            name: 'Safety Michael',
            role: 'Crit Racer | Cross Racer | Gravel Rider | Chief Safety Officer | Race Promoter',
            bio: '',
            img: 'safety.png',
            shavedLegs: false,
            socials: {
                instagram: 'https://www.instagram.com/___safetymichael/',
            }
          },
          {
            name: 'Taylor Long',
            role: 'Crit Racer | Washington, DC Dart Representative',
            bio: '',
            img: 'taylor.png',
            shavedLegs: false,
            socials: {
                instagram: 'https://www.instagram.com/greatfortacos/',
            }
          },
          {
            name: 'Aaron Conley',
            role: 'Crit Racer',
            bio: '',
            img: 'aaron.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/conleyaaron/',
            }
          },
          {
            name: 'Austin Bauman',
            role: 'Friend of the Team',
            bio: '',
            img: 'austin.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/greenfleet/',
            }
          },
          {
            name: 'Sarah Portella',
            role: 'Triathlete | Coach',
            img: 'sarah.png',
            shavedLegs: true,
            socials: {
                instagram: 'https://www.instagram.com/coachsarahportella/',
            }
          },
          {
            name: 'Herchel Portella',
            role: 'Cross Racer | West Wing Aficionado',
            bio: '',
            img: 'herchel.png',
            shavedLegs: false,
            socials: {
                instagram: 'https://www.instagram.com/herchelp/',
            }
          },
          {
            name: 'Bill Crump',
            role: 'Friend of the Team',
            bio: '',
            img: 'bill.png',
            shavedLegs: false,
            socials: {
              instagram: 'https://www.instagram.com/wlcrump/',
            }
          },

          {
            name: 'Heather Sutherland',
            role: 'Friend of the Team',
            bio: '',
            img: 'heather.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/heathersoutherland/',
            }
          },

          {
            name: 'Reid Bauman',
            role: 'Team Pilot | Stache Grower',
            bio: '',
            img: 'reid.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/wrbauman/',
            }
          },
          {
            name: 'Sam Crowell',
            role: 'Cross Racer',
            bio: '',
            img: 'sam.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/thesemirealscrowell/',
            }
          },
          {
            name: 'Mike Riello',
            role: 'Cross Racer',
            bio: '',
            img: 'mike.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/__mikejoe__/',
            }
          },
          {
            name: 'Shay Howe',
            role: 'Friend of the Team',
            bio: '',
            img: 'shay.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/shayhowe/',
            }
          },
          {
            name: 'Daddy',
            role: 'Team Chef | Hot Dog Slinger',
            bio: '',
            img: 'daddy.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/daddysdogsnash/',
            }
          },
        ]
      }
    }
  }
</script>

<style scoped>

</style>
