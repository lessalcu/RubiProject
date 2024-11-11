# RubyProject

**RubyProject** is a simple web application built with Ruby and Sinatra, which responds with a "Hello World!" message when you access the server root. This project is dockerized to make it easy to deploy and run in any environment.

## Project Structure

```
RubyProject/
│
├── Dockerfile # Dockerfile to build the container image
├── Gemfile # Ruby dependency file
├── app.rb # Main file with the application code
└── README.md # Project documentation
```

## Requirements

1. **Docker** (if you want to run the application in a container).
2. **Ruby** (if you want to run the application locally).
3. **Bundler** (if you want to manage Ruby dependencies locally).

## Installation

### Clone the Repository

1. Clone the repository to your local machine:

```bash
git clone https://github.com/lessalcu/ruby-project.git
cd ruby-project
```

### Run Locally

If you prefer to run the application locally:

1. Make sure you have **Ruby** and **Bundler** installed. Then, install the dependencies:

```bash
bundle install
```

2. Run the application with the following command:

```bash
ruby app.rb
```

3. Access the application at `http://localhost:4567/`. You should see the message **"Hello world from Ruby, Lesly Salas SI08!"**.

### Run with Docker

1. If you prefer to use Docker, first build the container image:

```bash
docker build -t lssalas/ruby-project .
```

2. Then, run the container with the following command:

```bash
docker run --name ruby-project -p 4567:4567 lssalas/ruby-project
```

3. The application will be available at `http://localhost:4567/`.

## Notes

- Make sure you have Docker running if you are using containers.
- If you encounter any problems accessing `http://localhost:4567/`, verify that the port is not in use or check your firewall settings.

## Credits

Project developed by **Lesly Salas** (https://github.com/lessalcu).