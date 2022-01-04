<template>
  <div :class="$style.block" id="jobs">
    <h2 :class="$style.heading">Where I've Worked</h2>
    <div :class="$style.row">
      <ul role="tablist" aria-label="Job tabs" :class="$style.tabs">
        <li :class="[$style.li, $style.isActive]">
          <button id="tab-0" role="tab" aria-selected="false" aria-controls="panel-0" tabindex="-1" :class="$style.tabList">
            <span>Anatta</span>
          </button>
        </li>
        <li :class="$style.li">
          <button id="tab-1" role="tab" aria-selected="false" aria-controls="panel-1" tabindex="-1" :class="$style.tabList">
            <span>WebForte Pvt Ltd.</span>
          </button>
        </li>
        <li :class="$style.li">
          <button id="tab-2" role="tab" aria-selected="false" aria-controls="panel-2" tabindex="-1" :class="$style.tabList">
            <span>WebCronz</span>
          </button>
        </li>
        <span :class="$style.highlight"></span>
      </ul>
      <div id="panel-0" role="tabpanel" aria-labelledby="tab-0" tabindex="-1" :class="$style.tabContent" >
        <h4 :class="$style.title">
          <span>Sr UI Developer</span>
          <span :class="$style.company">
            <a :class="$style.link" href="http://anatta.io/" target="_blank" rel="nofollow noopener noreferrer">@ Anatta</a>
          </span>
          </h4>
        <h5 :class="$style.time"><span>January 2018 - Till Date</span></h5>
        <div :class="$style.copy">
          <ul>
            <li>Interviewed 10+ prospective employees and mentored junior UI developers on the team</li>
            <li>Optimized web performance by improving  Web Vitals.</li>
            <li>Developed multiple Single page applications using Vuejs.</li>
            <li>Developing and updating PLPs and PDPs to improve user experience and increase conversion and AOV across multiple brand websites whilst maintaining best practices (A/B testing).</li>
            <li>Rebranded multiple e-commerce websites which increases the number of leads.</li>
            <li>Developed PWA in Vue Js using shopify storefront API.</li>
            <li>Developed UI kit containing generic components to be used across the company.</li>
          </ul>
        </div>
      </div>
      <div id="panel-1" role="tabpanel" aria-labelledby="tab-1" tabindex="-1" :class="$style.tabContent"  hidden>
        <h4 :class="$style.title">
          <span>Sr UI Developer</span>
          <span :class="$style.company">
            <a :class="$style.link" href="http://anatta.io/" target="_blank" rel="nofollow noopener noreferrer">@ Anatta</a>
          </span>
        </h4>
        <h5 :class="$style.time"><span>August 2015 - December 2017</span></h5>
        <div :class="$style.copy">
          <ul>
            <li>Development of Clean Code - Optimized for performance, search engines and cross browsers compatibility.</li>
            <li>Improved website speed by optimizing images, reducing render blocking and eliminating dependency on external CSS libraries by designing custom stylesheets.</li>
            <li>Converted Sketch files  to responsive web pages using HTML5, CSS3 and JS.</li>
            <li>Developed custom HTML5 email templates for clients marketing campaigns.</li>
            <li>Developed pixel perfect responsive wordpress websites from scratch.</li>
            <li>Collaborated with a team of designers and developers to deploy and maintain over 50 WordPress sites.</li>
          </ul>
        </div>
      </div>
      <div id="panel-2" role="tabpanel" aria-labelledby="tab-2" tabindex="-1" :class="$style.tabContent"  hidden></div>
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

  width: 100%;

  @include above('tablet'){
    @include padding($top:75px, $bottom: 75px);
    @include max-width(700px);
  }

  @include above('tablet-large'){
    @include padding(150px,0, 150px,0);
  }
}

.heading {
  @include relative();
  @include flex($align-items: center);
  @include margin(10px, 0, 40px, 0);
  @include font-family('primary');

  width: 100%;
  white-space: nowrap;
  font-size: 32px;
  line-height: 42px;
  color: color('primary-200');
  text-transform: capitalize;

  @include below('tablet'){
    font-size: 24px;
  }

  &::before {
    counter-increment: section 1;
    content: "0" counter(section) ".";

    @include relative();
    @include margin($right: 10px);
    @include font-family('secondary');

    color: color('highlight');
    font-weight: normal;
    font-size: 20px;
    bottom: 4px;
  }

  &::after {
    content: "";
    display: block;

    @include relative($top: -5px);
    @include margin($left: 20px);
    @include blocksize(300px, 1px);

    background-color: rgb(45, 57, 82);
  }
}

.row {
  @include flex($direction: column, $align-items: flex-start);
  @include relative();

  @include above('tablet'){
    flex-direction: row;
  }
}


.tabs {
  display: block;
  position: relative;
  width: max-content;
  z-index: 3;
  list-style: none;

  @include padding($all: 0);
  @include margin(20px, 0, 0, 0);

  @include below('tablet'){
    width: 100%;
    display: flex;
  }

}

.tabList {
  @include padding(0, 20px, 2px, 20px);
  @include relative();
  @include flex($align-items: center);
  @include blocksize(100%, 42px);
  @include font-family('secondary');

  border: none;
  min-width: 180px;
  text-decoration: none;
  text-decoration-skip-ink: auto;
  cursor: pointer;
  background-color: transparent;
  border-left: 2px solid rgb(51, 63, 88);
  text-align: left;
  white-space: nowrap;
  font-size: 13px;
  color: inherit;

  &:hover {
    background-color: rgb(23, 42, 69);
  }

  @include below('tablet'){
    min-width: fit-content;
    width: 33%;
    border-left: none;
    border-bottom: 2px solid rgb(51, 63, 88);
  }
}

.highlight {
  display: block;
  background: rgb(100, 255, 218);
  width: 2px;
  height: 42px;
  border-radius: 3px;
  position: absolute;
  top: 0;
  left: 0;
  transition: transform 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0.1s;
  z-index: 10;
  transform: translateY(0);

  @include below('tablet'){
    width: 100%;
    max-width: 33%;
    height: 2px;
    top: auto;
    bottom: 0;
    transform: translateX(0);
  }
}

.tabContent {
  @include relative();
  @include blocksize(100%, auto);
  @include padding($top: 12px, $left: 30px);
  @include margin($top: 20px);

  @include below('tablet'){
    @include padding( $left: 5px);
  }
}

.title {
  @include font-family('primary');

  color: rgb(204, 214, 246);
  font-size: 22px;
  font-weight: 500;
  margin-bottom: 5px;
}

.company {
  color: color('highlight');
}

.link {
    display: inline-block;
    text-decoration: none;
    text-decoration-skip-ink: auto;
    position: relative;
    transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
    cursor: pointer;
    color: rgb(100, 255, 218);
}

.time {
    @include font-family('secondary');

    font-size: 13px;
    font-weight: normal;
    letter-spacing: 0.05em;
    color: rgb(168, 178, 209);
    margin-bottom: 30px;
}

.copy {
  @include font-family('primary');

  ul {
    padding: 0;
    margin: 0;
    list-style: none;
    font-size: 18px;
  }

  li {
    position: relative;
    padding-left: 30px;
    margin-bottom: 10px;

    &::before {
      content: "▹";
      position: absolute;
      left: 0;
      color: rgb(100, 255, 218);
    }
  }
}

.li {
  @include relative();
  @include padding($left: 0);
  @include margin($bottom: 0);
  @include font-family('secondary');

  font-size: 13px;
  line-height: 17px;
  color: color('primary');
  text-transform: capitalize;

  &:hover,
  &.isActive {
     background-color: rgb(23, 42, 69);
     color: rgb(100, 255, 218);
  }

}
</style>
