<template>
  <div :class="$style.block" id="about">
    <h2 :class="$style.heading">About me</h2>
    <div :class="$style.row">
      <div :class="$style.content">
        <p>Hello! I'm Viney, a UI engineer and Biker. Here's the link to my blog on medium. I love programming, writing, speaking and traveling.</p>
        <p>As a UI engineer, I enjoy using my obsessive attention to detail, my unequivocal love for making things that change the world. That's why I like to make things that make a difference.</p>
        <p>Here are a few technologies I've been working with recently:</p>
        <ul :class="$style.ul">
          <li v-for="item in techs" :class="$style.li" :key="item.name" >{{ item.name }}</li>
        </ul>
      </div>
      <div :class="$style.media">
        <span :class="$style.user" >
          <img src="../assets/images/user.png"/>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      techs:[
      {
        name:'HTML',
      },
      {
        name:'CSS',
      },
      {
        name:'JavaScript (ES6+)',
      },
      {
        name:'VueJs',
      },
      {
        name:'Webpack',
      },
      {
        name:'Web Vitals',
      },
      {
        name:'Googling :)',
      },
    ]
    }
  }
}
</script>

<style lang="scss" module>

.block {
  @include padding($top:150px, $bottom: 150px);
  @include margin($left: auto, $right: auto);
  @include max-width(1000px);
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
  @include flex($justify-content: space-between, $align-items: center);
}

.content {
  @include margin($top: 25px);

  max-width: 480px;
  width: 60%;

  @include use-text-style('copy');
}

.media {
  @include relative();
  @include margin($left: 60px);

  width: 40%;
  max-width: 300px;
}

.user {
  @include flex();
  @include blocksize(300px, 326px);
  @include relative();

  transition: transform .1s linear;

  &::after {
    content: "";
    display: block;
    position: absolute;
    left: 20px;
    top: 20px;
    width: 100%;
    height: 100%;
    border: 2px solid rgb(100, 255, 218);
    border-radius: 3px;
    z-index: -1;
    transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
  }


  img {
    @include absolute();
    @include blocksize(100%);

    object-fit: cover;
    border-radius: 3px;
    transition: transform .1s linear;
    cursor: pointer;
  }


  &:hover img{
    transform: scale(.9) translate(22px, 22px);
    transition: transform .2s linear;
  }
}

.ul {
  display: grid;
  grid-template-columns: repeat(2, minmax(140px, 200px));
  overflow: hidden;

  @include padding($all: 0);
  @include margin(20px, 0, 0, 0);

  list-style: none;
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

  &::before {
    content: "▹";

    @include absolute($left: 0);

    color: color('highlight');
    font-size: 14px;
    line-height: 12px;
  }
}
</style>
