# repo-complexity-calculator

# Repo Complexity Collector

This repository contains a Python program that uses the GitHub API to collect various metrics for a given GitHub repository. The collected metrics are used to (roughly) calculate the complexity of that codebase. 

This is a hobby project so the generated score is not meant to be interpreted beyond the amusement. Feel free to fork the repo and change the code to add/remove factors that make sense for your codebase. 

The current code is written to fetch data from public GitHub repositories. You can modify the code to add [GitHub authentication tokens](https://docs.github.com/en/rest/guides/getting-started-with-the-rest-api?apiVersion=2022-11-28#about-tokens) to fetch data from private GitHub repositories.

## Features

- Retrieves the number of contributors.
- Retrieves the number of branches.
- Retrieves the number of open issues.
- Retrieves the number of open pull requests.
- Retrieves the number of lines of code.
- Allows you to specify the number of dependencies.

## Requirements

- Python 3.x
- requests library (can be installed via `pip install requests`)

## Usage

1. Clone the repository:

```bash
git clone https://github.com/your-username/code-metrics-collector.git
```

2. Navigate to the project directory::

```bash
cd repo-complexity-calculator
```

3. Install the required dependencies:

```bash
pip install requests
```

4. Open the `find-complexity-score.py` file and set the OWNER and REPO variables to your desired GitHub repository details.

5. The program will retrieve the metrics for the specified repository and display the complexity score. Currently, there's no baseline or indication what the score means. A future improvement will set a baseline and indicate the complexity level of a repository based on score.

## Customization

To add additional metrics or modify the existing metrics, you can extend the functionality of the program by modifying the respective functions in `find-complexity-score.py`.

## Notes

- Ensure that you have valid GitHub API credentials to avoid rate limiting issues.
- Make sure to review the GitHub API rate limits and usage guidelines for more information.

## License

This project is licensed under the MIT License.


