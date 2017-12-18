<script type="text/javascript">
  import DataTable from 'vuetify/es5/components/VDataTable'

  /* Extendes Data-table from vuetify
  * - https://vuetifyjs.com/components/data-tables
  */


  export default {
    extends: DataTable,

    render (h) {
      return h('table', {
        'class': {
          'datatable table': true,
          'datatable--select-all': this.selectAll
        }
      }, [
        this.genTHead(),
        this.genTBody()
      ])
    }
  }
</script>