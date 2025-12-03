# DeepLinkRedirect

A universal deep link redirector for the SpeedTest app, hosted on GitHub Pages.

## 🔗 Live Demo

Visit the live site at: [https://armandfardeau.github.io/DeepLinkRedirect/](https://armandfardeau.github.io/DeepLinkRedirect/)

## 📖 What is This?

This project provides a simple web-based redirector that allows you to create shareable links that open specific locations within the SpeedTest mobile application using deep links.

## 🚀 Usage

To create a deep link that opens the SpeedTest app, use the following URL format:

```
https://armandfardeau.github.io/DeepLinkRedirect/deeplink.html?to=speedtest://[path]
```

### Examples

Open a specific server:
```
https://armandfardeau.github.io/DeepLinkRedirect/deeplink.html?to=speedtest://server/12345
```

Start a speed test immediately:
```
https://armandfardeau.github.io/DeepLinkRedirect/deeplink.html?to=speedtest://start
```

## 🛠️ How It Works

1. User clicks on a redirector link with a `to` query parameter
2. The `deeplink.html` page extracts the deep link from the URL
3. JavaScript attempts to open the deep link in the SpeedTest app
4. If successful, the app opens to the specified location
5. If the app is not installed, the user is notified with troubleshooting steps

## 📋 Requirements

- The SpeedTest app must be installed on the user's device
- The browser must allow opening external applications
- The deep link must use the `speedtest://` URL scheme

## 🏗️ Development

This is a static site with no build process required. The project consists of:

- `index.html` - Landing page with documentation
- `deeplink.html` - Redirect handler page

To test locally, simply open the HTML files in a web browser or use a local web server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 👤 Author

**Armand Fardeau**

- GitHub: [@armandfardeau](https://github.com/armandfardeau)