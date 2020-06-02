# PRODUCTION CODE: 
software running on production servers to handle live users and data of the intended audience. Note this is different from production quality code, which describes code that meets expectations in reliability, efficiency, etc., for production. Ideally, all code in production meets these expectations, but this is not always the case.

## CLEAN: 
readable, simple, and concise. A characteristic of production quality code that is crucial for collaboration and maintainability in software development.

## MODULAR: 
logically broken up into functions and modules. Also an important characteristic of production quality code that makes your code more organized, efficient, and reusable.

## MODULE: a file. Modules allow code to be reused by encapsulating them into files that can be imported into other files.

# Refactoring Code
- REFACTORING: restructuring your code to improve its internal structure, without changing its external functionality. This gives you a chance to clean and modularize your program after you've got it working.
- Since it isn't easy to write your best code while you're still trying to just get it working, allocating time to do this is essential to producing high quality code. Despite the initial time and effort required, this really pays off by speeding up your development time in the long run.
- You become a much stronger programmer when you're constantly looking to improve your code. The more you refactor, the easier it will be to structure and write good code the first time.

# Writing Clean Code: Meaningful Names
## Tip: _Use meaningful names_
- Be descriptive and imply type - E.g. for booleans, you can prefix with is_ or has_ to make it clear it is a condition. You can also use part of speech to imply types, like verbs for functions and nouns for variables.
- Be consistent but clearly differentiate - E.g. age_list and age is easier to differentiate than ages and age.
- Avoid abbreviations and especially single letters - (Exception: counters and common math variables) Choosing when these exceptions can be made can be determined based on the audience for your code. If you work with other data scientists, certain variables may be common knowledge. While if you work with full stack engineers, it might be necessary to provide more descriptive names in these cases as well.
- Long names != descriptive names - You should be descriptive, but only with relevant information. E.g. good functions names describe what they do well without including details about implementation or highly specific uses.

# Documentation
- In-line Comments - line level **Comments are useful for clarifying complex code** 
- Docstrings - module and function level **Docstrings are surrounded by triple quotes**
## Ex. of Multi-line docstring 
```

	"""Calculate the population density of an area.

    Args:
    population: int. The population of the area
    land_area: int or float. This function is unit-agnostic, if you pass in values in terms of square 
    km or square miles the function will return a density in those units.

    Returns:
    population_density: population/land_area. The population density of a 
    particular area.
    """

```
- Project Documentation - project level such as README.md files