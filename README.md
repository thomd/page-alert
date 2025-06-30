# Page Alert

A GitHub Actions-powered web page monitoring tool that tracks changes to multiple HTML pages and generates RSS feeds for updates.

## Configuration

Create a `config.yml` file in the root directory with the following structure:

```yaml
urls:
  - name: "Example Page 1"
    url: "https://example-1.com"
  - name: "Example Page 2"
    url: "https://example-2.com"
```

## Usage

1. Fork this repository
2. Edit `config.yml` to add your desired URLs
3. Enable GitHub Actions in your repository
4. The workflow will run automatically at 8:30 AM UTC daily
5. Manual runs can be triggered using the "Run workflow" button in GitHub Actions

## Files Generated

- `fetched-pages/`: Directory containing downloaded HTML files
- `rss.xml`: RSS feed with update notifications

