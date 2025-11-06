# jundyque.life Blog

A minimalistic Jekyll blog website for jundyque.life.

## Setup

1. Install Ruby and Bundler if you haven't already:
   ```bash
   gem install bundler
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Serve the site locally:
   ```bash
   bundle exec jekyll serve
   ```

4. Visit `http://localhost:4000` in your browser

## Customization

### Site Configuration
Edit `_config.yml` to update:
- Site title and description
- Email and social media links
- URL settings

### Home Page
Edit `_markdown/index.md` to customize your home page content.

### Profile Image
Add your profile image at `assets/images/profile.jpg` (200x200px recommended).

### Social Links
Update the social links in `_layouts/home.html`:
- LinkedIn URL
- GitHub URL
- CV/Resume link

### Blog Posts
Create new posts in the `_posts/` directory with the naming format:
```
YYYY-MM-DD-post-title.md
```

Each post should include front matter:
```yaml
---
layout: post
title: "Your Post Title"
date: 2025-01-15
tags: [tag1, tag2]
featured_image: /assets/images/your-image.jpg  # optional
---
```

### Blog Tags
Edit the `custom_tags` array in `_layouts/blog.html` to customize available tags.

### Styling
Modify `assets/css/style.css` to customize the design.

## Deployment

### GitHub Pages
1. Push this repository to GitHub
2. Go to Settings > Pages
3. Select your branch and source
4. Add a `CNAME` file with your domain (already included)

### Custom Domain (GoDaddy)
1. In your GoDaddy DNS settings, add:
   - Type: CNAME
   - Name: @
   - Value: your-username.github.io
2. Wait for DNS propagation (can take up to 48 hours)

## License

Feel free to use this template for your own blog!

