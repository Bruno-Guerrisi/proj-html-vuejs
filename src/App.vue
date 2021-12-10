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
        </main>
        
    </div>
</template>

<script>
import NavHeader from '@/components/NavHeader.vue'
import MainIntro from '@/components/MainIntro.vue'
import Statistics from '@/components/Statistics.vue'
import AboutMe from '@/components/AboutMe.vue'
import Courses from '@/components/Courses.vue'
import Bookstore from '@/components/Bookstore.vue'

export default {
    name: 'App',
    components: {
        NavHeader,
        MainIntro,
        Statistics,
        AboutMe,
        Courses,
        Bookstore,
    },
    data() {
        return {

            courses: [
                {
                    poster: require('@/assets/img/motivation-course-06-480x298.jpg'),
                    dollars: '30',
                    cents: '00',
                    description: 'How to be Successful: Create A Growth Mindset For Success',
                    lesson: 3,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-05-480x298.jpg'),
                    dollars: '30',
                    cents: '00',
                    description: 'How to Build Confidence in Your Abilities',
                    lesson: 1,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-04-480x298.jpg'),
                    dollars: '20',
                    cents: '00',
                    description: 'Productivity Machine - Focus in a Distracted World',
                    lesson: 1,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-03-480x298.jpg'),
                    dollars: '20',
                    cents: '00',
                    description: 'Effective Time Management Mastery - Complete Guide',
                    lesson: 18,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-02-480x298.jpg'),
                    dollars: '25',
                    cents: '99',
                    description: 'Body Language Secrets for Entrepreneurs',
                    lesson: 19,
                    students: 50,
                },
                {
                    poster: require('@/assets/img/motivation-course-01-480x298.jpg'),
                    dollars: '19',
                    cents: '99',
                    description: 'Management Skills: The Science of Leadership',
                    lesson: 17,
                    students: 50,
                },
            ],
        }
    }
}
</script>

<style lang="scss">
@import '@/style/global';
@import '@/style/variables';

header{
  z-index: 4;
}

</style>
