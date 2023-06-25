<template>
  <div class="banner-conatiner">
        <div class="banner-text-block">
            <div class="last-title-btn"> 
                <h2 class="fr-last-title">Flashcard Portfolio Demo SaaS Project</h2>
            </div>
            <div class="banner-first-row">
                <div class="fr-column">
                    <h3 class="fr-content">
                        <p>Hello and thank you for taking the time to visit our site! My name is Lance Nines and 
                        I'm excited to share with you a project that I worked on during my time at Tech Elevator. 
                        This web application was developed in collaboration with my classmates in an Agile environment.</p>
                        <p>As a member of our Agile team of five developers, I played an integral role in designing and implementing the backend logic of our web application using Spring Boot.
                        We followed the MVC design pattern and coordinated project aspects to deliver MVP features for a product owner through personal sprints.
                        We had daily standup meetings to go over our progress with our project manager, who was an instructor at Tech Elevator.
                        Our team designed a REST API that enables access to a PostgreSQL database for CRUD operations and implemented responsive UI/UX design principles in the Vue.js frontend.</p>
                        <p>I was responsible for setting up the REST API in Java using Spring Boot and creating the CRUD operations for the REST API.
                        I also worked very closely with my teammates to integrate components of the Vue.js frontend.
                        We placed a strong emphasis on pair-programming and integration testing to ensure that all components of the web application worked seamlessly together.
                        Through our collaborative efforts, we were able to deliver a well-rounded web application that met our project goals.</p>
                        <p>Since completing the project, I have continued to expand my skills by learning how to deploy this app as a SaaS application on Google Cloud using App Engine and containerization with Docker.
                        I have migrated my pgAdmin database to a Cloud SQL instance and updated my Spring Boot app's configuration to use Cloud SQL for database access.
                        The logic for creating, storing, editing, and testing decks is handled by the backend and stored in a Cloud SQL database.</p> 
                        <p>This project showcases my ability to work in a team environment and utilize modern development tools and techniques.
                        Please check out the <a class="external-link"  target="_blank" href="https://github.com/ninesl/flashcards">github repo here</a>!</p>
                    </h3>
                </div>
                <div class="fr-image" id="fr-img">
                    <img id="desk-notebook" src="..\assets\pexels-pixabay-459791.jpg" alt="Desk with notebook" width="100%" height="auto">
                </div> 
            </div>

        </div>
    </div>
</template>

<script>

export default {
    name: 'the-banner',
    methods: {
        goToRegister() {
            this.$router.push({name: 'register'});
        }
    }
}
</script>

<style scoped>
p {
    font-size: 18px;
    text-align: justify;
}
.external-link {
    color: blue;
}

#desk-notebook {
    border-radius: 10px;
    box-shadow: 2px 3px 5px;
    margin-top: 10px;
}
.banner-f-title {
    text-align: center;
    text-shadow: 1px 1px 1px rgba(57, 158, 57, 0.76);
    font-size: 2em;

}

.banner-first-row {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 20px;
    overflow: hidden;
}

.fr-title {
    font-size: 2em;
}
.fr-column {
    width: 50%;
}
.fr-image {
    margin-left: 5%;
    width: 50%;
}

.last-title-btn {
    display: flex;
    justify-content: center;
    align-items: baseline;
    margin: auto;
}

.fr-last-title{
    text-align: center;
    text-shadow: 3px 3px 5px rgba(57, 158, 57, 0.76);
    font-size: 2em;
}

#last-btn-shaped{
    border-radius: 16px;
    padding: 12px 24px;
    margin-left: 10px;
}

@media only screen and (max-width: 1300px) {
    .last-title-btn {
        flex-direction: column;
        align-items: center;
    }
    .banner-first-row {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    .fr-column, .fr-image {
        margin: 10px;
        width: 100%;
        padding: 0;
    }
    .fr-title {
        margin: auto;
        text-align: center;
    }

}
/* 
@media only screen and (max-width: 590px) {

    .fr-content {
        max-width: 60%;
    }

}

@media only screen and (max-width: 500px) {

    .fr-content {
        max-width: 50%;
    }

}

@media only screen and (max-width: 400px) {

    .fr-content {
        max-width: 40%;
    }

} */

</style>
