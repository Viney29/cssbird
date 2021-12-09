<template>
  <div :class="$style.block" id="contact">
    <h4 :class="$style.highlight">What's Next?</h4>
    <h5 :class="$style.heading">get in touch</h5>
    <div :class="$style.content">
      <p>If your team is looking for a creative, high professional and result-oriented developer, my inbox is always open. Whether for a potential project or just to say hi, I'll try my best to answer your email!</p>
    </div>
    <a :class="$style.link"  href="mailto:viney.bishnoi@gmail.com" rel="nofollow noopener noreferrer" aria-label="External Link">Say Hello</a>
  </div>
</template>

<script>

export default {
  data(){
    return{
      techs:[
      {
        name:'JavaScript (ES6+)',
      },
      {
        name:'HTML & (S)CSS',
      },
      {
        name:'vueJs',
      },
      {
        name:'Nuxt',
      },
    ]
    }
  }
}
</script>

<style lang="scss" module>

.block {
  @include padding($top:45px, $right: 20px, $bottom: 45px, $left: 20px);
  @include margin($left: auto, $right: auto);
  @include text('center');

  width: 100%;

  @include above('tablet'){
    @include padding($top:75px, $bottom: 75px);
    @include max-width(600px);
  }

  @include above('tablet-large'){
    @include padding(150px,0, 150px,0);
  }
}

.highlight {
  @include relative();
  @include flex($align-items: center, $justify-content: center);
  @include margin(10px, 0, 20px, 0);
  @include font-family('secondary');

  color: color('highlight');
  width: 100%;
  white-space: nowrap;
  font-size: 16px;
  font-weight: normal;

  &::before {
    counter-increment: section 1;
    content: "0" counter(section) ".";

    @include relative();
    @include margin($right: 10px);
    @include font-family('secondary');

    color: color('highlight');
    font-weight: normal;
    font-size: 16px;
  }
}

.heading {
  margin: 0 0 20px;
  font-size: 32px;
  color: color('primary-200');
  text-transform: capitalize;

  @include above('tablet'){
    font-size: 42px;
  }

  @include above('tablet-large'){
     font-size: 60px;
  }
}


.content {
  @include use-text-style('copy');

  @include below('tablet'){
    font-size: 18px;
  }
}

.link {
  @include padding(1.25rem, 1.75rem, 1.25rem, 1.75rem);
  @include margin($top: 50px);
  @include use-text-style('button');

  display: inline-flex;
  color: color('highlight');
  background-color: transparent;
  border: 1px solid color('highlight');
  border-radius: 3px;
  text-decoration: none;
  text-transform: capitalize;
  cursor: pointer;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
  margin-top: 50px;

  &:hover {
    background-color: rgba(100, 255, 218, 0.07);
  }

  @include below('tablet'){
    margin-top: 30px;
  }
}
</style>
