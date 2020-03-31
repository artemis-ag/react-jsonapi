
# React JSONAPI

## Introduction

We currently have ample opportunity to create a state management and data fetching tool for react, that would support all [JSONAPI-SPEC](https://jsonapi.org/) compliant api's. Because JSONAPI-SPEC is fully documented and follows a set standard, we can use query languages and their syntax (like graphql) or plain json objects/urls to request data from the server.
 
## Code Standards
Most eslint styles and configs are yet to be determined, but we know we want the following things:

 1. Simple React Hooks
 2. Leverage react context whenever possible
 3. Favor functions over classes if/when reasonable
 4. Test Driven Development using react-test-library and jest/enzyme
 5. Strictly typed whenever possible
 6. Low foot print, whenever possible

## What needs to be done?
Data fetching support for the following JSONAPI standard
 - [ ] Support for interception and pipe for requests and responses (i.e. apollo link)
 - [ ] Support for base routes (/users, /posts)
 - [ ] Support for basic route crud
 - [ ] Support for sparse fields (/articles?fields[articles]=title,body)
 - [ ] Support for relationships (/articles?include=author)
 - [ ] Support for sorting
 - [ ] Support for pagination
 - [ ] Support for filters
 - [ ] Support for updating relationships
 - [ ] Support for JSONAPI compliant errors

 State Management support for the following
 - [ ] Mapping relationships to models in state
 - [ ] Cache management and cache busting for state
 - [ ] Support for Polymorphic relationships (maybe a stand in model?, or oneOf syntax?)
 - [ ] Optimistic and Pessimistic ui updates
 - [ ] Simple, declarative api, using hooks and a simple query/mutation model (maybe take lead from graphql)
 - [ ] Top Down state management that is transactional
 - [ ] Support for History i.e. redux history/time traveling
 - [ ] Support for lazy loading
