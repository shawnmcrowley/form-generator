<div align="center">

# Form Generator

**Modern dynamic form generation with Next.js and advanced configuration**

[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-blue)](https://reactjs.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E)](https://www.ecmascript.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

<a name="toc"></a>

[Features](#features) •
[Getting Started](#getting-started) •
[Configuration](#configuration) •
[Project Structure](#project-structure) •
[Contributing](#contributing)

</div>

---

<a name="overview"></a>

## 📋 Overview

A production-ready form generation system built with Next.js 16 that enables rapid creation and deployment of dynamic, responsive forms through configuration-driven development. Perfect for building flexible form solutions with minimal code.

<a name="features"></a>

## ✨ Features

- 🎯 **Dynamic Form Generation** - Create forms from JSON/configuration files
- 📱 **Responsive Design** - Mobile-first approach with Tailwind CSS
- ⚡ **Next.js 16** - Latest Next.js features with Turbopack
- 🎨 **Tailwind CSS** - Utility-first CSS framework for rapid styling
- 🔧 **Configuration-Driven** - No code required for form creation
- 📝 **Flexible Validation** - Built-in and custom validation rules
- 🚀 **Production Ready** - Optimized for performance and scalability
- 💾 **State Management** - Efficient form state handling

[Back to Top](#toc)

<a name="getting-started"></a>

## 🚀 Getting Started

### Prerequisites

- Node.js 18.17 or later
- npm or yarn
- Basic knowledge of React and Next.js

### Installation

```bash
# Clone the repository
git clone <repository-url>

# Navigate to form-generator directory
cd form-generator

# Install dependencies
npm install

# Run development server with Turbopack
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the application.

### Building for Production

```bash
npm run build
npm start
```

[Back to Top](#toc)

<a name="configuration"></a>

## ⚙️ Configuration

### Form Configuration

Forms are defined through configuration objects that specify:

```javascript
{
  name: "User Registration",
  fields: [
    {
      name: "email",
      type: "email",
      label: "Email Address",
      required: true,
      validation: {
        pattern: /^[^\s@]+@[^\s@]+\.[^\s@]+$/
      }
    },
    {
      name: "password",
      type: "password",
      label: "Password",
      required: true,
      minLength: 8
    }
  ],
  submitLabel: "Register"
}
```

### Tailwind Configuration

Edit `tailwind.config.js` to customize your design system:

```javascript
module.exports = {
  theme: {
    extend: {
      colors: {},
      spacing: {}
    }
  }
}
```

[Back to Top](#toc)

<a name="project-structure"></a>

## 📁 Project Structure

```
form-generator/
├── jsconfig.json           # JavaScript configuration
├── next.config.mjs         # Next.js configuration
├── package.json            # Project dependencies
├── postcss.config.mjs      # PostCSS configuration
├── tailwind.config.js      # Tailwind CSS configuration
├── public/                 # Static assets
│   └── favicon.ico
└── src/
    ├── app/               # Next.js app directory
    ├── components/        # Reusable React components
    │   ├── FormGenerator.jsx
    │   └── FormField.jsx
    └── styles/            # Global styles
```

### Key Directories

- **`src/app/`** - Next.js pages and layouts
- **`src/components/`** - Reusable form and UI components
- **`public/`** - Static assets served publicly

[Back to Top](#toc)

<a name="contributing"></a>

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

[Back to Top](#toc)

---

<div align="center">

**[Back to Top](#toc)**

</div>
