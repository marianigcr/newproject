# Hugging Face Open Data Dashboard

A modern, interactive dashboard for exploring and visualizing open datasets from Hugging Face. Discover, analyze, and interact with thousands of publicly available datasets in an intuitive web interface.

## Features

- **Interactive Data Visualization**: Explore datasets with charts, graphs, and interactive plots
- **Advanced Search & Filtering**: Find datasets by category, size, language, and more
- **Dataset Analytics**: View statistics, sample data, and metadata insights
- **Modern UI/UX**: Clean, responsive design built with modern web technologies
- **Mobile Responsive**: Works seamlessly across all devices
- **Real-time Updates**: Live data fetching from Hugging Face APIs
- **Local Caching**: Fast performance with intelligent data caching

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn package manager
- Modern web browser

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/huggingface-dashboard.git
   cd huggingface-dashboard
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your Hugging Face API token (optional)
   ```

4. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:3000` to view the dashboard

## Tech Stack

- **Frontend**: React.js with TypeScript
- **Styling**: Tailwind CSS + CSS Modules
- **Charts**: Chart.js or D3.js for data visualization
- **State Management**: React Context or Redux
- **API Integration**: Hugging Face Datasets API
- **Build Tool**: Vite or Next.js
- **Deployment**: Vercel, Netlify, or Docker

## Project Structure

```
huggingface-dashboard/
├── src/
│   ├── components/          # Reusable UI components
│   ├── pages/              # Page components and routing
│   ├── hooks/              # Custom React hooks
│   ├── services/           # API services and data fetching
│   ├── utils/              # Helper functions and utilities
│   ├── types/              # TypeScript type definitions
│   └── styles/             # Global styles and CSS modules
├── public/                 # Static assets
├── docs/                   # Documentation
└── tests/                  # Test files
```

## Configuration

### Environment Variables

Create a `.env` file in the root directory:

```env
# Hugging Face API Configuration (optional)
HUGGINGFACE_API_TOKEN=your_token_here

# App Configuration
NEXT_PUBLIC_APP_NAME=Hugging Face Dashboard
NEXT_PUBLIC_API_BASE_URL=https://huggingface.co/api
```

### API Rate Limits

The dashboard respects Hugging Face's API rate limits:
- **Anonymous users**: 100 requests/hour
- **Authenticated users**: 1000 requests/hour

## Usage

1. **Browse Datasets**: Use the main dashboard to explore available datasets
2. **Search & Filter**: Use the search bar and filters to find specific datasets
3. **View Details**: Click on any dataset to see detailed information
4. **Visualize Data**: Use the built-in visualization tools to explore dataset contents
5. **Export Data**: Download dataset samples or metadata for further analysis

## Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

### Development Setup

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

### Code Style

- Follow the existing code style and conventions
- Use TypeScript for all new code
- Write meaningful commit messages
- Include tests for new features

## Testing

```bash
# Run unit tests
npm run test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage

# Run end-to-end tests
npm run test:e2e
```

## Building for Production

```bash
# Build the application
npm run build

# Start production server
npm start

# Export as static site (if using Next.js)
npm run export
```

## Deployment

### Vercel (Recommended)

1. Connect your GitHub repository to Vercel
2. Configure environment variables
3. Deploy automatically on every push

### Docker

```bash
# Build Docker image
docker build -t huggingface-dashboard .

# Run container
docker run -p 3000:3000 huggingface-dashboard
```

### Manual Deployment

1. Build the project: `npm run build`
2. Upload the `dist/` or `out/` folder to your hosting provider
3. Configure your web server to serve the static files

## API Reference

The dashboard integrates with several Hugging Face APIs:

- **Datasets API**: Fetch dataset metadata and information
- **Models API**: Access model information and metadata
- **Spaces API**: Explore Hugging Face Spaces

For detailed API documentation, visit [Hugging Face API Docs](https://huggingface.co/docs/api-inference).

## Troubleshooting

### Common Issues

1. **API Rate Limiting**: If you hit rate limits, consider authenticating with an API token
2. **CORS Issues**: Ensure your hosting provider allows CORS requests
3. **Build Errors**: Check Node.js version compatibility and dependency versions

### Getting Help

- [Documentation](docs/)
- [Issue Tracker](https://github.com/yourusername/huggingface-dashboard/issues)
- [Discussions](https://github.com/yourusername/huggingface-dashboard/discussions)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Hugging Face](https://huggingface.co/) for providing the datasets and APIs
- [React](https://reactjs.org/) team for the framework
- All contributors and users of this project

## Roadmap

- [ ] Advanced data visualization options
- [ ] Dataset comparison tools
- [ ] User authentication and favorites
- [ ] Offline mode support
- [ ] Mobile app version
- [ ] Integration with other data platforms

---

**Made with ❤️ by the Open Source Community**

If you find this project helpful, please consider giving it a star on GitHub!
