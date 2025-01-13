<script setup>



import { ref } from 'vue'
import { marked } from 'marked'

// const markdown = marked('#Hello World')
// const html = ref(markdown)

const html = ref(marked(`
# TrueVibe Technical Specifications and Project Scope

## Project Overview
This project involves developing a Single Page Application (SPA) using Vue.js and Supabase. The application will enable users to take a quiz, receive a personalized report based on their results, and connect with matched users via a WhatsApp button. A key focus of this project is to create a reusable infrastructure that allows for future scaling without the need for a complete revamp. Additionally, we will prioritize accessibility to ensure that all users can effectively engage with the application.

### User Flows

1. **User Registration/Login**
   - Users can sign up for a new account or log in to an existing account.
   - Authentication will utilize Supabase's robust authentication features, ensuring a secure experience for all users.

2. **Taking the Quiz**
   - Once logged in, users will access a quiz designed with an intuitive & interactive interface.
   - The quiz will consist of multiple-choice questions (MCQs), ensuring a straightforward experience for all participants.

3. **Submitting the Quiz**
   - After completing the quiz, users will submit their responses.
   - The application will process the results and generate a personalized report & Ai generated profile.

4. **Viewing the Report**
   - Users will receive a detailed report based on their quiz results, including insights and recommendations tailored to their responses.

5. **Matching Users**
   - A matching algorithm will analyze quiz results to identify compatible users based on predefined criteria.
   - Matched users will have their profiles accessible for further interaction, promoting community engagement.

6. **Contacting Matched Users**
   - Users can contact matched users through a WhatsApp button, which opens the WhatsApp application with a pre-defined message.

## Technical Specifications

### 1. Frontend
- **Framework**: Vue.js
- **State Management**: Vuex (for managing application state)
- **Routing**: Vue Router (for handling navigation between pages)
- **UI Library**: Vuetify or BootstrapVue (for responsive design and UI components)

### 2. Backend
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth (for user registration and login)
- **API**: Supabase client library for interaction with the database and real-time features.

### 3. Features
- **Quiz Module**:
  - Dynamic quiz creation and management, with focus on reusability for future quizzes.
  - Scoring system based on user responses, ensuring scalability for additional features.

- **Report Generation**:
  - Automated AIreport generation based on quiz results, with flexibility for updates as new insights are developed.
  - Accessibility features to ensure that reports are usable by all individuals, including those with disabilities.

- **Matching Algorithm**:
  - Custom logic for matching users based on quiz results, with an emphasis on scalable criteria that can be adapted as the user base grows.

- **WhatsApp Integration**:
  - Use WhatsApp's API to facilitate direct messaging.
  - Button functionality that opens WhatsApp with a pre-filled message, ensuring ease of communication for all users.

#### Accessibility Focus
- The application will adhere to WCAG (Web Content Accessibility Guidelines) standards to ensure usability for individuals with disabilities.
- Features will include keyboard navigation, screen reader compatibility, and color contrast considerations to enhance user experience for everyone.

### Project Scope

#### Deliverables
1. A fully functional SPA with:
   - User registration and login pages.
   - Interactive Quiz interface designed for accessibility and ease of use.
   - Report generation feature with accessible formats.
   - User matching functionality that is scalable and adaptable.
   - WhatsApp contact button for seamless communication.

2. Documentation:
   - User guide for navigating the application, with an emphasis on accessibility features.
   - Technical documentation for the codebase and architecture, highlighting reusable components and infrastructure.

3. Testing:
   - Unit tests for critical components, ensuring reliability.
   - User acceptance testing (UAT) with a focus on accessibility to ensure the application meets diverse user needs.

### Timeline
- **Phase 1**: Requirements gathering and design (1 week)
- **Phase 2**: Development of frontend components (3 weeks)
- **Phase 3**: Backend integration and database setup (3 weeks)
- **Phase 4**: Testing and bug fixes (2 weeks)
- **Phase 5**: Deployment and user training (1 week)

### Assumptions
- Users have access to the internet and are familiar with using web applications.
- The matching algorithm's criteria will be predefined and agreed upon before development.
- The application will be designed with scalability in mind, minimizing the need for future overhaul.

### Conclusion
This project aims to create an engaging and inclusive platform for users to connect based on deeper vulnerabilities rather than shared surface level interests revealed through a quiz. By leveraging Vue.js and Supabase, the application will provide a modern user experience, a robust backend, and a scalable infrastructure that can grow with its user base. Emphasizing accessibility ensures that all users can participate fully, fostering a diverse and vibrant community.
`))

</script>

<template>

        

        
    <div>
        <!-- <textarea v-model="markdown" @input="html = marked(markdown)"></textarea> -->
        <div v-html="html"></div>
    </div>
    


</template>

<style scoped>  



</style>