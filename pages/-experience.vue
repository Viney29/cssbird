<template>
  <div :class="$style.block" id="jobs">
    <h2 :class="$style.heading">Where I've Worked</h2>
    <div :class="$style.row">
      <ul role="tablist" aria-label="Job tabs" :class="$style.tabs">
        <li :class="$style.li">
          <button id="tab-0" role="tab" aria-selected="false" aria-controls="panel-0" tabindex="-1" :class="$style.tabList">
            <span>Anatta</span>
          </button>
        </li>
        <li :class="$style.li">
          <button id="tab-1" role="tab" aria-selected="false" aria-controls="panel-1" tabindex="-1" :class="$style.tablist">
            <span>WebForte Pvt Ltd.</span>
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
        <h5 :class="$style.time"><span>Jul 2018 - Jun 2019</span></h5>
        <div :class="$style.copy">
          <ul>
            <li>Interviewed 5+ prospective employees and mentored junior software developers on the team</li>
            <li>Created and launched CPE mobile on React Native(Typescript). The app for the sale of building materials in the Netherlands. Then I helped the company get a new big project worth €1 Million</li>
            <li>Created and launched Dakota Calc App on React Native(Typescript). The app is used for calculation roof repair on Netherland</li>
            <li>Developed Brockmeyer Portal on React and Nodejs. This web app is a portal for looking for employees in Europe</li>
          </ul>
        </div>
      </div>
      <div id="panel-0" role="tabpanel" aria-labelledby="tab-0" tabindex="-1" :class="$style.tabContent"  hidden></div>
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
  @include padding($top:150px, $bottom: 150px);
  @include margin($left: auto, $right: auto);
  @include max-width(700px);
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
  @include flex($align-items: flex-start);
  @include relative();
}


.tabs {
  display: block;
  position: relative;
  width: max-content;
  z-index: 3;
  list-style: none;

  @include padding($all: 0);
  @include margin(20px, 0, 0, 0);

}

.tabList {
  @include padding(0, 20px, 2px, 20px);
  @include relative();
  @include flex($align-items: center);
  @include blocksize(100%, 42px);
  @include font-family('primary');

  text-decoration: none;
  text-decoration-skip-ink: auto;
  cursor: pointer;
  background-color: transparent;
  border-left: 2px solid rgb(51, 63, 88);
  text-align: left;
  white-space: nowrap;
  font-size: 13px;
  color: rgb(100, 255, 218);
}

.tabContent {
  position: relative;
  width: 100%;
  height: auto;
  padding-top: 12px;
  padding-left: 30px;
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
  @include padding($left: 20px);
  @include margin($bottom: 10px);
  @include font-family('secondary');

  font-size: 13px;
  line-height: 17px;
  color: color('primary');
  text-transform: capitalize;

}
</style>