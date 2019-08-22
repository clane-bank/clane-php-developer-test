![alt text](https://avatars3.githubusercontent.com/u/17319994?s=200&v=4)
## Clane Backend Software Engineer Test

Hello and thanks for taking the time to try this out.

The goal of this test is to assert (to some degree) your coding and architectural skills. You're given a simple problem so you can focus on showcasing development techniques. We encourage you to overengineer the solution a little to show off what you can do - assume you're building a production-ready application that other developers will need to work on and add to over time.

The test should be written in PHP. We would also encourage you to use [Laravel/Lumen](https://lumen.laravel.com/) as it is our framework of choice. You are required to demonstrate being comfortable coding in PHP, to maximise your chance of a positive code review.

You're **allowed and encouraged** to use third party libraries,be prepared to answer some questions about those libraries, like why you chose them and what other alternatives you're familiar with.

_Note: Send us the link to your repository on github when you're done the test. This challenge is only shared with people interviewing, and for obvious reasons we'd like it to remain this way._

## Prerequsites

We use [Docker](https://www.docker.com/products/docker) to administer this test. This ensures that we get an identical result to you when we test your application out, and it also matches our internal development workflows. If you don't have it already, you'll need Docker installed on your machine. **The application MUST run in the Docker containers** - if it doesn't we cannot accept your submission.

### Technology

- Valid PHP 7.2
- Persist data to either Postgres or Mysql
- You can also use Redis (if and/or where applicable)
- Use a `docker-compose.yml` version 3 to  define and run your containers.

## Requirements

We'd like you to build a simple Articles API. The API **MUST** conform to REST practices and **MUST** provide the following functionality:

- List, create, read, update, and delete articles
- Search articles
- Rate articles

### Endpoints

Your application **MUST** conform to the following endpoint structure and return the HTTP status codes appropriate to each operation. Endpoints specified as protected below **SHOULD** require authentication to view. The method of authentication is up to you.

##### Articles

| Name   | Method      | URL                     | Protected |
| ---    | ---         | ---                     | ---       |
| List   | `GET`       | `/articles`             | ✘         |
| Create | `POST`      | `/articles`             | ✓         |
| Get    | `GET`       | `/articles/{id}`        | ✘         |
| Update | `PUT/PATCH` | `/articles/{id}`        | ✓         |
| Delete | `DELETE`    | `/articles/{id}`        | ✓         |
| Rate   | `POST`      | `/articles/{id}/rating` | ✘         |

An endpoint for article search functionality **MUST** also be implemented. The HTTP method and endpoint for the search functionality **MUST** be clearly documented.

## Evaluation criteria

These are some aspects we pay particular attention to:

- Your application **MUST** run within the containers. Please provide short setup instructions.
- The API **MUST** return valid JSON and **MUST** follow the endpoints set out above.
- You **MUST** write testable code and demonstrate unit testing (We encourage you to use PHPUnit or any other kind of **testing** framework).
- You **SHOULD** pay attention to best security practices.
- You **SHOULD** follow SOLID principles where appropriate.
- You do **NOT** have to build a UI for this API.

The following earn you bonus points:

- Your answers during code review
- An informative, detailed description in you readme file
- Setup with a one liner or a script
- Content negotiation
- Pagination
- Using any kind of Database Access Abstraction
- Other types of testing - e.g. integration tests
- Following the industry standard style guide for the language you choose to use - `PSR-4`, etc.
- A git history (even if brief) with clear, concise commit messages.

---

Good luck!
