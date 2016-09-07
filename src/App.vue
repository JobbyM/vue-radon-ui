<template>
  <div id="app">
    <div class=container>
      <rd-datepicker :date="datePicker"></rd-datepicker>
    </div>
  </div>
</template>

<script>
import { rdDatepicker } from 'radon-ui'

export default {
  data () {
    return {
      datePicker: {
        value: '',
        options: {
          quickClose: true,
          format: 'YYYY/MM/DD'
        }
      }
    }
  },
  components: {
    rdDatepicker
  }
}
</script>

<style src=radon-ui/dist/static/css/dist.css></style>
<style>
  .container {
    width: 200px;
    height: 30px;
  }
</style>