# README

This is an example of Wallarm FAST running security tests in the CircleCI pipeline. The target application is a vulnerable RoR project.


Build with vuln (should fail): [![CircleCI](https://circleci.com/gh/wallarm/fast-example-circleci-rails-integration/tree/master.svg?style=svg)](https://circleci.com/gh/wallarm/fast-example-circleci-rails-integration/tree/master)

All build results: https://circleci.com/gh/wallarm/fast-example-circleci-rails-integration

## How to reproduce example

1. Create your FAST node and get `WALLARM_API_TOKEN` here https://us1.my.wallarm.com/nodes
2. Fork this repository
3. Add project into Circle CI (first build will fail without `WALLARM_API_TOKEN`)
4. Add env-variable `WALLARM_API_TOKEN` in the project settings 
5. Rerun build. It will find some vulnerabilities

## Useful links

- More about Wallarm FAST: https://wallarm.com/products/fast
- More about CircleCI: https://circleci.com/product/
- Vulnerable Rails application's source code: https://github.com/wallarm/fast-example-rails
- Full FAST documentation: https://docs.fast.wallarm.com

TRY WALLARM FAST NOW: https://fast.wallarm.com/signup
