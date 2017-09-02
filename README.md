# Earthquake List

## The brief

- Create a react component that displays a list of places where earthquakes have happened.
- List should be filterable by `magnitude` or `magtype` of the earthquake. 
- If the filter does not return any items then display a message to say ‘not found’. 
- You should use React, ES6 and Redux if you think appropriate. 
- Create some (not necessary to unit test everything) tests to show the app works (using either Jasmine or Mocha). 
- Please provide two solutions if you can and the pros and cons of each approach.
- Do not worry about resetting the filters or styling. 
- Pay attention to reusing and composing components where possible.

Use the following endpoint:
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&starttime=2014-01-01&endtime=2014-01-02

The list items should display in the following format

`Id: place: mag: magType`

e.g.

```
- Ak10992887: 117km NW of Talkeetna, Alaska : 1.1 : ml
- Nc72134401 : 6km E of Mammoth Lakes, California : 0.6 : md
```

Create two inputs with buttons:

1. Text Input with button to filter by magnitude
2. Text Input with button to filter by magtype


## Notes on two approaches

### Solution 1

Intention: Quick approach without too much concern for tooling and the 
structure of that app beyond the component itself.

- Use [Create React App](https://facebook.github.io/react/docs/installation.html) to get started quickly
- Use [TDD](https://technologyconversations.com/2014/09/30/test-driven-development-tdd/) 
 and an [XP](https://en.wikipedia.org/wiki/Extreme_programming) approach to fulfill the business logic as efficiently as possible.
- Don't worry about PropTypes (interesting talking point)

#### Still to do:

- Improve test coverage 
    - around the filters
    - around data being returned in unexpected format

- Import `isomorphic-fetch` and mock 


### Solution 2

Intention: A more carefully crafted app, some exploration into 
technology which is less familiar and more time setting up tooling to 
encourage best practice and consistent and high quality code.

- Configure Babel, Webpack and NPM scripts from scratch (don't use create-react-app)
- Incorporate tooling that encourages best practice (e.g. ESLint, AirBnb rules)
- (Try) Jest for unit tests
- (Maybe) Demonstrate state handling using Redux -- although there's not enough complexity to really warrent it

#### Still to do

*Solution 2 has not been started*

---

### Still to do both both solutions

- Consider publishing build versions of both solutions to GitHub pages.
    + Move each solution to it's own repo
    + Provide links to repos and Git Hub pages from this repo.
