# vue2 pagination

> A Vue.js project

## Get started

It must be used in the environment of vue2.0 or more

## Usage

You need to use pagination in your vue app's main file or the container you need to use:
``` bash
import vPagination from 'pagination.vue'
Vue.use(Eagle)
``` 
## Basic idea
A very basic File Component for pagination would look like this:
``` bash
<v-pagination :total="total" :current-page='current' :pagegroup="pagegroup" @pagechange="pagechange" v-if="isShowPagination"></v-pagination>

<script>
import vPagination from 'pagination.vue'
export default {
  components: {
    'v-pagination': vPagination
  },
  data() {
    total: 1,     // Total number of records
    display: 10,   // Display number per page
    current: 1,   // Current page number
    pagegroup: 1,
    isShowPagination: false
  },
  methods: {
    pagechange(currentPage) {
      console.log(currentPage);
    }
  }
}
</script>
```
