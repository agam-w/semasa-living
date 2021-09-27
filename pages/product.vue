<template>
  <v-container>
    <h1 class="mb-14">Products</h1>
    <v-row>
      <v-col
        v-for="n in images"
        :key="n.price"
        class="d-flex child-flex"
        cols="6"
        sm="4"
        md="3"
      >
        <v-img
          :src="`https://drive.google.com/uc?export=view&id=${n.id}`"
          :lazy-src="`https://picsum.photos/10/6?image=${30}`"
          aspect-ratio="1"
          class="grey lighten-2"
        >
          <template #placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular
                indeterminate
                color="grey lighten-5"
              ></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
    <h3 class="text-center pt-6" style="color: #27cfb1">Show More</h3>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      imagesRow: 4,
      images: [
        {
          id: '1mtxCiG-Hyb_x6w9JGKPHOr2GzFe4l6p6',
          name: '',
          price: 1,
        },
        {
          id: '18nj8PF9ogdUw__Rsz7bEkbZFNKpEo1-5',
          name: '',
          price: 2,
        },
        {
          id: '155FmqWgBD0DEpTSHQndbH6NjljrkMLcd',
          name: '',
          price: 3,
        },
        {
          id: '1ISxSmd_HVjnODvs4ZP7agUwXPWNHRyIs',
          name: '',
          price: 4,
        },
        {
          id: '135_tfLLdVI8KmDsRy6gpTHMpMxMUYsPr',
          name: '',
          price: 5,
        },
        {
          id: '1bu0RV2RNTA0S02sYPhZXLe16oSQaY2PF',
          name: '',
          price: 6,
        },
        {
          id: '1I0bFQep4DHZjl8-4eJ5HHDZS_bGHe0aP',
          name: '',
          price: 7,
        },
        {
          id: '1ziG1jSo94BLce28Z5GTvcqSZxu0ACW4U',
          name: '',
          price: 8,
        },
        {
          id: '1r9cmmU-fScFMisGAlz1TqmmVNZYMU9xR',
          name: '',
          price: 9,
        },
        {
          id: '11iTit_QkM3CF4JD1WDap7a8R0GuWpATL',
          name: '',
          price: 10,
        },
        {
          id: '1C9oM6hOqQTwFCvJR-XmIgRbUmhAj_HK1',
          name: '',
          price: 11,
        },
        {
          id: '1wYRBdNfspZCv8z38JlMLnYbT2z6ykYvj',
          name: '',
          price: 12,
        },
        {
          id: '10T3XCTFPD8WlEhmYM5HWnpYzpLJlW9sB',
          name: '',
          price: 13,
        },
        {
          id: '1dubAGcOF208yKc0pnd22ZpaY2071TK82',
          name: '',
          price: 14,
        },
        {
          id: '1HpJRKppo9k2z34L_8H3F_C_HPiWxderQ',
          name: '',
          price: 15,
        },
        {
          id: '1HRGLQ7lRkpOUBaunt5vaVL4wHhZJF0SW',
          name: '',
          price: 16,
        },
        {
          id: '1zcQuBgBHVH687ZCm4M12F5E9AEJhj9hB',
          name: '',
          price: 17,
        },
        {
          id: '1dO6ec4oDyZj86e9tIqzCe66eMLCl1X1n',
          name: '',
          price: 18,
        },
        {
          id: '1Akd6r5DKpLdfv9GimGQNrUjqidqES9e2',
          name: '',
          price: 19,
        },
        {
          id: '1EWy2CN4vONjlbtdLbwN6SNItdwFTfaFc',
          name: '',
          price: 20,
        },
        {
          id: '1m95-G0RFx0ryCIZ1J0d7eUEXSu12w9YN',
          name: '',
          price: 21,
        },
        {
          id: '1SuLkdMVXXroSxcqn6p_Yvub5tpvwC0_P',
          name: '',
          price: 22,
        },
        {
          id: '1mcgIEphysZpQMAOaasi1YwthAO7sUsL4',
          name: '',
          price: 23,
        },
        {
          id: '16m2V17ydCHs-bYOR8U9Pl2WCNFjO-6Wb',
          name: '',
          price: 24,
        },
        {
          id: '1MUDedg-T0OFLksapTzrnNJYFqp0Tc7D_',
          name: '',
          price: 25,
        },
        {
          id: '14a-bASsZr7Rx9KdcOSO-xk9OtPYcDDDL',
          name: '',
          price: 26,
        },
        {
          id: '1V-HoQ1iDlIutL3xNSuMkPVLgRCj5Fmbg',
          name: '',
          price: 27,
        },
        {
          id: '1OLhR-oep_fyHXA9X2W8LEEgkm7JPWWL0',
          name: '',
          price: 28,
        },
        {
          id: '1zn_p5bCoimYwHgVnDyZtgXneCtIjsQY-',
          name: '',
          price: 29,
        },
        {
          id: '1Hizxc90bNBIj-o-vbXRspoAufgBlA5Ys',
          name: '',
          price: 30,
        },
        {
          id: '1FOONCRyL63ZPxJRmgeVR_SAhxw0hfd5C',
          name: '',
          price: 31,
        },
        {
          id: '1r5yd-1rEprecQEiK-OFqNCwsJZnfA-3p',
          name: '',
          price: 32,
        },
        {
          id: '1V-m9hnjLVLCwXtykn-XCvoaDqLDGX7yj',
          name: '',
          price: 33,
        },
        {
          id: '1Lo0OMCWZwkwKj5eP0S25c885UG2RTH47',
          name: '',
          price: 34,
        },
        {
          id: '11uMYnd4oCHjJJGAvSUrckoGeAA9mT5gM',
          name: '',
          price: 35,
        },
        {
          id: '1GBIPqye8e4gqEOw-W_2q6YQD0AUSP3-j',
          name: '',
          price: 36,
        },
        {
          id: '1DqzN3Nt-sLNq9f0Z0H-EtbCTBx04a1fX',
          name: '',
          price: 37,
        },
        {
          id: '1UbyAZGSx4vzWV0kpJm-AZupPsCFMc_-h',
          name: '',
          price: 38,
        },
        {
          id: '1J4Asr0Dg3k_W4IiL1slY7i3z_f1k6V_B',
          name: '',
          price: 39,
        },
        {
          id: '1D4yCiFzAfHNhYMRHWIsW-Xg99TgIP0BE',
          name: '',
          price: 40,
        },
        {
          id: '1cbbZ0VhZ7TJgq-rSlRFqvydmFBibay5O',
          name: '',
          price: 41,
        },
        {
          id: '10p2KeTkL3VNlUYwV2ax3GyB2PLov0ThB',
          name: '',
          price: 42,
        },
        {
          id: '1Foj3219EXENF13NwTQdMTkck_Trva9Bp',
          name: '',
          price: 43,
        },
        {
          id: '1IYzHqNMlBYzl_7Anoy-UyUilL8EbEP5J',
          name: '',
          price: 44,
        },
        {
          id: '1Jj7M6i4PsmLaqHEhs3Zix0hO9K29aOMr',
          name: '',
          price: 45,
        },
        {
          id: '1s81pCQr5SH3jAnB9KwdlADNmszE3xWTs',
          name: '',
          price: 46,
        },
        {
          id: '1e8pIJh804nEi46sw-4QdOZKnAR_SboGT',
          name: '',
          price: 47,
        },
        {
          id: '1ow5SKk-8rDkFj6MD5g4VYXB8yKkDRp2r',
          name: '',
          price: 48,
        },
        {
          id: '1JKVqGKXhJxzVg7iNgC13__xILpBSTy6O',
          name: '',
          price: 49,
        },
        {
          id: '120H2sgYFmlTK0KN5iikeF1cTChoF8onp',
          name: '',
          price: 50,
        },
        {
          id: '1wZyymO2hiab-BIFi_-kaJcPRbA674CVg',
          name: '',
          price: 51,
        },
        {
          id: '1Zxb7gCc748bSKfUcZ9Asab-ihKReaRRr',
          name: '',
          price: 52,
        },
        {
          id: '1xVe6l8jY-qUAbmeAQZeV-h5zNx93mgGu',
          name: '',
          price: 53,
        },
        {
          id: '11nQssbnqp_vs8ruDv2vpUP_5z9pGtf0y',
          name: '',
          price: 54,
        },
        {
          id: '1xLNX4hbEVV9Oc-aXiHGhsxj7RswyFbtx',
          name: '',
          price: 55,
        },
        {
          id: '12mvabRwtJGeuV-HQVKTkVoJ3N72qp7_j',
          name: '',
          price: 56,
        },
        {
          id: '1DW2yKZ4uRki4zvcBO9x-VMsH3K3H1vIy',
          name: '',
          price: 57,
        },
        {
          id: '1a7Zj8WxeWAKxpaiCy12_I1fLrD2kpYu-',
          name: '',
          price: 58,
        },
        {
          id: '1l_1C1zEa_d8CVwINrmOBsYZ1fnCgjyKz',
          name: '',
          price: 59,
        },
        {
          id: '1yHOaB_ggidL3UsX3sTF5NzlvQ-dPVdAu',
          name: '',
          price: 60,
        },
        {
          id: '1HR6nla8jb3sSAdYKv5so0q-Cq2pKUUQr',
          name: '',
          price: 61,
        },
        {
          id: '1revYq26qtTjEE7EPaUyPXYi_QI70C23X',
          name: '',
          price: 62,
        },
        {
          id: '11wtcJ_nFyGtXhwMsu1euj0hg3Z60RXC-',
          name: '',
          price: 63,
        },
        {
          id: '1PSOFf01My5bNZKKMGqO_dSsViH99fCqF',
          name: '',
          price: 64,
        },
        {
          id: '1NYEAorLXQeymFVZKqqAwfIe_j_xweh37',
          name: '',
          price: 65,
        },
        {
          id: '1oCceLrNyQSfL32g7Q8TkbaCmyk1CsTGW',
          name: '',
          price: 66,
        },
        {
          id: '1KYB_pangoiWNfGfUB334hoU91vAJAep8',
          name: '',
          price: 67,
        },
        {
          id: '1CkCFmrR2jXHuOKDeSdaZuupsqLVLpxU8',
          name: '',
          price: 68,
        },
        {
          id: '1u6RKx8Q_bQHsQ0Dhi0HmzEMtshwgSmYu',
          name: '',
          price: 69,
        },
        {
          id: '1v7mjgh2NtEcVpGKvi4Ukg8_ADi7SU5Ua',
          name: '',
          price: 70,
        },
        {
          id: '14zSgiCt1BCxRDT2T--sAjSsSkGju5YB1',
          name: '',
          price: 71,
        },
        {
          id: '136bgMivrvK5aBBWhBbZeY162gEbzGbn5',
          name: '',
          price: 72,
        },
        {
          id: '1oIlqDPSV5Jtt7KNM73oEwBv2RaH-h2V7',
          name: '',
          price: 73,
        },
      ],
    }
  },
  computed: {
    imagesShow() {
      let num = 0
      if (this.$vuetify.breakpoint.width >= 600) {
        num = 3
      } else if (this.$vuetify.breakpoint.width >= 960) {
        num = 4
      } else {
        num = 2
      }
      return num * this.imagesRow
    },
  },
  watch: {
    imagesShow(newValue, oldValude) {
      console.log(newValue, 'watch')
    },
  },
  mounted() {
    console.log(this.imagesShow, 'mounted')
  },
}
</script>
