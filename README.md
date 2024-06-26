# 🚀 Perplexica - An AI-powered search engine 🔎

![preview](.assets/perplexica-screenshot.png)

## Overview

Perplexica is an open-source AI-powered searching tool or an AI-powered search engine that goes deep into the internet to find answers. Inspired by Perplexity AI, it's an open-source option that not just searches the web but understands your questions. It uses advanced machine learning algorithms like similarity searching and embeddings to refine results and provides clear answers with sources cited.

## Preview

![video-preview](.assets/perplexica-preview.gif)

## Features

- **Two Main Modes:**
  - **Copilot Mode:** (In development) Boosts search by generating different queries to find more relevant internet sources. Like normal search instead of just using the context by SearxNG, it visits the top matches and tries to find relevant sources to the user's query directly from the page.
  - **Normal Mode:** Processes your query and performs a web search.
- **Focus Modes:** (In development) special modes to better answer specific types of questions.
- **Current Information:** Some search tools might give you outdated info because they use data from crawling bots and convert them into embeddings and store them in a index (its like converting the web into embeddings which is quite expensive.). Unlike them, Perplexica uses SearxNG, a metasearch engine to get the results and rerank and get the most relevent source out of it, ensuring you always get the latest information without the overhead of daily data updates.

It has many more features like image and video search. Some of the planned features are mentioned in [upcoming features](#upcoming-features).

## Installation

There are mainly 2 ways of installing Perplexica - With Docker, Without Docker. Using Docker is highly recommended.

### Getting Started with Docker (Recommended)

1. Ensure Docker is installed and running on your system.
2. Clone the Perplexica repository:

   ```bash
   git clone https://github.com/ItzCrazyKns/Perplexica.git
   ```

3. After cloning, navigate to the directory containing the project files.

4. Rename the `.env.example` file to `.env`. For Docker setups, you need only fill in the following fields:
   - `OPENAI_API_KEY`
   - `SIMILARITY_MEASURE` (This is filled by default; you can leave it as is if you are unsure about it.)

5. Ensure you are in the directory containing the `docker-compose.yaml` file and execute:

   ```bash
   docker compose up
   ```

6. Wait a few minutes for the setup to complete. You can access Perplexica at `http://localhost:3001` in your web browser.

**Note**: Once the terminal is stopped, Perplexica will also stop. To restart it, you will need to open Docker Desktop and run Perplexica again.

### Non-Docker Installation

For setups without Docker:

1. Follow the initial steps to clone the repository and rename the `.env.example` file to `.env` in the root directory. You will need to fill in all the fields in this file.
2. Additionally, rename the `.env.example` file to `.env` in the `ui` folder and complete all fields.
3. The non-Docker setup requires manual configuration of both the backend and frontend.

**Note**: Using Docker is recommended as it simplifies the setup process, especially for managing environment variables and dependencies.

## Upcoming Features

- Finalizing Copilot Mode
- Adding support for multiple local LLMs and LLM providers such as Anthropic, Google, etc.
- Adding Discover and History Saving features
- Introducing various Focus Modes
- Continuous bug fixing

## Contribution

Perplexica is built on the idea that AI and large language models should be easy for everyone to use. If you find bugs or have ideas, please share them in via GitHub Issues. Details on how to contribute will be shared soon.

## Acknowledgements

Inspired by Perplexity AI, Perplexica aims to provide a similar service but always up-to-date and fully open source, thanks to SearxNG.

If you have any queries you can reach me via my Discord - `itzcrazykns`. Thanks for checking out Perplexica.
