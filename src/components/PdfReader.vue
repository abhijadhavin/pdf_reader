<template>
  <div>    
    <PDFViewer
      :source="base64"
      style="height: 100vh; width: 100vw"
      @download="handleDownload"
    />
  </div>
</template>


<script>
import PDFViewer from 'pdf-viewer-vue'

// OR THE FOLLOWING IMPORT FOR VUE 2
// import PDFViewer from 'pdf-viewer-vue/dist/vue2-pdf-viewer'

export default {
  components: {
    PDFViewer,
  },

  data() {
    return {       
      base64: '<BASE64_ENCODED_PDF>',
    }
  },
}
</script>