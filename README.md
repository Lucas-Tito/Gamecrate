# Gamecrate

Gamecrate is a personal web application for cataloging and reviewing video games, inspired by platforms like Letterboxd (for movies) and Backloggd. The project is designed to help users organize, rate, and comment on the games they have played, while also serving as a full stack development exercise using modern technologies.

#### Project Overview

Gamecrate allows users to build their own game library, register details about each game, and keep track of their gaming experiences. Users can search for games using an external API or add games manually if they are not found. Each game entry can include the platform played, a rating, comments, estimated completion time, and completion status.

#### Objectives

- Deliver a functional and visually appealing web application for personal game cataloging and review.
- Practice and consolidate full stack development skills using Vue.js, Spring Boot, PostgreSQL, and Docker.
- Integrate with at least one public games API (such as IGDB or RAWG.io) for automated game search.
- Maintain a modular, well-documented codebase following Clean Architecture principles.

#### Main Features

- User registration and authentication.
- Search for games via an external API and add them to a personal catalog.
- Manual addition of games not found in the API.
- Rate games (0–10), write comments, log estimated completion time, and mark completion status (Not Started, In Progress, Completed).
- Create custom categories to group games.
- List and filter games by platform, rating, date added, completion time, status, or category.

#### Out of Scope

The following features are not included in the initial scope:

- Social features (friends, followers, messaging).
- Automatic game recommendations.
- Integration with game stores (Steam, PSN, etc.).
- Native mobile apps.
- Achievement/trophy tracking.
- Content moderation or reporting mechanisms.
- Multi-language support.

#### Technologies Used

- **Frontend:** Vue.js
- **Backend:** Spring Boot
- **Database:** PostgreSQL
- **Containerization/Deployment:** Docker

#### Database Model

The database is designed with the following main entities:

- **User:** Stores user information (name, email, password hash).
- **Game:** Stores game details (name, description, launch date, image, etc.).
- **Review:** Links users to games, storing ratings, comments, completion time, and status.
- **Category:** Custom categories created by users to group games.
- **Platform:** Platforms on which games can be played.
- **Game_Category / Game_Platform:** Associative tables for many-to-many relationships.

For a detailed entity-relationship diagram, see the file: `Diagrama ER de banco de dados (pé de galinha).pdf`.

#### Requirements

**Functional Requirements:**

- Register and authenticate users.
- Search and add games via external API.
- Add games manually.
- Rate and review games.
- Create and manage custom categories.
- List and filter games by various criteria.

**Non-Functional Requirements:**

- Intuitive and modern user interface.
- Responsive design for desktop and mobile.
- Data security (encryption, secure authentication).
- Accessibility best practices.
- Stable integration with external APIs.

#### Documentation

- All project documentation, including architecture, API usage, and deployment instructions, is available in the Docs folder.
- For more details, refer to the `Requisitos.pdf` and `Escopo.pdf` files.

