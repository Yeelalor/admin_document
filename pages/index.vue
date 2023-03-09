<template>
  <div class="bgs">
    <v-row class="bgs" align="center">
      <v-col>
        <div class="text-center pb-4">
          <img class="mx-auto" src="../assets/images/logo.png" width="60" />
          <h3 class="white--text">LDB</h3>
        </div>
        <v-card width="400" class="mx-auto bgs" elevation="0" height="300">
          <div class="text-center white--text pt-6 font-weight-bold">
            ເຂົ້າສູ່ລະບົບ
          </div>
          <v-card-text>
            <v-text-field
              label="ຊື່ຜູ້ໃຊ້"
              prepend-icon="mdi-account"
              v-model="userName"
              color="white"
              dark
              
            ></v-text-field>
            <v-text-field
              label="ລະຫັດຜ່ານ"
              :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
              prepend-icon="mdi-lock"
              v-model="password"
              :type="showPassword ? 'text' : 'password'"
              @click:append="onShowpassword"
              @keyup.enter="onLogin"
              dark
              color="white"
            ></v-text-field>
            <div class="text-center">
              <v-btn
              v-if="loadingLogin"
              color="primary"
              class="mt-5"
            >
              <v-progress-circular
                :width="2"
                color="white"
                indeterminate
              ></v-progress-circular>

              <span class="ml-2">ກຳລັງເຂົ້າສູ່ລະບົບ...</span>
            </v-btn>
            <v-btn
              elevation="0"
              v-else
              color="white"
              class="mt-5"
              @click="onLogin"
            >
              ເຂົ້າສູ່ລະບົບ
            </v-btn>
            </div>
           
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>
<script>
// import swal from 'sweetalert2'
export default {
  layout: 'blank',
  data() {
    return {
      showPassword: false,
      userName: '',
      password: '',
      loadingLogin: false,
    }
  },
  methods: {
    onShowpassword() {
      this.showPassword = !this.showPassword
    },
    async onLogin() {
      this.$router.push('/contract_type')
      //   try {
      //     if (this.userName != '' && this.password != '') {
      //       let data = {
      //         user: this.userName,
      //         password: this.password,
      //       }
      //       this.loadingLogin = true
      //       await this.$axios.$post('Login', data).then((data) => {
      //         if (data?.status == '00') {
      //           console.log(data)
      //           localStorage.setItem('USER_ID', data?.data?.staftId)
      //           localStorage.setItem('USER_NAME', data?.data?.staftName)
      //           localStorage.setItem('USER_ROLE', data?.data?.role)
      //           this.loadingLogin = false
      //           this.$router.push('/customer')
      //         } else {
      //           this.loadingLogin = false
      //           swal.fire({
      //             title: 'ແຈ້ງເຕືອນ',
      //             text: data?.message,
      //             icon: 'error',
      //             allowOutsideClick: false,
      //             confirmButtonColor: '#3085d6',
      //             confirmButtonText: 'OK',
      //           })
      //         }
      //       })
      //     }
      //   } catch (error) {
      //     this.loadingLogin = false
      //     swal.fire({
      //       title: 'ແຈ້ງເຕືອນ',
      //       text: error,
      //       icon: 'error',
      //       allowOutsideClick: false,
      //       confirmButtonColor: '#3085d6',
      //       confirmButtonText: 'OK',
      //     })
      //   }
    },
  },
}
</script>
<style scoped>
.bg {
  background-color: #3992c8;
}
.bgs {
  background: linear-gradient(#3c98ce, #2171a1, #144d70);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  height: 100vh;
}
</style>
