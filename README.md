# flashcards
Fullstack web application created for school. I worked with an Agile team
with my classmates and did 'mini-sprints' along with daily stand-ups with a Scrum master,
and a product owner. We utilized Spring Boot and Vue.js for this project, along with the MVC design pattern.

The application, also known as Ninja Flashcards, utilizes a pgAdmin database to keep track
of student's flashcards for studying. You can share flashcards with your friends based off just
the URL if set to public, or you can have flashcard decks for private use.

There is also tracking for your study sessions per user. If you're logged in and complete a study session,
your performance based off the deck will be tracked and saved for a later session.

![ERD Schema](schema.png)

One to Many

1 user can have many decks

One to Many

1 deck can have multiple cards

Many to Many

Many decks can have a history of many users (user_deck_history merge table)

![Public Decks](public_decks.jpg)
When you look at public decks, you can see all decks that are marked public. The brain
signifies how well you've done when you've previously saved your score, Red means you need work,
Yellow means you're doing okay, Green means you are good on that topic.
You can also see an edit button for the decks where you are the owner, I'm signed in as Lance in this screenshot.

![Edit Deck](edit_deck.jpg)
Here you can change all aspects of the deck, including if it is private, unlisted or public.
Public will have the deck show on the public decks page.
Unlisted means that anyone can access the deck, but only if they have the link to it.
Private means that only the owner can access it, and it will only show up on My Decks.