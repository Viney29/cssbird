<template>
  <div :class="$style.block" id="projects">
    <h2 :class="$style.heading">Other Noteworthy Projects</h2>
    <nuxt-link :class="$style.link" to="/archive">view the archive</nuxt-link>
    <div :class="$style.row">
      <div :class="$style.item">
        <div :class="$style.content">
          <span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 60 60"><title>Folder</title><path d="M57.49,21.5H54v-6.268c0-1.507-1.226-2.732-2.732-2.732H26.515l-5-7H2.732C1.226,5.5,0,6.726,0,8.232v43.687l0.006,0 c-0.005,0.563,0.17,1.114,0.522,1.575C1.018,54.134,1.76,54.5,2.565,54.5h44.759c1.156,0,2.174-0.779,2.45-1.813L60,24.649v-0.177 C60,22.75,58.944,21.5,57.49,21.5z M2,8.232C2,7.828,2.329,7.5,2.732,7.5h17.753l5,7h25.782c0.404,0,0.732,0.328,0.732,0.732V21.5 H12.731c-0.144,0-0.287,0.012-0.426,0.036c-0.973,0.163-1.782,0.873-2.023,1.776L2,45.899V8.232z M47.869,52.083 c-0.066,0.245-0.291,0.417-0.545,0.417H2.565c-0.243,0-0.385-0.139-0.448-0.222c-0.063-0.082-0.16-0.256-0.123-0.408l10.191-27.953 c0.066-0.245,0.291-0.417,0.545-0.417H54h3.49c0.38,0,0.477,0.546,0.502,0.819L47.869,52.083z"></path></svg></span>
          <h5 :class="$style.name">Name</h5>
          <div :class="$style.copy">
            <p>Register your in-app as a dealer and you can purchase roofing materials directly from CPE. Photo order, direct contact. Easy ordering when / where you want.</p>
          </div>
          <ul :class="$style.ul">
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
          </ul>
        </div>
      </div>
      <div :class="$style.item">
        <div :class="$style.content">
          <span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 60 60"><title>Folder</title><path d="M57.49,21.5H54v-6.268c0-1.507-1.226-2.732-2.732-2.732H26.515l-5-7H2.732C1.226,5.5,0,6.726,0,8.232v43.687l0.006,0 c-0.005,0.563,0.17,1.114,0.522,1.575C1.018,54.134,1.76,54.5,2.565,54.5h44.759c1.156,0,2.174-0.779,2.45-1.813L60,24.649v-0.177 C60,22.75,58.944,21.5,57.49,21.5z M2,8.232C2,7.828,2.329,7.5,2.732,7.5h17.753l5,7h25.782c0.404,0,0.732,0.328,0.732,0.732V21.5 H12.731c-0.144,0-0.287,0.012-0.426,0.036c-0.973,0.163-1.782,0.873-2.023,1.776L2,45.899V8.232z M47.869,52.083 c-0.066,0.245-0.291,0.417-0.545,0.417H2.565c-0.243,0-0.385-0.139-0.448-0.222c-0.063-0.082-0.16-0.256-0.123-0.408l10.191-27.953 c0.066-0.245,0.291-0.417,0.545-0.417H54h3.49c0.38,0,0.477,0.546,0.502,0.819L47.869,52.083z"></path></svg></span>
          <h5 :class="$style.name">Name</h5>
          <div :class="$style.copy">
            <p>Register your in-app as a dealer and you can purchase roofing materials directly from CPE. Photo order, direct contact. Easy ordering when / where you want.</p>
          </div>
          <ul :class="$style.ul">
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
          </ul>
        </div>
      </div>
      <div :class="$style.item">
        <div :class="$style.content">
          <span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 60 60"><title>Folder</title><path d="M57.49,21.5H54v-6.268c0-1.507-1.226-2.732-2.732-2.732H26.515l-5-7H2.732C1.226,5.5,0,6.726,0,8.232v43.687l0.006,0 c-0.005,0.563,0.17,1.114,0.522,1.575C1.018,54.134,1.76,54.5,2.565,54.5h44.759c1.156,0,2.174-0.779,2.45-1.813L60,24.649v-0.177 C60,22.75,58.944,21.5,57.49,21.5z M2,8.232C2,7.828,2.329,7.5,2.732,7.5h17.753l5,7h25.782c0.404,0,0.732,0.328,0.732,0.732V21.5 H12.731c-0.144,0-0.287,0.012-0.426,0.036c-0.973,0.163-1.782,0.873-2.023,1.776L2,45.899V8.232z M47.869,52.083 c-0.066,0.245-0.291,0.417-0.545,0.417H2.565c-0.243,0-0.385-0.139-0.448-0.222c-0.063-0.082-0.16-0.256-0.123-0.408l10.191-27.953 c0.066-0.245,0.291-0.417,0.545-0.417H54h3.49c0.38,0,0.477,0.546,0.502,0.819L47.869,52.083z"></path></svg></span>
          <h5 :class="$style.name">Name</h5>
          <div :class="$style.copy">
            <p>Register your in-app as a dealer and you can purchase roofing materials directly from CPE. Photo order, direct contact. Easy ordering when / where you want.</p>
          </div>
          <ul :class="$style.ul">
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">Vuejs</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      jobs:[
      {
        name:'Anatta',
        position: 'Sr UI Engineer',
        link:'#'
      },
      {
        name:'WebForte',
        position: 'Frontend Developer',
        link:'#'
      },
      {
        name:'Web Cronz',
        position: 'UI Intern',
        link:'#'
      }
    ]
    }
  }
}
</script>

<style lang="scss" module>

.block {
  @include padding($top:45px, $right: 20px, $bottom: 45px, $left: 20px);
  @include margin($left: auto, $right: auto);
  @include flex($direction: column, $align-items: flex-start, $justify-content: center);

  width: 100%;

  @include above('tablet'){
    @include padding($top:75px, $bottom: 75px);
  }

  @include above('tablet-large'){
    @include padding(150px,0, 150px,0);
    @include max-width(1000px);
  }
}


.heading {
  @include margin(0, auto,0, auto);
  @include font-family('primary');

  font-size: 32px;
  line-height: 42px;
  color: color('primary-200');
  text-transform: capitalize;

  @include below('tablet'){
    font-size: 24px;
  }
}

.link {
  @include font-family('secondary');

  text-decoration: none;
  color:color('highlight');
  font-size: 14px;
  line-height: 24px;
  text-align: center;
  margin: auto;

  &::after {
    content: "";
    display: block;
    width: 0;
    height: 1px;
    position: relative;
    bottom: 0.1em;
    background-color: rgb(100, 255, 218);
    transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
    opacity: 0.5;
  }

  &:hover{

    &::after {
      width: 100%;
    }
  }
}

.row {
  @include relative();

  margin-top: 50px;
  width: 100%;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 15px;

  @include below('tablet'){
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  }
}

.item {
  box-shadow: rgb(2 12 27 / 70%) 0 10px 30px -15px;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  align-items: flex-start;
  position: relative;
  padding: 2rem 1.75rem;
  height: 100%;
  border-radius: 3px;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
  background-color: rgb(23, 42, 69);

  &:focus,
  &:hover {
    @include above('tablet'){
      box-shadow: rgb(2 12 27 / 70%) 0 20px 30px -15px;
      transform: translateY(-5px);
    }
  }
}

.icon {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 30px;
  color: color('highlight');

  svg {
    @include blocksize(40px);

    fill: currentColor;
  }
}

.name {
  margin: 0 0 10px;
  font-size: 22px;
  color: rgb(204, 214, 246);
}

.copy {
  font-size: 17px;
  line-height: 22px;
  color: rgb(168, 178, 209);
}


.ul {
  display: flex;
  align-items: flex-end;
  flex-grow: 1;
  flex-wrap: wrap;
  padding: 0;
  margin: 20px 0 0;
  list-style: none;
}

.li {
  @include font-family('secondary');

  font-size: 12px;
  color: rgb(136, 146, 176);
  line-height: 1.75;
  margin-right: 15px;
}
</style>
