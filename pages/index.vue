<template>
  <NavigationBar />
  <div class="mx-24">
    <div class="flex justify-center items-center gap-10">
      <div>
        <div class="text-5xl font-bold w-80">
          Hello, Welcome to my Blogs
        </div>
        <div class="flex flex-col mt-5">
          I talk about my experiances and share my knowledge here
        </div>
      </div>

      <div>
        <img class="w-64 h-64" src="images/cat.png">
      </div>
    </div>
  </div>

  <div class="grid gap-3 mt-10">
    <nuxt-link
      href="/blog"
      class="btn btn-primary w-fit mx-auto px-10"
    >
      Go to Blogs
    </nuxt-link>

    <div class="flex justify-center">
      <div class="max-w-3xl mt-10 flex flex-col justify-center items-center">
        <div class="text-3xl font-bold">
          A little bit about me
        </div>

        <div class="mt-5 text-justify">
          In short, I am a curious and innovative Software Developer. I do not have a precise focus area, but I like spending time solving
          data structure and algorithms. I am also a web developer with an hands on experiance on real world enterprise level applications.
          And one last thing, AI and ML. I have a plan of giving my time and work on ML projects. So, that is all about me in short. I would
          be very happy to share my experiances and knowledge. That is why I created this blog. Hope you enjoy and learn something.
        </div>
      </div>
    </div>
    <Background/>
  </div>
</template>
