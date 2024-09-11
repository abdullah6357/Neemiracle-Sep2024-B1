# Quote Scraping and Guessing Game
This project scrapes quotes from the "Quotes to Scrape" website, extracts details like the author's name and birthdate, and then allows users to play a game where they guess the author of a randomly selected quote. The user is given up to four chances with progressively easier hints to guess the author correctly.

### Features
1) Quote Scraping: Uses requests and BeautifulSoup to scrape quotes and author details from the website Quotes to Scrape. Author Details:
2) Extracts the author's birthdate from the author's biography page.
3) Guessing Game: The user is given four chances to guess the author of a randomly selected quote, with a series of hints provided after each     incorrect guess.

### Requirements
Make sure you have Python installed along with the following dependencies:

**Python Version:** 3.x

**Libraries:**
1) requests: Used to make HTTP requests to the website.
2) beautifulsoup4: Used to parse HTML content.

### How It Works
##### Scraping Quotes:
The scrape_quotes function visits the homepage of the "Quotes to Scrape" website, extracts the quotes, authors, and their respective biography URLs.
For each author, it follows the biography link and scrapes the birthdate.
The scraped quotes and author information (name, birthdate) are stored in a list of dictionaries.
##### Guessing Game:
The play_game_with_four_chances function randomly selects a quote from the scraped data and asks the user to guess the author.
The user has four chances to guess, and hints (author's birthdate, initials of first and last name) are given after each wrong attempt.
The score is calculated based on correct guesses, and the game ends after one round.



### How to Run the Code
1) Clone the repository or copy the Python code to your local environment.
2) The script will first scrape quotes and author details from the website.
3) After scraping, the guessing game will start. You will be presented with a random quote and can try to guess the author. Use the hints provided if necessary.

 ### Code Explanation
**scrape_quotes():**
Scrapes the homepage of the "Quotes to Scrape" website for quotes and their details (text, author, and birthdate)

**scrape_author_bdate(url):**
Fetches the author's birthdate by scraping the biography page.

**play_game_with_four_chances(quotes_with_info):**
 The user gets four chances to guess the author with hints provided after each incorrect attempt.

**author_name_hint(auth):**
Provides hints about the author's name.

**hints_display(quote):**
Displays hints based on the quote and author details , providing one hint per incorrect attempt.



