# VizMarkdown MVP

A client-side tool that allows users to create embeddable charts using simple, Markdown-like syntax. Built as a single HTML file for maximum simplicity and ease of deployment.

## 🎯 Vision

To provide the fastest way for anyone to create and share embeddable charts using simple text.

## ✨ Features

### Core Features (MVP)

1. **Text-Based Chart Definition**
   - Simple textarea for defining chart properties using Markdown-like syntax
   - Supports chart type, title, labels, and dataset configuration
   - Real-time syntax validation

2. **Live Chart Preview**
   - Instant visual preview using Chart.js
   - Responsive chart rendering
   - Multiple chart types supported (bar, line, pie, etc.)

3. **Embed Code Generation**
   - iFrame embed code for websites
   - Static image embed code for emails
   - One-click copy functionality

4. **Dashboard & Persistence**
   - Save charts to browser localStorage
   - Dashboard view to manage saved charts
   - Load and edit previous charts
   - Delete unwanted charts

## 🚀 Quick Start

1. **Open the application**: Simply open `index.html` in any modern web browser
2. **Create your first chart**: Use the sample data provided or enter your own
3. **Generate the chart**: Click "Generate Chart" to see the live preview
4. **Save your work**: Click "Save Chart" to store it in your dashboard
5. **Get embed codes**: Copy the generated embed codes for your website or email

## 📝 Chart Syntax

The application uses a simple, Markdown-like syntax for defining charts:

```
chart type: bar
title: Sales Performance
labels: Q1, Q2, Q3, Q4
dataset: 120, 190, 300, 500
```

### Supported Properties

- **chart type**: The type of chart (bar, line, pie, doughnut, etc.)
- **title**: The chart title
- **labels**: Comma-separated labels for the x-axis
- **dataset**: Comma-separated numerical values for the y-axis

### Example Charts

**Bar Chart:**
```
chart type: bar
title: Monthly Revenue
labels: Jan, Feb, Mar, Apr, May, Jun
dataset: 12000, 19000, 30000, 50000, 20000, 30000
```

**Line Chart:**
```
chart type: line
title: Website Traffic
labels: Mon, Tue, Wed, Thu, Fri, Sat, Sun
dataset: 1000, 1200, 800, 1500, 2000, 1800, 1600
```

**Pie Chart:**
```
chart type: pie
title: Market Share
labels: Product A, Product B, Product C, Product D
dataset: 30, 25, 20, 25
```

## 🎨 User Interface

The application features a clean, modern interface with:

- **Two-panel layout**: Input panel on the left, preview panel on the right
- **Responsive design**: Works on desktop and mobile devices
- **Navigation**: Easy switching between editor and dashboard views
- **Toast notifications**: User feedback for all actions
- **Modern styling**: Built with Tailwind CSS

## 🔧 Technical Details

### Tech Stack

- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Styling**: Tailwind CSS (via CDN)
- **Charts**: Chart.js (via CDN)
- **Storage**: Browser localStorage
- **Deployment**: Static hosting (Netlify, Vercel, GitHub Pages, etc.)

### File Structure

```
VizMarkdown MVP/
├── index.html          # Main application file
├── README.md           # This documentation
└── PRD MVP            # Product Requirements Document
```

### Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 📊 Embedding Charts

### Website Embed (iFrame)

The application generates iFrame embed codes that can be used on any website:

```html
<iframe src="https://your-domain.com/index.html?embed=true&name=Chart%20Name&config=chart%20type%3A%20bar..." width="100%" height="400" frameborder="0"></iframe>
```

### Email Embed (Static Image)

For email compatibility, static image embed codes are provided (placeholder implementation in MVP).

## 🎯 Target Users

- **Content Creators**: Bloggers who need quick charts for articles
- **Students**: Creating visualizations for reports and presentations
- **Developers**: Quick prototyping and documentation
- **Business Users**: Simple data visualization without complex tools

## 🚀 Deployment

### Local Development

1. Clone or download the project
2. Open `index.html` in your browser
3. Start creating charts!

### Production Deployment

The application is designed to be deployed as a static site:

1. **Netlify**: Drag and drop the `index.html` file
2. **Vercel**: Connect your repository and deploy
3. **GitHub Pages**: Push to a repository and enable Pages
4. **Any static hosting**: Upload the single HTML file

## 📈 Success Metrics

The MVP aims to validate:

- **Usage Rate**: 50% of unique visitors successfully generate at least one chart
- **User Satisfaction**: Direct feedback collection from testers
- **Feature Discovery**: Tracking most-requested chart types and features

## 🔮 Future Enhancements

Based on user feedback, potential future features include:

- More chart types (scatter, radar, etc.)
- Custom colors and styling
- Multiple datasets support
- Real-time data integration
- Cloud-based saving and sharing
- User accounts and collaboration
- Export to various formats (PNG, SVG, PDF)

## 🤝 Contributing

This is an MVP for idea validation. Feedback and suggestions are welcome!

## 📄 License

This project is open source and available under the MIT License.

---

**Built with ❤️ for content creators who need fast, simple chart creation.**