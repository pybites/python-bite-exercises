# Python Bite Exercises for Hactoberfest 2024

Thanks for stopping by. This repo allows you to suggest ideas for exercises and write your own. A nice way to contribute as part of Hacktoberfest 2024!

Before submitting an idea or exercise, [check our existing collection](https://pybitesplatform.com/bites/regular/) to make sure we don't already have something similar.

## How to suggest an idea

1. [Create an issue](https://github.com/PyBites-Open-Source/python-bite-exercises/issues) with a short description of your exercise idea.
2. If you want to write the exercise, mention this in the issue.

## How to write your own exercise

1. Fork this repo. If this is your first exercise, make sure you install install pytest: `uv sync` and the pre-commit hook: `pre-commit install` (we use `ruff` to ensure clean code).

2. Create a new directory with the exercise name (use underscores):
   `cp -r template my_exercise_name`

3. Update `script.py` and `test_script.py` with your exercise code and tests. If you need dependencies, add them with `uv add <dependency>`.

4. Copy the `script.py` file to `script-template.py`, and remove the solution code that you don't want users to see (this version is what users will see when they first open the exercise).

5. Update the `exercise.md` file with:

- level: beginner / intermediate / advanced, we don't accept newbies or intro Bites at this time,
- a couple of tags,
- needed dependencies if applicable (note that some dependencies might not be supported yet on our platform),
- your GitHub user handle to credit,
- the exercise details: title + description.

6. Validate that the code works locally by running the tests in your exercise directory: `uv run pytest --cov=script --cov-fail-under=90 --cov-report=term-missing`

7. Open a PR with your new exercise, and we will review it. Once approved and merged, your exercise will be added to the platform, crediting your GitHub user account as listed in exercise.md. Don't submit more than one exercise per PR.

Thanks for contributing to Pybites' growing collection of Python exercises! 🙏 🐍 📈
