<script>
import homePageHtml from './homePage.html'
let Cesium = require('../../../node_modules/cesium/Build/Cesium/Cesium')
import 'cesium/Widgets/widgets.css'
export default {
  name: 'homePage',
  extends: homePageHtml,
  data () {
    return {
      viewer: null
    }
  },
  methods: {
    initMap () {
      this.viewer = new Cesium.Viewer('project')
    }
  },
  mounted () {
    this.initMap()
  }
}
</script>
