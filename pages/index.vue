<template>
  <div>
    <header>
      <h1>Zach Spring</h1>
      <p class="flex">
        <AcademicCapIcon class="svg-icon-sky" />
        Computer Science student at the University of Central Florida
      </p>
      <p class="flex">
        <BriefcaseIcon class="svg-icon-sky" />
        Chief Executive Officer at&nbsp;
        <a href="https://streamcord.io/" target="_blank" rel="noopener">Streamcord, LLC</a>
      </p>
      <p class="flex">
        <MapPinIcon class="svg-icon-sky" />
        Maineville, OH &middot; Orlando, FL
      </p>
      <p class="flex">
        <EnvelopeIcon class="svg-icon-sky" />
        <a href="mailto:me@zachspri.ng" target="_blank" rel="noopener">me@zachspri.ng</a>
      </p>
      <p class="flex">
        <GlobeAltIcon class="svg-icon-sky" />
        <a href="https://www.linkedin.com/in/zach-spring-94bb73227/" target="_blank" rel="noopener">LinkedIn</a>
        &nbsp;&middot;&nbsp;
        <a href="https://github.com/zspri" target="_blank" rel="noopener">GitHub</a>
      </p>
    </header>
    <h2>Skills</h2>
    <h3>Programming Languages</h3>
    <ul class="ul-cols-2">
      <li>Python</li>
      <li>Go</li>
      <li>TypeScript</li>
      <li>JavaScript</li>
      <li>Java</li>
      <li>C / C++</li>
      <li>Swift</li>
      <li>SQL</li>
      <li>Visual Basic</li>
    </ul>
    <h3>Libraries, Frameworks, & Stacks</h3>
    <ul class="ul-cols-2">
      <li>discord.py</li>
      <li>Vue / Nuxt.js</li>
      <li>React / Next.js</li>
      <li>Cloudflare Workers</li>
      <li>Flask</li>
      <li>Chrome Extensions</li>
      <li>SwiftUI</li>
    </ul>
    <h3>Databases & Programs</h3>
    <ul class="ul-cols-2">
      <li>MongoDB</li>
      <li>RethinkDB</li>
      <li>Redis</li>
      <li>Docker</li>
    </ul>
    <h3>Other</h3>
    <ul class="ul-cols-2">
      <li>Figma</li>
      <li>Spanish (Professional working proficiency)</li>
      <li>Magento</li>
      <li>Shopify</li>
      <li>Linux, Windows, Mac</li>
      <li>Microsoft Word Suite</li>
    </ul>
    <h2>Experience</h2>
    <EntryList>
      <Entry
        href="https://streamcord.io/"
        position="Chief Executive Officer"
        company="Streamcord, LLC"
        image-url="/logos/streamcord.png"
        :start-date="new Date(2017, 8)"
        :highlights="[
          'Built and launched online automation service for >1,000,000 content creators and consumers of Discord and Twitch.',
          'Maintained and administrated a production Docker environment using several cloud servers with 99.9% uptime.',
          'Wrote microservice-oriented code using a diverse stack of languages, frameworks, and databases.',
          'Recruited and hired software developers and customer service representatives.',
          'Managed customer service teams and wrote documentation for common customer interactions.',
          'Created a profitable subscription-based business model.'
        ]"
      />
      <Entry
        href="https://johnsonelectric.com/"
        position="Intern, Web Development"
        company="Johnson Electric"
        image-url="/logos/johnsonelectric.png"
        :start-date="new Date(2023, 6)"
        :highlights="[
          'Worked with a third-party marketing agency to transform visual concepts / mockups into a final, functioning webpage.',
          'Collaborated with designer and made contributions to page design elements before implementation.',
          'Recommended and implemented enhancements to user experience and SEO.',
          'Programmed 7 product pages using React.',
          'Refactored existing codebase.',
          'Experienced in React and using Git and Docker workflows.'
        ]"
      />
    </EntryList>
    <LinkButton href="https://www.linkedin.com/in/zach-spring-94bb73227/details/experience/">
      View more experience on LinkedIn
      <ArrowRightIcon />
    </LinkButton>
    <h2>Education</h2>
    <EntryList>
      <Entry
        href="https://ucf.edu/"
        position="University of Central Florida"
        company="B.S., Computer Science; Minor, Finance"
        image-url="/logos/ucf.png"
        :start-date="new Date(2023, 7)"
        :end-date="new Date(2027, 4)"
        :highlights="[
          'Burnett Honors College',
          'Beta Theta Pi Fraternity: Merchandise Committee, Recruitment Committee, Alumni Relations Chair, Health & Wellbeing Chair',
          'Intramural Pickleball'
        ]"
      />
    </EntryList>
    <LinkButton href="https://www.linkedin.com/in/zach-spring-94bb73227/details/education/">
      View more education on LinkedIn
      <ArrowRightIcon />
    </LinkButton>
    <footer class="mt-12 pt-6 border-t-[1px] border-slate-200 text-sm text-gray-500">
      <span>Copyright &copy; 2024 Zach Spring</span>
    </footer>
  </div>
</template>

<style scoped>
h1 {
  @apply mb-4 mt-6 font-bold text-4xl text-gray-900;
}

h2 {
  @apply mb-4 mt-6 font-semibold text-3xl text-gray-900;
}

h3 {
  @apply mb-1 mt-4 font-semibold text-lg text-gray-900;
}

p {
  @apply my-4 text-base;
}

p a {
  @apply underline;
}

ul.ul-cols-2 {
  @apply list-disc pl-4 grid grid-cols-2;
}

ul.ul-cols-2 li {
  @apply mb-1;
}

svg.svg-icon-sky {
  @apply w-6 h-6 mr-1.5 stroke-sky-600;
}
</style>

<script setup>
import { AcademicCapIcon, ArrowRightIcon, BriefcaseIcon, EnvelopeIcon, GlobeAltIcon, MapPinIcon } from '@heroicons/vue/24/outline'

const components = {
  AcademicCapIcon,
  ArrowRightIcon,
  BriefcaseIcon,
  EnvelopeIcon,
  GlobeAltIcon,
  MapPinIcon,
}
</script>