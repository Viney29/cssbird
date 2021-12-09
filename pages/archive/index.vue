<template>
  <div :class="$style.block" id="projects">
    <h2 :class="$style.heading">Archive</h2>
    <h4 :class="$style.subtite">A big list of things I’ve worked on</h4>
    <div :class="$style.tablerRow">
      <table :class="$style.table">
        <thead>
          <tr>
            <th>Year</th>
            <th>Title</th>
            <th class="hide-on-mobile">Made at</th>
            <th class="hide-on-mobile">Built with</th>
            <th>Link</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td :class="$style.year">2020</td>
            <td :class="$style.title">Rothy's</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span>Vuejs</span><span>&nbsp;·&nbsp;</span><span>Nuxt</span></td>
            <td :class="$style.link">2020</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style lang="scss" module>

.block {
  @include padding($top:45px, $right: 20px, $bottom: 45px, $left: 20px);
  @include margin($left: auto, $right: auto);

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
  @include flex($direction: column, $align-items: flex-start);
  @include relative();
}

</style>
