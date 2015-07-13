# POSTMAN tests for our API

We would like to have a full set of POSTMAN-scripts to test our REST-API. POSTMAN is a Chrome-extension. See: https://www.getpostman.com/

We need a full collection of requests. For each request we need test. See: https://www.getpostman.com/docs/jetpacks_writing_tests

To be able to contribute you need:
- basic knowledge of HTTP and REST-API's
- basic knowledge of Javascript
- the POSTMAN Chrome-extension
- the Jetpack (https://www.getpostman.com/features#jetpacks) -> **contact us, we will buy you a license!**

The API-documentation is here: https://github.com/mobbr/mobbr-api-v1/#mobbr-crowdpayment-rest-api-v1 and here https://test-api.mobbr.com

# How to contribute?

To reward the work you do, we will pledge BTC to the issues. As soon as the issue is closed, the money will be divided. We use MOBBR for this. Just click the Mobbr-link in the issue description for details. 

Your workflow will probably be something like:
- add a comment to the issue to inform others know you are working on it
- discuss any collaboration through the issue comments
- construct/record a set of requests into a collection
- add tests to each request
- ask us for specifications and clarification in the issue comments whenever specs are not obvious, start with the 'simple, trivial' cases
- commit the JSON containing the request and tests to this repo

To use the scripts in Postman, import your local Git files and run them.

**important** 

Make sure to make your tests resistant to database resets. So don't use dynamically generated or volatile properties such as dates, ID's, etc. to test for correctness of results. Check a response using data you entered in the request as much as possible.

#Instructions first milestone

https://github.com/mobbr/mobbr-api-testscripts/milestones/Simple%20endpoint%20test

The simple endpoint/unit tests.

Create a basic set of tests for each method/endpoint. An additional request for each additional default parameter. Do some obvious checks on the limits/ranges of the parameters. Try some obvious illegal values. Once this basic collection has been established, we will create a new milestone with more detailed test specifications and pledge additional BTC to that.

Use the TEST-API on https://test-api.mobbr.com, authenticate using username test1, test2, test3, test4. Password for these accounts is 'm0bbr2014'.

Make each request using:
- no authentication
- basic authentication
- token authentication

Use the JSON-request and reply format: https://github.com/mobbr/mobbr-api-v1/#request-format
