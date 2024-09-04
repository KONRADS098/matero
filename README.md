# Matero

A community-driven platform for yerba mate enthusiasts, offering a comprehensive database of yerba mate products, user reviews, and ratings. This platform allows users to explore, discover, and share their experiences with various yerba mate brands and varieties. Features include detailed product information, personalized collections, a robust search and filter system, and an active community forum for discussions and knowledge sharing. Whether you're a seasoned yerba mate connoisseur or just beginning your journey, this platform serves as the ultimate resource for all things yerba mate.

## Tech Stack

### Frontend

- [React.js](https://reactjs.org/) - Chosen for its component-based architecture and efficient rendering, ideal for building interactive UIs
- [Next.js](https://nextjs.org/) - Selected for its server-side rendering capabilities, optimized performance, and seamless integration with React
- [TypeScript](https://www.typescriptlang.org/) - Adopted to enhance code quality, improve maintainability, and catch errors early in development
- [Tailwind CSS](https://tailwindcss.com/) - Picked for rapid UI development and easy customization without leaving HTML

### Backend

- [Node.js](https://nodejs.org/) - Chosen for its non-blocking I/O and event-driven architecture, suitable for scalable applications
- [Express.js](https://expressjs.com/) - Selected for its minimalist approach and flexibility in building robust APIs
- TypeScript - Used for consistency with the frontend and to maintain a unified development experience

### Database

- [PostgreSQL](https://www.postgresql.org/) - Chosen for its reliability, feature-rich environment, and support for complex queries
- [Redis](https://redis.io/) - Implemented for high-performance caching to improve application responsiveness

### Authentication

- [NextAuth.js](https://next-auth.js.org/) - Selected for its seamless integration with Next.js and support for various authentication providers

### API

- [GraphQL](https://graphql.org/) with [Apollo Server](https://www.apollographql.com/docs/apollo-server/) - Chosen for its flexible querying capabilities and efficient data fetching

### Hosting/Deployment

- [Vercel](https://vercel.com/) - Selected for its seamless integration with Next.js and optimized deployment process
- [Docker](https://www.docker.com/) - Adopted to ensure consistency across development and production environments

### Testing

- [Jest](https://jestjs.io/) - Chosen for its simplicity and comprehensive testing capabilities for JavaScript applications
- [Cypress](https://www.cypress.io/) - Selected for its powerful end-to-end testing features and developer-friendly API

## Features

- Yerba Mate Database
- User Accounts
- Review System
- Search and Filter
- User Collections
- Community Forum

## User Stories and Requirements

### Infrastructure User Stories

1. As a developer, I want to set up the Next.js project with TypeScript so that I can start building the frontend.

   - Requirements:
     - Initialize a new Next.js project with TypeScript support
     - Configure ESLint and Prettier for code quality
     - Set up folder structure for components, pages, and styles
   - Definition of Done:
     - Project successfully initializes without errors
     - ESLint and Prettier configurations are in place and working
     - Folder structure is created and documented

2. As a developer, I want to configure Tailwind CSS in the project so that I can efficiently style components.

   - Requirements:
     - Install and configure Tailwind CSS
     - Create a base set of custom utility classes
     - Set up a theme configuration file
   - Definition of Done:
     - Tailwind CSS is installed and configured correctly
     - Custom utility classes are created and documented
     - Theme configuration file is set up and can be easily modified

3. As a developer, I want to set up the Express.js backend with TypeScript so that I can start building API endpoints.

   - Requirements:
     - Initialize a new Express.js project with TypeScript
     - Set up folder structure for routes, controllers, and models
     - Configure middleware for error handling and request parsing
   - Definition of Done:
     - Express.js project is set up with TypeScript and runs without errors
     - Folder structure is in place and documented
     - Middleware for error handling and request parsing is implemented and tested

4. As a developer, I want to set up PostgreSQL and create initial database schemas so that I can store application data.

   - Requirements:
     - Install and configure PostgreSQL
     - Design and implement database schemas for users, yerba mate products, reviews, and collections
     - Set up database migration scripts
   - Definition of Done:
     - PostgreSQL is installed and configured correctly
     - Database schemas are designed, implemented, and documented
     - Migration scripts are created and successfully run

5. As a developer, I want to implement GraphQL with Apollo Server so that I can create efficient API queries.

   - Requirements:
     - Set up Apollo Server with Express.js
     - Define GraphQL schema for main entities (users, products, reviews)
     - Implement resolvers for queries and mutations
   - Definition of Done:
     - Apollo Server is set up and integrated with Express.js
     - GraphQL schema is defined and documented
     - Resolvers for main entities are implemented and tested

6. As a developer, I want to set up NextAuth.js for authentication so that users can create accounts and log in.

   - Requirements:
     - Install and configure NextAuth.js
     - Implement authentication providers (e.g., email/password, Google, Facebook)
     - Create protected routes and API endpoints
   - Definition of Done:
     - NextAuth.js is installed and configured correctly
     - At least two authentication providers are implemented and tested
     - Protected routes and API endpoints are created and working as expected

7. As a developer, I want to configure Docker for the project so that I can ensure consistent development and deployment environments.

   - Requirements:
     - Create Dockerfiles for frontend and backend services
     - Set up docker-compose for local development
     - Configure environment variables for different deployment stages
   - Definition of Done:
     - Dockerfiles for frontend and backend are created and tested
     - docker-compose file is set up and works for local development
     - Environment variables are configured for development, staging, and production

8. As a developer, I want to set up Jest and Cypress for testing so that I can ensure code quality and functionality.
   - Requirements:
     - Install and configure Jest for unit and integration tests
     - Set up Cypress for end-to-end testing
     - Create initial test suites for critical components and functions
   - Definition of Done:
     - Jest is installed and configured for both frontend and backend
     - Cypress is set up and configured for end-to-end testing
     - Initial test suites are created and passing for critical components and functions

### Feature-based User Stories

9. As a user, I want to view a list of yerba mate brands and varieties so that I can explore different options.

   - Requirements:
     - Create a paginated list view of yerba mate products
     - Display key information for each product (name, brand, average rating)
     - Implement sorting options (e.g., alphabetical, popularity)
   - Definition of Done:
     - Paginated list view is implemented and displays correctly
     - Key information for each product is shown accurately
     - Sorting options are functional and update the list in real-time
   - Acceptance Criteria:
     - List loads within 3 seconds on average internet connection
     - Pagination works correctly, showing the right number of items per page
     - Sorting options change the order of items as expected

10. As a user, I want to search for specific yerba mate products so that I can quickly find information about them.

    - Requirements:
      - Implement a search bar with autocomplete functionality
      - Create a search results page with relevant product information
      - Allow filtering of search results by various criteria
    - Definition of Done:
      - Search bar with autocomplete is implemented and functional
      - Search results page displays relevant information clearly
      - Filtering options for search results are implemented and working
    - Acceptance Criteria:
      - Autocomplete suggestions appear after typing 3 characters
      - Search results load within 2 seconds of submitting a query
      - Filtering options update results in real-time

11. As a user, I want to create an account so that I can participate in the community and save my preferences.

    - Requirements:
      - Implement user registration form with email verification
      - Create user profile page with editable information
      - Set up secure password hashing and storage
    - Definition of Done:
      - User registration form is created and validates input correctly
      - Email verification process is implemented and working
      - User profile page allows editing of information and saves changes
    - Acceptance Criteria:
      - Registration process completes within 1 minute
      - Email verification link is received within 5 minutes of registration
      - Password is securely hashed before storage

12. As a user, I want to rate and review yerba mate products so that I can share my experiences with others.

    - Requirements:
      - Create a rating system (e.g., 1-5 stars)
      - Implement a review form with text input and optional image upload
      - Display user reviews on product pages with pagination
    - Definition of Done:
      - Rating system is implemented and saves ratings correctly
      - Review form accepts text and image uploads successfully
      - User reviews are displayed on product pages with proper pagination
    - Acceptance Criteria:
      - Rating submission is instant and updates the product's average rating
      - Image uploads are limited to 5MB and common image formats
      - Reviews display the user's name, rating, date, and review text

13. As a user, I want to create and manage my personal yerba mate collections so that I can keep track of my favorites and wish list.

    - Requirements:
      - Allow users to create multiple named collections
      - Implement add/remove functionality for products in collections
      - Create a user dashboard to manage collections
    - Definition of Done:
      - Users can create, edit, and delete named collections
      - Products can be added to and removed from collections easily
      - User dashboard displays all collections with management options
    - Acceptance Criteria:
      - Collections are private by default with an option to make them public
      - Adding/removing products from collections is instant
      - User dashboard loads within 2 seconds

14. As a user, I want to view detailed information about a specific yerba mate product, including its flavor profile and characteristics.

    - Requirements:
      - Create a product detail page with comprehensive information
      - Display flavor profile using visual representations (e.g., charts)
      - Show related products or recommendations
    - Definition of Done:
      - Product detail page is created with all relevant information
      - Flavor profile is visually represented and easy to understand
      - Related products or recommendations are displayed accurately
    - Acceptance Criteria:
      - All product information is accurate and up-to-date
      - Flavor profile visualization is interactive and responsive
      - At least 3 related products are shown for each product

15. As a user, I want to filter yerba mate products by various criteria (e.g., brand, flavor profile) so that I can find products that match my preferences.

    - Requirements:
      - Implement a multi-faceted filter system
      - Create an intuitive UI for selecting and applying filters
      - Ensure fast and responsive filtering of results
    - Definition of Done:
      - Multi-faceted filter system is implemented and working correctly
      - UI for selecting and applying filters is user-friendly
      - Filtering results are updated quickly and accurately
    - Acceptance Criteria:
      - At least 5 different filter criteria are available
      - Filters can be combined and removed easily
      - Results update within 1 second of applying or removing filters

16. As a user, I want to participate in forum discussions about yerba mate so that I can engage with other enthusiasts.

    - Requirements:
      - Create a forum system with categories and threads
      - Implement posting, replying, and quoting functionality
      - Add moderation tools for administrators
    - Definition of Done:
      - Forum system with categories and threads is created and functional
      - Users can post new threads, reply to existing ones, and quote others
      - Moderation tools are implemented and available to administrators
    - Acceptance Criteria:
      - Forum posts support basic formatting (bold, italic, links)
      - Users receive notifications for replies to their posts
      - Administrators can pin, lock, and delete threads as needed

17. As a user, I want to view average ratings for yerba mate products so that I can quickly gauge their popularity and quality.

    - Requirements:
      - Calculate and display average ratings for each product
      - Show rating distribution (e.g., percentage of 5-star ratings)
      - Update ratings in real-time when new reviews are submitted
    - Definition of Done:
      - Average ratings are calculated and displayed accurately
      - Rating distribution is shown in an easy-to-understand format
      - Ratings update immediately when new reviews are submitted
    - Acceptance Criteria:
      - Average rating is displayed with one decimal place
      - Rating distribution shows percentages for each star rating
      - New ratings are reflected in the average within 5 seconds

18. As a user, I want the website to be responsive so that I can comfortably use it on both desktop and mobile devices.
    - Requirements:
      - Implement responsive design using Tailwind CSS
      - Ensure all features are accessible and functional on mobile devices
      - Optimize images and assets for different screen sizes
    - Definition of Done:
      - Website layout adjusts appropriately for different screen sizes
      - All features are usable on both desktop and mobile devices
      - Images and assets load quickly on mobile connections
    - Acceptance Criteria:
      - Website is fully functional on devices with screen widths from 320px to 1920px
      - Touch interactions are implemented for mobile users
      - Page load time on mobile devices is under 3 seconds on 4G connection

## Getting Started

<!-- TODO -->

## Contributing

<!-- TODO -->

## License

<!-- TODO -->
