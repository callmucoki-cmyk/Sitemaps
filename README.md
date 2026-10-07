# Sitemaps Repository

This repository contains XML sitemaps for luxorita.store to help Google robots index all product URLs instantly.

## Files

- **sitemap.xml** - Main XML sitemap with all product URLs in proper format
- **robots.txt** - Instructions for search engine crawlers
- **Sitenaps** - Original plain-text URL list (deprecated)

## How to Use

### 1. Deploy Sitemap to Your Website
Copy `sitemap.xml` to your website's root directory:
```
https://luxorita.store/sitemap.xml
```

### 2. Submit to Google Search Console
- Go to [Google Search Console](https://search.google.com/search-console)
- Add your sitemap URL: `https://luxorita.store/sitemap.xml`
- Google will automatically crawl and index all URLs

### 3. Add to robots.txt
Place this in your website's `robots.txt`:
```
Sitemap: https://luxorita.store/sitemap.xml
```

## When Adding New URLs

1. Update `sitemap.xml` with new URLs following this format:
```xml
<url>
  <loc>https://luxorita.store/your-new-product-url</loc>
  <lastmod>2026-10-07</lastmod>
  <changefreq>weekly</changefreq>
  <priority>0.8</priority>
</url>
```

2. Commit changes to this repository
3. Resubmit updated sitemap to Google Search Console
4. Google will re-crawl within 24-48 hours

## Sitemap Best Practices

- ✅ Each URL in valid XML format
- ✅ `lastmod` tag shows when content was updated
- ✅ `changefreq` helps Google prioritize crawling
- ✅ `priority` indicates URL importance (0.0-1.0)
- ✅ Maximum 50,000 URLs per sitemap
- ✅ Maximum 50MB file size

## Current Stats

- Total URLs: unlimited 
- Last Updated: 2026-10-07
- Format: XML 1.0 UTF-8
