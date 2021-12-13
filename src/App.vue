<template>
    <div id="app">

        <header>
            <NavHeader />
        </header>

        <main>
            <MainIntro />

            <Statistics />

            <AboutMe />

            <Courses :listCourses="courses"/>

            <Bookstore />

            <Sponsorimage :listSponsor="sponsor"/>

            <Stories />

            <Articles :listArticles="articles"/>
        </main>

        <footer>

            <Footer />
        </footer>

        <Navright />

    </div>
</template>

<script>
import NavHeader from '@/components/NavHeader.vue'
import MainIntro from '@/components/MainIntro.vue'
import Statistics from '@/components/Statistics.vue'
import AboutMe from '@/components/AboutMe.vue'
import Courses from '@/components/Courses.vue'
import Bookstore from '@/components/Bookstore.vue'
import Sponsorimage from '@/components/Sponsorimage.vue'
import Stories from '@/components/Stories.vue'
import Articles from '@/components/Articles.vue'
import Footer from '@/components/Footer.vue'
import Navright from '@/components/Navright.vue'

export default {
    name: 'App',
    components: {
        NavHeader,
        MainIntro,
        Statistics,
        AboutMe,
        Courses,
        Bookstore,
        Sponsorimage,
        Stories,
        Articles,
        Footer,
        Navright,
    },
    data() {
        return {

            courses: [
                {
                    poster: require('@/assets/img/motivation-course-06-480x298.jpg'),
                    dollars: '30',
                    cents: '00',
                    title: 'How to be Successful: Create A Growth Mindset For Success',
                    lesson: 3,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-05-480x298.jpg'),
                    dollars: '30',
                    cents: '00',
                    title: 'How to Build Confidence in Your Abilities',
                    lesson: 1,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-04-480x298.jpg'),
                    dollars: '20',
                    cents: '00',
                    title: 'Productivity Machine - Focus in a Distracted World',
                    lesson: 1,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-03-480x298.jpg'),
                    dollars: '20',
                    cents: '00',
                    title: 'Effective Time Management Mastery - Complete Guide',
                    lesson: 18,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-02-480x298.jpg'),
                    dollars: '25',
                    cents: '99',
                    title: 'Body Language Secrets for Entrepreneurs',
                    lesson: 19,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-01-480x298.jpg'),
                    dollars: '19',
                    cents: '99',
                    title: 'Management Skills: The Science of Leadership',
                    lesson: 17,
                    students: 50,
                },
            ],

            sponsor: [ 'client-logo-05-primary',
                        'client-logo-06-primary',
                        'client-logo-07-primary',
                        'client-logo-04-primary',
                        'client-logo-03-primary',
                        'client-logo-02-primary',
                        ],

            articles: [
                {
                    poster: require('@/assets/img/motivation-blog-04-480x325.jpg'),
                    date: 'May 13, 2020',
                    title: 'How to Stay True to Your Personal Brand',
                    description: 'When it comes to your business or career, you want ...',
                },
                {
                    poster: require('@/assets/img/motivation-blog-03-480x325.jpg'),
                    date: 'May 13, 2020',
                    title: '5 Vital Lesson in 5 Years of Freelancing',
                    description: "Being self-employed and working from home, it's easy to get ...",
                },
                {
                    poster: require('@/assets/img/motivation-blog-02-480x325.jpg'),
                    date: 'May 13, 2020',
                    title: '11 Super Useful Tips for Small-Business Owners',
                    description: 'Being a small-business owner poses a ton of challenges. We ...',
                },
                {
                    poster: require('@/assets/img/motivation-blog-01-480x325.jpg'),
                    date: 'May 13, 2020',
                    title: 'How to Give Yourself Grace to Start Again',
                    description: 'Forgive yourself for bad habits you may have started or ...',
                },
            ],
        }
    }
}
</script>

<style lang="scss">
@import '@/style/global';
@import '@/style/variables';

#app{
    position: relative;
}

header{
  z-index: 4;
}

footer{
    background-color: #171621;
    padding: 40px 0 20px;

    color: white;
}

</style>
