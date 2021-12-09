<template>
  <div :class="$style.block" id="projects">
    <h2 :class="$style.heading">Archive</h2>
    <h4 :class="$style.subtitle">A big list of things I’ve worked on</h4>
    <div :class="$style.tableRow">
      <table :class="$style.table">
        <thead>
          <tr>
            <th :class="$style.th">Year</th>
            <th :class="$style.th">Title</th>
            <th :class="[$style.th, $style.onlyDesktop]">Made at</th>
            <th :class="[$style.th, $style.onlyDesktop]">Built with</th>
            <th :class="$style.th">Link</th>
          </tr>
        </thead>
        <tbody>
          <tr :class="$style.tr">
            <td :class="$style.year">2020-21</td>
            <td :class="$style.title">Mackwledon</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Vuejs</span><span>&nbsp;·&nbsp;</span><span>Nuxt</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://mackweldon.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2019-20</td>
            <td :class="$style.title">Rothy's</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Vuejs</span><span>&nbsp;·&nbsp;</span><span>Nuxt</span><span>&nbsp;·&nbsp;</span><span>PWA</span><span>&nbsp;·&nbsp;</span><span>Optimizely</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://rothys.com"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2019</td>
            <td :class="$style.title">Athletic Greens</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Vuejs</span><span>&nbsp;·&nbsp;</span><span>Nuxt</span><span>&nbsp;·&nbsp;</span><span>PWA</span><span>&nbsp;·&nbsp;</span><span>Optimizely</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://athleticgreens.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2019</td>
            <td :class="$style.title">Upscribe</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Vuejs</span><span>&nbsp;·&nbsp;</span><span>Nuxt</span><span>&nbsp;·&nbsp;</span><span>PWA</span><<span>&nbsp;·&nbsp;</span><span>Web Vitals</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://upscribe.io/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2019</td>
            <td :class="$style.title">Marie forleo.</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Shopify</span><span>&nbsp;·&nbsp;</span><span>Vujs</span><span>&nbsp;·&nbsp;</span><span>PWA</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span></span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://www.marieforleo.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2019</td>
            <td :class="$style.title">Dr Chatterjee</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Wordpress</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://drchatterjee.com"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Kosas</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Shopify</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://kosas.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Vimergy</td>
            <td :class="$style.company">Anatta</td>
            <td :class="$style.tech"><span><span>Shopify</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://vimergy.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Golub</td>
            <td :class="$style.company">Webforte Technologies</td>
            <td :class="$style.tech"><span><span>Wordpress</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https:golubandcompany.com"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Momentchicago</td>
            <td :class="$style.company">Webforte Technologies</td>
            <td :class="$style.tech"><span><span>Wordpress</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://www.momentchicago.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Marqueeblock37</td>
            <td :class="$style.company">Webforte Technologies</td>
            <td :class="$style.tech"><span><span>Wordpress</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://www.marqueeblock37.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Love that video</td>
            <td :class="$style.company">Webforte Technologies</td>
            <td :class="$style.tech"><span><span>Wordpress</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://lovethatvideo.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">1001southstate</td>
            <td :class="$style.company">Webforte Technologies</td>
            <td :class="$style.tech"><span><span>Wordpress</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://www.1001southstate.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Fog pilot</td>
            <td :class="$style.company">Webforte Technologies</td>
            <td :class="$style.tech"><span><span>Wordpress</span><span>&nbsp;·&nbsp;</span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>Css</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="http://fog-pilot.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
          </tr>
          <tr :class="$style.tr">
            <td :class="$style.year">2018</td>
            <td :class="$style.title">Blur Communications</td>
            <td :class="$style.company">Webforte Technologies</td>
            <td :class="$style.tech"><span><span>Js</span><span>&nbsp;·&nbsp;</span><span>Html</span><span>&nbsp;·&nbsp;</span><span>CSS</span></span></td>
            <td :class="$style.link"><a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="http://blurcommunications.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a></td>
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
    @include max-width(1400px);

    min-height: 100vh;
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

  @include above('tablet'){
    font-size: 42px;
  }

  @include above('tablet-large'){
    font-size: 60px;
  }
  @include above('desktop'){
    font-size: 80px;
  }
}

.subtitle {
  @include margin($bottom: 20px);
  @include font-family('secondary');

  color: rgb(100, 255, 218);
  font-size: 16px;
  font-weight: normal;
  line-height: 1.5;
}

.row {
  @include flex($direction: column, $align-items: flex-start);
  @include relative();
}

.tableRow {
  @include margin($top: 60px, $bottom: 60px);

  @include above('tablet'){
    @include margin($top: 80px, $bottom: 80px);
  }

  @include above('desktop'){
     @include margin($top: 100px, $bottom: 100px);
  }
}

.table {
  display: table;
  width: 100%;
  border-collapse: collapse;
  text-indent: initial;
  border-spacing: 2px;
  border-color: grey;
}

.tr:hover  {
  background-color: rgb(23, 42, 69);
}

.th {
  text-align: left;
  line-height: 1.5;
  padding: 10px 20px;

  @include use-text-style('title');
  @include font-family('primary');

  color: #8892b0;

  @include below('tablet'){
    padding: 8px 4px;
  }
}

.projectLink {
  text-decoration: none;
  color: inherit;

  svg {
    width:20px;
    height: 20px;
    fill: currentColor;
  }

  &:hover {
    color: color('highlight');

    svg {
      fill: currentColor;
    }
  }

  @include below('tablet'){
    color: #a8b2d1;
  }
}

.link {
  display: inline-block;
  text-decoration: none;
  text-decoration-skip-ink: auto;
  color: inherit;
  position: relative;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
}

.table td {
  line-height: 1.5;
  padding: 10px 20px;

  @include below('tablet'){
    padding: 8px 5px;
  }
}

.year {
  width: 25%;
  color: rgb(100, 255, 218);
  font-size: 12px;

  @include font-family('secondary');

  @include above('tablet-large'){
   width: 10%;
   font-size: 16px;
  }
}

.table .title {
  padding-top: 10px;
  color: rgb(204, 214, 246);
  font-size: 18px;
  font-weight: 700;

  @include font-family('primary');

  @include above('tablet-large'){
   padding-top: 15px;
   font-size: 20px;
  }

}

.table .company {
  width: 35%;
  padding-top: 10px;
  font-size: 16px;
  display: none;

  @include font-family('primary');

  @include above('tablet-large'){
    display: table-cell;
    width: 15%;
    padding-top: 15px;
    font-size: 18px;
  }
}

.tech {
  @include font-family('secondary');

  font-size: 12px;
  display: none;

  @include above('tablet-large'){
    display: table-cell;
  }
}

.onlyDesktop {
  display: none;

  @include above('tablet-large'){
    display: table-cell;
  }
}

</style>
