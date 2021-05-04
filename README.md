# Example LTI Tool Provider Using ims-lti Gem

This is a basic and simple LTI Tool Provider that uses the
[ims-lti](https://github.com/instructure/ims-lti) gem.
To get this running in your development environment, check out the repo then:

    bundle install
    bundle exec shotgun -o 0.0.0.0

If you'd rather run the app using docker a docker-compose file is included:

    docker-compose run --rm web bundle install
    docker-compose up

If you're using dinghy on OS X you'll be able to visit the app at: http://lti1-example.docker/

You can use the XML from the `/tool_config.xml` endpoint to configure the tool in a Tool Consumer.

You can use this with the [example LTI Tool Consumer](https://github.com/firstdraft/lti_tool_consumer_example)
to do some simple LTI testing.
