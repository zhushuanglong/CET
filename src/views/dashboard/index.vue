<template>
  <div class="dashboard-container">
    <component :is="currentRole" />
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
import uploadExcel from './upload-excel'
import page404 from '../error-page/404'

export default {
  name: 'Dashboard',
  components: { uploadExcel, page404 },
  data() {
    return {
      currentRole: 'uploadExcel'
    }
  },
  computed: {
    ...mapGetters([
      'roles'
    ])
  },
  created() {
    if (!this.roles.includes('admin')) {
      this.currentRole = 'page404'
    }
  }
}
</script>
