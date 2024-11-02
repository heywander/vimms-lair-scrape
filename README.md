Vimm's Lair Scraper
This script scrapes game links from Vimm’s Lair for personal or educational use, focusing on Xbox game categories and individual game pages. It dynamically builds URLs based on the site structure to avoid errors, making it easy to adapt for other game directories.

How It Works
Category & Game Link Handling:

Differentiates between category pages (/vault/Xbox) and game pages (/vault/[game_number]).
Avoids incorrect URL paths by adjusting for each type.
Adjustable for Other Games:

To scrape other game directories, simply change xbox_category_url in the script to a different system, e.g., /vault/PS2 for PlayStation 2 games.
Ensure that the script filters links correctly if the structure varies by system.
Usage
Install dependencies:
bash
Copy code
pip install requests beautifulsoup4
Run the script:
bash
Copy code
python script.py
Important Notes
Respect Site Limits: The script includes basic safeguards. Add rate limiting if you make frequent requests.
Disclaimer: Use responsibly and in accordance with Vimm’s Lair’s terms of service.
