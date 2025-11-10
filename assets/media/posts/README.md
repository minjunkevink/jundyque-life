# Post Media Organization

This directory contains media files (images, videos, memes, etc.) organized by blog post.

## Structure

Each post has its own folder named after the post filename (without the `.md` extension):

```
assets/media/posts/
├── 2025-11-03-is-living-in-a-car-cheaper/
│   ├── image1.jpg
│   ├── meme.png
│   └── video.mp4
├── 2025-11-03-stolen-focus-review/
│   └── book-cover.jpg
└── 2025-01-15-welcome-to-my-blog/
    └── screenshot.png
```

## Usage in Posts

Reference media files in your markdown posts using Jekyll's `relative_url` filter:

```markdown
![Alt text]({{ '/assets/media/posts/2025-11-03-is-living-in-a-car-cheaper/image.jpg' | relative_url }})
```

Or for videos:

```html
<video controls>
  <source src="{{ '/assets/media/posts/2025-11-03-is-living-in-a-car-cheaper/video.mp4' | relative_url }}" type="video/mp4">
</video>
```

## Naming Convention

- Folder names must match the post filename exactly (without `.md` extension)
- Media files can have any descriptive name
- Use lowercase with hyphens for consistency

## Adding Media to a New Post

1. Create a new folder: `assets/media/posts/YYYY-MM-DD-post-title/`
2. Add your media files to that folder
3. Reference them in your post using the path shown above

