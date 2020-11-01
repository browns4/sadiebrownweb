<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Me"
      subtitle=" "
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Hey! </h3>
          <p>
            <strong>
            My name is Sadie.
            </strong>
          </p>
          <p>
            I was born in Southern California, I grew up in the mountains of San
            Burnadino I was fascinated with snow and loved playing with my dogs
            and older sister. We moved down the mountain, into a house in Redlands.
            We moved for a couple reasons it was closer to work and school which
            also gave for more opportunities for activities outside of school. I played
            soccer for a little but then ended up joining the YMCA circus and found a
            passion for hanging upside down or flying through the air.
            <br />
            When I was in 6th grade my family moved to Portland, Oregon. I went to a very small
            high school which focused on community learning. I continued my love for circus
            through out middle school and into high school. In high school I also for a love
            for competitive swimming and an apperception for running cross country and attempts
            in pole vaulting.
            <br />
            The summer before my freshman year I got my first job as a swim instructor working for Portland
            Parks and Recreation. I worked everyday in the summer teach kids ages 2-12.
            It was a pretty good first job, I learned a lot about communication through
            taking to parents about their child's progress as well as through talking to
            my boss about my responsibilities. I also learn time management skills and
            lesson planning. I did this job for a couple of summers- I loved working
            with kids especially because it was outside in a pool on a hot day.
            <br />
            Through out the school year in highschool I worked at The Circus Project. A
            similar job on paper- instructing people, time management, and communication
            but this job opened up a little more freedom in choosing what skills i taught
            based on what I thought the student was ready for. This job was slightly more
            fun because in most cases the child or individual chose to be there. They
            were taking a circus class not just for the skill but for fun and personal
            growth. From this experience I learned how to have the skill to teach while
            also understanding where a student was at and where their potential is and
            taking to the student about that one on one. 

          </p>

          <h3>Another Fake Heading</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci
            eligendi impedit inventore ipsa laboriosam libero magnam modi odio,
            sunt temporibus. Distinctio doloremque eum magni nostrum quasi
            ratione rem repudiandae sit!
          </p>
          <quote-card />
          <h3>Still More Fake Content</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci
            eligendi impedit inventore ipsa laboriosam libero magnam modi odio,
            sunt temporibus. Distinctio doloremque eum magni nostrum quasi
            ratione rem repudiandae sit! Lorem ipsum dolor sit amet, consectetur
            adipisicing elit.
            <strong>Alias aut facere harum ipsam</strong> quibusdam quidem
            quisquam saepe? Alias architecto blanditiis consequatur consequuntur
            dicta ipsa iste modi provident, quod, similique veritatis.
          </p>
        </div>

        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Cool Stuff We Do
              </p>
              <p class="subtitle">
                Sooo Cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Other Cool Things
              </p>
              <p class="subtitle">
                Just as cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                All the cool
              </p>
              <p class="subtitle">
                that is all
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
