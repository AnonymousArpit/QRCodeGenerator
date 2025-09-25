# QR Code Generator

A modern, feature-rich QR code generator built with React, TypeScript, and Tailwind CSS. Create customizable QR codes instantly with real-time preview and high-quality downloads.

![QR Code Generator](https://img.shields.io/badge/React-18+-blue.svg)
![TypeScript](https://img.shields.io/badge/TypeScript-5+-blue.svg)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## ✨ Features

- **🚀 Instant Generation**: Real-time QR code generation as you type
- **🎨 Full Customization**: Customize colors, size, and error correction levels
- **📱 Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **💾 High-Quality Downloads**: Download QR codes as PNG images in various sizes
- **🔧 Error Correction**: Multiple error correction levels (Low, Medium, Quartile, High)
- **🎯 Multiple Data Types**: Support for URLs, text, contact info, and more
- **⚡ Fast & Lightweight**: Built with modern web technologies for optimal performance

## 🛠️ Technology Stack

- **Frontend Framework**: React 18+ with TypeScript
- **Styling**: Tailwind CSS + Shadcn/ui components
- **QR Generation**: qrcode library
- **Build Tool**: Vite
- **Package Manager**: pnpm

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ 
- pnpm (recommended) or npm

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/anonymousarpit/qr-code-generator.git
   cd qr-code-generator
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   ```

3. **Start development server**
   ```bash
   pnpm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

### Build for Production

```bash
# Build the project
pnpm run build

# Preview the production build
pnpm run preview
```

## 📖 Usage

1. **Enter Text**: Type or paste any text, URL, or data into the text area
2. **Customize**: Adjust size, colors, and error correction level using the controls
3. **Preview**: See your QR code update in real-time
4. **Download**: Click the download button to save your QR code as a PNG image

### Supported Data Types

- **URLs**: `https://example.com`
- **Plain Text**: Any text content
- **Email**: `mailto:user@example.com`
- **Phone**: `tel:+1234567890`
- **SMS**: `sms:+1234567890`
- **WiFi**: `WIFI:T:WPA;S:NetworkName;P:Password;;`
- **Contact Info**: vCard format

## ⚙️ Customization Options

### Size Options
- Range: 128px - 512px
- Step: 32px increments
- Default: 256px

### Error Correction Levels
- **Low (L)**: ~7% error correction
- **Medium (M)**: ~15% error correction (default)
- **Quartile (Q)**: ~25% error correction
- **High (H)**: ~30% error correction

### Color Customization
- **Foreground Color**: QR code pattern color
- **Background Color**: QR code background color
- Full color picker support

## 📁 Project Structure

```
qr-code-generator/
├── public/
│   ├── favicon.svg
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── ui/              # Shadcn/ui components
│   │   ├── QRGenerator.tsx  # Main generator component
│   │   ├── QRDisplay.tsx    # QR code display and download
│   │   └── QRCustomizer.tsx # Customization controls
│   ├── pages/
│   │   ├── Index.tsx        # Home page
│   │   └── NotFound.tsx     # 404 page
│   ├── lib/
│   │   └── utils.ts         # Utility functions
│   ├── App.tsx              # Root component
│   ├── main.tsx             # Entry point
│   └── index.css            # Global styles
├── package.json
├── tailwind.config.ts
├── vite.config.ts
└── README.md
```

## 🔧 Configuration

### Vite Configuration
The project uses Vite for fast development and building. Configuration can be found in `vite.config.ts`.

### Tailwind CSS
Tailwind configuration is in `tailwind.config.ts`. The project uses a custom design system with Shadcn/ui components.

### TypeScript
TypeScript configuration is split into:
- `tsconfig.json` - Base configuration
- `tsconfig.app.json` - App-specific settings
- `tsconfig.node.json` - Node.js specific settings

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Guidelines

1. **Code Style**: Follow the existing code style and use TypeScript
2. **Components**: Use functional components with React hooks
3. **Styling**: Use Tailwind CSS classes and Shadcn/ui components
4. **Testing**: Ensure your changes work across different browsers and devices

### Pull Request Process

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 Scripts

- `pnpm run dev` - Start development server
- `pnpm run build` - Build for production
- `pnpm run preview` - Preview production build
- `pnpm run lint` - Run ESLint
- `pnpm run type-check` - Run TypeScript type checking

## 🐛 Troubleshooting

### Common Issues

1. **QR Code not generating**: Ensure text input is not empty
2. **Download not working**: Check if your browser blocks automatic downloads
3. **Styling issues**: Clear browser cache and reload
4. **Build errors**: Delete `node_modules` and `pnpm-lock.yaml`, then reinstall

### Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+


## 🙏 Acknowledgments

- [qrcode](https://github.com/soldair/node-qrcode) - QR code generation library
- [Shadcn/ui](https://ui.shadcn.com/) - UI component library
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework
- [Lucide React](https://lucide.dev/) - Icon library
- [Vite](https://vitejs.dev/) - Build tool


---

**Made with ❤️ by Arpit Raizada (https://github.com/anonymousarpit)**

*If you found this project helpful, please consider giving it a ⭐ on GitHub!*
