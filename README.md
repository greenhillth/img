# img

A simple GitHub Pages site for displaying images via URL endpoints.

## Usage

Access the site and specify an image using the `img` URL parameter:

### Local Images

Display images from the `images/` directory:
```
https://greenhillth.github.io/img/?img=images/sample.svg
https://greenhillth.github.io/img/?img=images/example.svg
```

### External Images

Display images from external URLs:
```
https://greenhillth.github.io/img/?img=https://example.com/image.jpg
```

## Features

- 📷 Display images from local paths or external URLs
- 🎨 Clean, responsive design
- ⚡ Fast loading with error handling
- 📱 Mobile-friendly interface

## Examples

The repository includes sample images in the `images/` directory:
- `images/sample.svg` - Green sample image
- `images/example.svg` - Blue example image

## Local Development

To test locally:

1. Clone the repository
2. Open `index.html` in a web browser
3. Add query parameter: `?img=images/sample.svg`

Or use a local server:
```bash
python -m http.server 8000
# Then visit: http://localhost:8000/?img=images/sample.svg
```

## How It Works

The site uses JavaScript to:
1. Parse the `img` parameter from the URL
2. Load and display the specified image
3. Show error messages if the image fails to load
4. Provide usage instructions when no image is specified