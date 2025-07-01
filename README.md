# Page Alert

A GitHub Actions-powered **web page monitoring** tool that tracks changes to multiple HTML pages and generates a **RSS feed** for **alerting** updates.

## Usage

1. Edit `config.yml` to add URLs to be watched for changes
1. Enable GitHub Actions in your repository
1. The workflow will run automatically at 6:35am UTC daily (update in `alert.yml` )
1. Manual runs can be triggered using the "Run workflow" button in GitHub Actions

## Configuration

Create a `config.yml` file in the root directory with the following structure:

```yaml
urls:
  - name: "Example Page 1"
    url: "https://example-1.com"
  - name: "Example Page 2"
    url: "https://example-2.com"
```

## Files Generated

- `fetched-pages/`: Directory containing downloaded HTML files
- `rss.xml`: RSS feed with update notifications

