<template>
  <div class="moduleindex" :class="{ indexview: index }">

    <div class="coursetitle">Mapping and Data</div>
    <div class="course">
      <SequenceLinks path="14-geospatial-concepts" />
      <SequenceLinks path="15-intro-qgis" />
      <SequenceLinks path="19-data_visualization" />
    </div>

    <div class="coursetitle">Computational Drawing</div>
    <div class="course">
      <SequenceLinks path="12-rhino-intro" />
      <SequenceLinks path="13-arch-drawing" />
    </div>

    <div class="coursetitle">Programming for Design Practices: A - Grasshopper</div>
    <div class="course">
      <SequenceLinks path="4-grasshopper-intro" />
      <SequenceLinks path="5-computational-design-modeling-in-grasshopper" />
    </div>

    <div class="coursetitle">Programming for Design Practices: B - Python</div>
    <div class="course">
      <SequenceLinks path="6-intro-to-python" />
      <SequenceLinks path="7-fundamentals-of-python" />
      <SequenceLinks path="8-intro-to-python-in-rhino" />
      <SequenceLinks path="10-spatial-python" />
    </div>

    <div class="coursetitle">Programming for Design Practices: C - Web and Interactivity</div>
    <div class="course">
      <SequenceLinks path="11-interactive-web" />
      <SequenceLinks path="16-ambient-computing-network-architecture" />
      <SequenceLinks path="17-ambient-computing-interactivity" />
      <SequenceLinks path="18-behavioral-modeling-intro" />
    </div> 

       <div class="coursetitle">Computation for Design and Representation</div>
    <div class="course">
      <SequenceLinks path="21-integrated-computational-simulation" />
    </div> 


  </div>
</template>

<style scoped>

.course {
  border-left: 2px solid gray;
  padding-left: 8px;
}

.coursetitle {
  font-size: 1.5em;
  margin-bottom: 10px;
}

.moduleindex {
  color: 555;
  font-family: Lato;
  color: black;
  font-size: 0.85em;
}

.sequence {
  line-height: 1.5em;
  margin-bottom: 20px;
}


</style>

<script>

export default {
  data() {
    return {
      hover: false,
    };
  }, 
  props: ['index', 'blah'],
  computed: {
    contentdata () {
      return this.$store.state.contentdata
    }
  },
  methods: {
  },
}
</script>
