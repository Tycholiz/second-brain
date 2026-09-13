
When designing a formula, you want to include as variables, any of your current variable's dependents.  
- ex. I am making a spreadsheet to calculate RoI by year, and have as a variable `biweeklyContribution: Number`. This variable naturally depends on the person's salary, so instead of `biweeklyContribution` being a constant, we should introduce 2 new constants: `annualSalary: Number` and `contributionPercentage: Number` and make `biweeklyContribution` its own formul derived by multiplying the two.
