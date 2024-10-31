 TDS Project 1 - GitHub User and Repository Data Collection of Chicago City

## Overview
This project involves collecting and analyzing data about GitHub users in Chicago who have over 100 followers and repositories. The data includes user profiles and their associated repositories, which will be stored in CSV files for further analysis. The project utilizes the GitHub API to fetch this data.

## Usage

1. Ensure you have a valid GitHub personal access token. Create one if you don't have it yet.
2. Update the `GITHUB_TOKEN` variable in the script with your token.

The script will fetch user data and their repositories, saving them in `users.csv` and `repositories.csv`.

## Data Collection

- The user data collection script fetches users based in Chicago with more than 100 followers and repositories.
- Repositories are fetched in parallel to optimize the data retrieval process.
- The collected data is saved in CSV format for easy analysis.

## CSV File Formats

Data is saved in two CSV files:
  - `users.csv`: Contains user profile data.
  - `repositories.csv`: Contains repository data for each user.
    
### `users.csv`

| Column          | Description                                   |
|-----------------|-----------------------------------------------|
| login           | GitHub username                               |
| name            | Full name of the user                         |
| company         | Company associated with the user              |
| location        | User's location                               |
| email           | User's email address                          |
| hireable        | Hireable status                               |
| bio             | User's bio                                    |
| public_repos    | Number of public repositories                 |
| followers       | Number of followers                           |
| following       | Number of users followed                      |
| created_at      | Account creation date                         |

### `repositories.csv`

| Column          | Description                                   |
|-----------------|-----------------------------------------------|
| repo_name       | Name of the repository                        |
| description     | Repository description                        |
| url             | URL to the repository                         |
| language        | Primary programming language used             |
| stars           | Number of stars                               |
| forks           | Number of forks                               |
| created_at      | Repository creation date                      |
| updated_at      | Last updated date of the repository           |

## Contributing

Feel free to contribute by submitting a pull request or opening an issue for any suggestions or bugs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


