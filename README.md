# Ruby on Rails Email Verification

## Overview

This repository demonstrates the implementation of email verification in a Ruby on Rails application using a verification code. Email verification is a vital security feature that ensures the authenticity of user accounts.

## Screenshots

![Email Verification](app/assets/images/screen.png) 


## Getting Started

Clone this repository to your local development environment:

1. Clone the repository:

```bash
git clone https://github.com/DeVuDeveloper/email-verification.git
cd email-verification
```

2. Install the required gems:

```bash
 bundle install
 bin/setup
```

3. Set up the database:

```bash
  rails db:create
  rails db:migrate
  rails db:seed
```


4. Run the server(Open your Browser and navigate to url: http://localhost:3000/): 

```bash
  bin/dev
```


## Dependencies

The Email Verification relies on the following main dependencies:

- Ruby on Rails: The web application framework used to build the app.
- Devise: A flexible authentication solution for Rails.
- Stimulus: JavaScript framework used to enhance interactivity on web pages and applications.
- Tailwind CSS: A utility-first CSS framework for styling the app.

## Linter

The Hotel App includes a linter. You can run the linter with the following command:

```bash
  rubocop && rubocop -A
  npm run lint && npm run lint:fix
```

## Tests

The Hotel App includes a test suite using RSpec. You can run the tests with the following command:

```bash
  rspec spec
```

## Background Jobs

This project uses background jobs for efficient email verification:

- **SendPinJob:** Sends verification codes to users' email addresses.
- **UpdateUserJob:** Updates the user's verification status.

## The Verify Controller

The `VerifyController` manages the email verification process:

- **new:** Displays the verification code input form.
- **create:** Sends verification codes to user email addresses.
- **edit:** Provides a form for entering verification codes.
- **update:** Validates entered codes and marks emails as verified.

## Stimulus Controller

A Stimulus controller improves the user experience by automatically focusing on the next input field after each code digit is entered.


## Built With 🔨

<div align="center">

|     | Languages                                                                                                                                                                                                                                                                                                                  |     |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --- |
|     | ![Ruby](https://img.shields.io/badge/-Ruby-000000?style=flat&logo=ruby&logoColor=red)![Ruby on Rails](https://img.shields.io/badge/-Ruby_on_Rails-000000?style=flat&logo=ruby-on-rails&logoColor=blue)![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)!![JavaScript](https://img.shields.io/badge/javascript-%23316192.svg?style=for-the-badge&logo=javascript&logoColor=white)![Stimulus](https://img.shields.io/badge/Stimulus-%23316192.svg?style=for-the-badge&logo=javascript&logoColor=white) |

<div align="center">


|     | Tools 🛠️                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --- |
|     | ![RSpec](https://img.shields.io/badge/RSpec-%23FF5545.svg?style=for-the-badge&logo=ruby&logoColor=white)![Jest](https://img.shields.io/badge/Jest-%23C21325.svg?style=for-the-badge&logo=jest&logoColor=white)![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) ![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white) ![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) |     |

<p align="right">(<a href="#top">back to top</a>)</p>
</div>

## Authors ✍️

<div align="center">

| 👤 DeVuDeveloper|
| -------- |

| <a target="_blank" href="https://github.com/DeVuDeveloper"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white" alt="Github profile"></a> <a target="_blank" href="https://www.linkedin.com/in/devuj/"><img src="https://img.shields.io/badge/-LinkedIn-0077b5?style=for-the-badge&logo=LinkedIn&logoColor=white" alt="Linkedin profile"></a> <a target="_blank" href="https://twitter.com/DejanVuj"><img src="https://img.shields.io/badge/-Twitter-1DA1F2?style=for-the-badge&logo=Twitter&logoColor=white" alt="Twitter profile"></a>
|

</div>

<p align="right">(<a href="#top">back to top</a>)</p>

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

This project was inspired by the need for secure user authentication.
Special thanks to the Ruby on Rails community for valuable resources and guidance.
