# Vimm's Lair Scraper

This script scrapes game links from Vimm’s Lair for personal or educational use, focusing on Xbox game categories and individual game pages. It dynamically builds URLs based on the site structure to avoid errors, making it easy to adapt for other game directories.

## How It Works

- **Category & Game Link Handling**: Differentiates between category pages (`/vault/Xbox`) and game pages (`/vault/[game_number]`) to build correct URLs.
- **Adaptable for Other Games**: To scrape other game directories, simply change `xbox_category_url` in the script to a different system, e.g., `/vault/PS2` for PlayStation 2 games.

<details>
  <summary>Usage Instructions</summary>

  1. **Install dependencies**:
      ```bash
      pip install requests beautifulsoup4
      ```

  2. **Run the script**:
      ```bash
      python script.py
      ```

</details>

<details>
  <summary>Important Notes</summary>

  - **Respects Site Limits**: This script does not bypass the download-per-client limit, and bypassing it may not be feasible. However, the script does bypass some bot protections by mimicking regular browser behavior through the use of a `User-Agent` header. Without this header, direct access may result in a block.

  - **Disclaimer**: Use responsibly and in accordance with Vimm’s Lair’s terms of service. While the script is designed with ethical scraping practices in mind, you're responsible for its use.

  - **Proxy Consideration**: It did occur to me to use proxies, but the overhead is annoying to me. Proxies add more variables, such as the need to manage multiple IP addresses and handle potential connection issues or delays. Using proxies can also introduce added complexity with rate limiting, as some IPs might be blocked or flagged more quickly, requiring constant monitoring and adjustments. Additionally, proxies can slow down the scraping process due to network latency, especially if rotating between multiple servers. Overall, while proxies could bypass certain limitations, the added overhead and maintenance make it less practical for my use case.

</details>
