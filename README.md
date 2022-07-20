# 国家地区组件
组件的样式
![示例图片](https://github.com/1880809/country-components/blob/main/e.jpg)

引入的地方
![示例图片](https://github.com/1880809/country-components/blob/main/e2.jpg)

   <country @getCountrieCode="getCountrieCode" v-if="countryShow"></country>

   	import country from '../../components/country/country'
       data () {
       return {
        countryShow: false
       }
   },
   
   components: {
      country,
		},
      getCountrieCode(event) {
        if(event.dialCode) {
          this.areaCode = event.dialCode
        }
        this.countryShow = false
      },
