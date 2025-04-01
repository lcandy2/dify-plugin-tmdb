# Dify Tool Plugin - The Movie Database (TMDB)

This plugin allows you to search The Movie Database (TMDB) for movies, TV shows, and people. It provides comprehensive metadata and information from TMDB's extensive entertainment database.

## Features

- **Movie Search**: Search for movies by title, keywords, or phrases
- **TV Show Search**: Search for TV shows by name, keywords, or phrases
- **Multi Search**: Combined search for movies, TV shows, and people in a single request

## Setup

1. Register for a TMDB account at [https://www.themoviedb.org](https://www.themoviedb.org)
2. Generate an API Read Access Token (v4 auth) at [https://developer.themoviedb.org/reference/intro/authentication](https://developer.themoviedb.org/reference/intro/authentication)
3. Install the plugin in your Dify instance
4. Configure the plugin with your TMDB API Read Access Token

## Usage

### Movie Search

Search for movies by title or keywords:

- **Parameters**:
  - `query` (required): Movie title or keywords
  - `language` (optional): ISO 639-1 language code (default: en-US)
  - `year` (optional): Filter by release year
  - `results_limit` (optional): Number of results to return (1-20, default: 5)

### TV Show Search

Search for TV shows by title or keywords:

- **Parameters**:
  - `query` (required): TV show title or keywords
  - `language` (optional): ISO 639-1 language code (default: en-US)
  - `first_air_date_year` (optional): Filter by first air date year
  - `results_limit` (optional): Number of results to return (1-20, default: 5)

### Multi Search

Search for movies, TV shows, and people in a single request:

- **Parameters**:
  - `query` (required): Search keywords
  - `language` (optional): ISO 639-1 language code (default: en-US)
  - `include_adult` (optional): Whether to include adult content (default: false)
  - `results_limit` (optional): Number of results to return (1-20, default: 10)

## Development

### Requirements

- Python 3.12+
- Dify Plugin SDK

### Local Development

1. Clone this repository
2. Create a virtual environment and install dependencies:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Copy `.env.example` to `.env` and configure your development environment
4. Run the plugin:
   ```
   python -m main
   ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This plugin uses the [TMDB API](https://developer.themoviedb.org/docs)
- Data and images provided by [The Movie Database (TMDB)](https://www.themoviedb.org)



