# Express, NPM, TDD, CI/CD

[An introduction to NodeJS and Express](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

## Express, Middleware

- **Middleware** refers to software functions that sit between a web application's server and client, processing incoming requests, and generating responses.

- **Express** is the most popular web framework for NodeJS.

- Express is "unopinionated" which means it doesn't force developers to use any specific approach or coding style. You have many choices with Express.

- **Module** self-contained block of code that can be reused in different parts of a program.

- **Modularity** allows us to break down complex programs into smaller, more manageable parts. Readability, easier to debug code, and reuse code.

## NPM (Node Package Manager)

[What is NPM?](https://docs.npmjs.com/about-npm)

- **NPM Version** - 9.6.4

- To install jshint we would use the command `npm install jshint`

## TDD (Test-driven development)

[What is TDD?](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))

- Developers write tests before writing the actual code.

- The process involves three main steps: writing a test for a specific functionality, running the test (which should fail at first), and then writing the code to pass the test.

- Tests are important because they help ensure that the software we develop works correctly and reliably. It's a good way to be confident that the code will work, and helps catch unintended bugs.

- **Three Benefits of Testing** - Bug detection, Code Refactoring, and Faster Development.

- **Individual Pitfalls** - Over-testing, where devs may write too many tests which can make the code harder to maintain. Incomplete Testing, devs may unintentionally miss testing certain things which can lead to issues.

- **Team Pitfalls** - Lack of collaboration, potential duplication of tests. Collaboration and communication are important when writing tests. Partial adoption, where only a few devs on the team use TDD.

## CI/CD (Continuous Integration/Delivery/Deployment)

[CI/CD](https://www.youtube.com/watch?v=k2aNsQKwyOo)

- **Three Benefits of Continuous Integration** - early bug detection, faster feedback loop, smoother collaboration.

- Continuous Delivery (CD) and Continuous Deployment are often used interchangeably with some differences. **Continuous Delivery** focuses on ensuring that software is always in a releasable state (ready to be deployed to prod). **Continuous Deployment** - whenever changes pass necessary tests and checks they are automatically deployed to the prod environment.

- **GitHub** - acts as a central hub for devs to store, collaborate, and manage their code. It integrates well with CI/CD processes, facilitating version control, collaboration, and automation of software build, test, and deployment pipelines.

## Learning Goals

- Looking forward to learning more about writing tests, and CI/CD

## Additional Resources

[nodeJS docs](https://nodejs.org/en/docs)

[npm docs](https://docs.npmjs.com/)

[express docs](https://expressjs.com/en/4x/api.html)

[http status codes](https://www.restapitutorial.com/httpstatuscodes.html)

[supertest](https://github.com/ladjs/supertest)