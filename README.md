http://github.com/bensomers/firefox-buildpack
http://github.com/buitron/geckodriver-buildpack
BUILDPACK_URL http://github.com/bensomers/firefox-buildpack
DATABASE_URL postgres://zuamvikoayfzqy:4195ea9f831c2872cee6531d525b8a60677e150439cf8917fd0dfad9c2655d0a@ec2-52-23-45-36.compute-1.amazonaws.com:5432/dccfq2af8345n5
# java-getting-started  sdfsdf

A barebones Java app, which can easily be deployed to Heroku.

This application supports the [Getting Started with Java on Heroku](https://devcenter.heroku.com/articles/getting-started-with-java) article - check it out.

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Running Locally

Make sure you have Java and Maven installed.  Also, install the [Heroku CLI](https://cli.heroku.com/).

```sh
$ git clone https://github.com/heroku/java-getting-started.git
$ cd java-getting-started
$ mvn install
$ heroku local:start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

If you're going to use a database, ensure you have a local `.env` file that reads something like this:

```
JDBC_DATABASE_URL=jdbc:postgresql://localhost:5432/java_database_name
```

## Deploying to Heroku

```sh
$ heroku create
$ git push heroku main
$ heroku open
```

## Documentation

For more information about using Java on Heroku, see these Dev Center articles:

- [Java on Heroku](https://devcenter.heroku.com/categories/java)
