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
      <div class="w-2/3 mx-auto pb-12">
        <h2 class="font-sans font-extrabold antialiased sm:text-1xl lg:text-3xl text-center drop-shadow-lg">The Dart Cycling Team was put together to find the fun in cycle racing. Started in Savannah, GA we have members across the United States. From Nashville, Tennessee to Washington, D.C. you can find someone in a Dart kit riding up front leading the group.</h2>
      </div>
      <div class="w-2/3 mx-auto pb-12">
        <div class="socials h-12 sm:mb-12 flex justify-center pb-12">
          <a href="https://instagram.com/thanksdart" class="pb-12">
            <img class="sm:block h-24 w-auto mx-auto pr-12" src="../assets/instagram-brands.svg" alt="Dart Instagram Account">
          </a>
          <a href="https://www.strava.com/clubs/dartcycle" class="pb-12">
            <img class="sm:block h-24 w-auto mx-auto pl-12" src="../assets/strava-brands.svg" alt="Dart Strava Club">
          </a>
        </div>
      </div>
      <div class="w-2/3 mx-auto">
        <h2 class="pb-12 font-sans font-extrabold antialiased sm:text-1xl lg:text-3xl text-center drop-shadow-lg">Want to join us? Or have a question? Maybe just want to say hi?</h2>
        <div class="rounded-md bg-green-50 p-4 max-w-md" v-if="showSuccess">
          <div class="flex">
            <div class="flex-shrink-0">
              <!-- Heroicon name: solid/check-circle -->
              <svg class="h-5 w-5 text-green-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
              </svg>
            </div>
            <div class="ml-3">
              <p class="text-sm font-medium text-green-800">Successfully uploaded</p>
            </div>
            <div class="ml-auto pl-3">
              <div class="-mx-1.5 -my-1.5">
                <button type="button" class="inline-flex bg-green-50 rounded-md p-1.5 text-green-500 hover:bg-green-100 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-green-50 focus:ring-green-600">
                  <span class="sr-only">Dismiss</span>
                  <!-- Heroicon name: solid/x -->
                  <svg class="h-5 w-5" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                    <path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd" />
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="block p-6 rounded-lg shadow-lg bg-white max-w-md mx-auto">

          <form action="https://fieldgoal.io/f/11Vje9" method="POST">
            <div class="form-group mb-6">
              <input type="text" class="form-control block
        w-full
        px-3
        py-1.5
        text-base
        font-normal
        text-gray-700
        bg-white bg-clip-padding
        border border-solid border-gray-300
        rounded
        transition
        ease-in-out
        m-0
                focus:text-gray-700 focus:bg-white focus:border-yellow-500 focus:outline-none
" id="exampleInput7"
                     placeholder="Name" name="name">
            </div>
            <div class="form-group mb-6">
              <input type="email" class="form-control block
        w-full
        px-3
        py-1.5
        text-base
        font-normal
        text-gray-700
        bg-white bg-clip-padding
        border border-solid border-gray-300
        rounded
        transition
        ease-in-out
        m-0
                focus:text-gray-700 focus:bg-white focus:border-yellow-500 focus:outline-none
" id="exampleInput8"
                     placeholder="Email address" name="email">
            </div>
            <div class="form-group mb-6">
      <textarea class="form-control block w-full px-3 py-1.5
        text-base
        font-normal
        text-gray-700
        bg-white bg-clip-padding
        border border-solid border-gray-300
        rounded
        transition
        ease-in-out
        m-0
        focus:text-black focus:bg-white focus:border-yellow-500 focus:outline-none
      "
          id="exampleFormControlTextarea13"
          rows="3"
          placeholder="Message"
                name="message"
      ></textarea>
            </div>
            <button type="submit" class="
      w-full
      px-6
      py-2.5
      daddy-yellow
      text-white
      font-medium
      text-xs
      leading-tight
      uppercase
      rounded
      shadow-md
      hover:bg-yellow-700 hover:shadow-lg
      focus:bg-yellow-700 focus:shadow-lg focus:outline-none focus:ring-0
      active:bg-yellow-800 active:shadow-lg
      transition
      duration-150
      ease-in-out"
            @click="sendForm()">Send</button>
          </form>
        </div>

      </div>
    </div>
    <div class="pt-12 pb-12 bg-black" id="sponsors">
      <div class="w-2/3 mx-auto">
        <h2 class="font-sans text-white text-5xl text-wide text-center drop-shadow-2xl uppercase font-bold">Sponsors</h2>
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
        <h2 class="font-sans text-white text-5xl text-wide text-center drop-shadow-2xl uppercase font-bold">Team</h2>
      </div>
    </div>
    <div class="pt-10 pb-10">
      <div class="w-2/3 mx-auto">
        <div class="grid sm:grid-cols-2 sm:gap-2 sm:mb-12  lg:grid-flow-col lg:auto-cols-fr">
          <div v-for="team in founders">
            <img :src="getPic(team.img)" v-bind:alt="team.name + ' image'" class="mx-auto h-32 w-32 rounded-full">
            <h4 class="text-center tracking-wider text-3xl pb-4">{{ team.name }}</h4>
            <p class="text-center tracking-wider font-bold lg:h-12">{{ team.role }}</p>
            <div class="socials h-12 sm:mb-12 flex justify-center">
              <div v-if="Object.keys(team.socials).length > 0">
                <a :href="team.socials.instagram" class="pb-12 inline-block pr-4" v-if="team.socials.instagram">
                  <img class="sm:block h-10 w-auto mx-auto pb-4" src="../assets/instagram-brands.svg" :alt="team.name + 'Instagram'">
                </a>
                <a :href="team.socials.strava" class="pb-12 inline-block pl-4"  v-if="team.socials.strava">
                  <img class="sm:block h-10 w-auto mx-auto pb-4 text-orange-500	" src="../assets/strava-brands.svg" :alt="team.name + 'Strava'">
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
        <div class="grid sm:grid-cols-2 sm:gap-2 sm:mb-12 lg:grid-cols-3 lg:gap-3 lg:auto-cols-max">
          <div v-for="team in teamMembers" class=" pb-12">
            <img :src="getPic(team.img)" v-bind:alt="team.name + ' image'" class="mx-auto h-32 w-32 rounded-full">
            <h4 class="text-center tracking-wider text-3xl pb-4">{{ team.name }}</h4>
            <p class="text-center tracking-wider font-bold lg:h-12">{{ team.role }}</p>
            <div class="socials h-12 sm:mb-12 flex justify-center">
              <div v-if="Object.keys(team.socials).length > 0">
                <a :href="team.socials.instagram" class="pb-12 inline-block pr-4" v-if="team.socials.instagram">
                  <img class="sm:block h-10 w-auto mx-auto pb-4" src="../assets/instagram-brands.svg" :alt="team.name + 'Instagram'">
                </a>
                <a :href="team.socials.strava" class="pb-12 inline-block pl-4"  v-if="team.socials.strava">
                  <img class="sm:block h-10 w-auto mx-auto pb-4 text-orange-500	" src="../assets/strava-brands.svg" :alt="team.name + 'Strava'">
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
      },

      sendForm() {
        this.showSuccess = true;
      }
    },
    data() {
      return {
        showSuccess: false,
        founders: [
          {
            name: 'Gregg Gannon',
            role: 'Founder/Savannah Leader',
            bio: '',
            img: 'gregg.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/unprotected_rider/',
              strava: 'https://www.strava.com/athletes/1076514',
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
              strava: 'https://www.strava.com/athletes/6468363',
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
              strava: null,
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
              strava: 'https://www.strava.com/athletes/996894',
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
              strava: 'https://www.strava.com/athletes/3110564',
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
            socials: {
              strava: 'https://www.strava.com/athletes/15450549',
            }
          },
          {
            name: 'Aubrey Moore',
            role: 'Crit Racer | Stache Chief',
            bio: '',
            img: 'aubrey.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/bigaubreezy/',
              strava: 'https://www.strava.com/athletes/1407085',
            },
          },
          {
            name: 'Anders Folgar',
            role: 'Friend of the Team',
            bio: '',
            img: 'anders.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/bigaubreezy/',
              strava: 'https://www.strava.com/athletes/1407085',
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
              strava: 'https://www.strava.com/athletes/1046112',
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
              strava: 'https://www.strava.com/athletes/2471926',
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
              strava: 'https://www.strava.com/athletes/22762389'
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
              strava: 'https://www.strava.com/athletes/402999',
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
              strava: 'https://www.strava.com/athletes/3187605',
            }
          },
          {
            name: 'Sarah Portella',
            role: 'Triathlete | Coach',
            img: 'sarah.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/coachsarahportella/',
              strava: 'https://www.strava.com/athletes/4494379',
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
              strava: 'https://www.strava.com/athletes/387523',
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
              strava: 'https://www.strava.com/athletes/8192',
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
              strava: 'https://www.strava.com/athletes/34434567',
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
              strava: 'https://www.strava.com/athletes/18045066',
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
              strava: 'https://www.strava.com/athletes/7129270',
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
              strava: 'https://www.strava.com/athletes/8192',
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
              strava: 'https://www.strava.com/athletes/8989985',
            }
          },
          {
            name: 'Michael Ringer',
            role: 'Crit Racer',
            bio: '',
            img: 'michael.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/ringading16/',
              strava: 'https://www.strava.com/athletes/6636930?oq=rin',
            }
          },
          {
            name: 'Chris Stephens',
            role: 'Friend of the Team',
            bio: '',
            img: 'chris.png',
            shavedLegs: true,
            socials: {
              instagram: 'https://www.instagram.com/stephensc4/',
              strava: 'https://www.strava.com/athletes/9566038',
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
  .daddy-yellow {
    background-color: rgb(255,223,74)
  }
</style>
