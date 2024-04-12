# Mutation Testing
## Using Stryker to generate mutants and test them

In this example, 2 basic JS functions are tested using the Jest unit testing library.
- **bmi.js:** which calculates the BMI by pounds, feet and inches
- **gradeToLetter.js**: Returns the corresponding letter for a grade.

The steps to run
- install nodejs
- install stryker using npm ```npm install -g stryker```
- to install the dependencies, run: ```npm install ``` 
- to run the unit test (Jest), use: ```npm test```
- to run the mutation generate using stryker and Jest : ```npx stryker run --reporters html```

The last line generates an HTML file with the name of repoerters/mutation.html which contains the test results for the coverage and also Mutants.

# Exercise
## Getting to know the artifact:
Review the code provided for `gradeToLetter.js` and the  provided `gradeToLetter.test.js` to test the functionality of the function.
## Run the tests
Run the following command: 
    ```npm test```
## Generate mutants
Run the following command: ```npx stryker run --reporters html```
## Open the report
Open the report in the browser: ```open reports/mutation/mutation.html```

## Find Survivors
Find the mutants that survived the mutation testing.

## Use the report to improve the tests
Add test cases for the mutants that survived the mutation testing.

## Redo the tests
Run the previous commands to execute the tests again. Check if there are any other mutants that survived the mutation testing.

## Delivarable Checklist
- [ ] The new gradeToLetter.test.js file with new test cases. (50 Points)
- [ ] The new Stryker report mutation.html file. (50 Points)


