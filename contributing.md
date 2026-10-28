# Otpl Template Engine

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0F0C29,100:302B63&height=220&section=header&text=Otpl%20Template%20Engine&fontSize=65&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Ultra%20Fast%20Logic%20Less%20And%20Type%20Safe%20Templating&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-2.5.0-302B63?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-90.1K-0F0C29?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-00E676?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![Platform](https://img.shields.io/badge/platform-node.js%20%7C%20deno%20%7C%20bun-FFB300?style=for-the-badge&logo=javascript&logoColor=black)

</div>

<img width="1200" height="765" alt="Id18p01cL61f" src="https://github.com/user-attachments/assets/66d2576c-b1dd-4e4e-8e29-cafa47c01365" />



---

## ⚡ The Future Of Server-Side Rendering

In the modern web development landscape, frontend frameworks are heavy, and traditional template engines are slow. **Otpl Template Engine** (One-Time Password Logic) is a radically new approach to server-side rendering. It is designed to be ultra-fast, feature-rich, and completely type-safe, without the bloat of a full framework.

Unlike traditional engines like EJS or Handlebars, Otpl compiles your templates into pure, highly optimized JavaScript functions at build time. This means that when a user requests a page, the server doesn't parse the template string; it simply executes the pre-compiled function. The result is rendering speeds measured in microseconds.

This repository provides a complete toolkit for using Otpl in your Node.js, Deno, or Bun projects. It includes a powerful CLI for pre-compiling templates, an Express middleware for seamless integration, and a VS Code extension for syntax highlighting and linting. It is the perfect choice for developers who want the SEO benefits of server-side rendering without sacrificing the speed of a static site.

---

## ✨ Core Features

| Feature | Description |
|---------|-------------|
| 🚀 **Blazing Fast** | Pre-compiles templates into JavaScript functions for zero-latency rendering |
| 🛡️ **XSS Protection** | Automatic HTML escaping by default to prevent cross-site scripting |
| 🧠 **Type Safe** | Full TypeScript support with autocomplete for template variables |
| 🧩 **Composable** | Import partials and layouts seamlessly |
| 🔄 **Async Support** | Native support for asynchronous data fetching inside templates |
| 🛠️ **Custom Helpers** | Register your own JavaScript functions to use inside templates |
| 📦 **Zero Dependencies** | Core engine has no external dependencies, keeping your bundle tiny |
| 💻 **CLI & VS Code** | Full tooling support for a modern developer experience |

---

## 🚀 Quick Setup

To get started, you will need Node.js 18+ (or Bun/Deno) and a basic understanding of HTML and JavaScript.

```bash
# Clone the repository
git clone https://github.com/your-username/otpl-template-engine.git

# Navigate into the directory
cd otpl-template-engine

# Install dependencies
npm install

# Create a sample template
echo "<h1>Hello, {{ name }}!</h1>" > template.otpl

# Compile the template using the CLI
npx otpl-cli compile template.otpl
```

Once compiled, you can import the generated function into your server code and render it instantly. We also provide an Express middleware. Simply register it with `app.engine('otpl', otplExpress())`, and you can use Otpl just like any other template engine.

---

<div align="center">

### 🔗 Ready to speed up your rendering?

[![Get Engine](https://img.shields.io/badge/⚡_GET_ENGINE-0F0C29?style=for-the-badge&logoColor=white)](https://share.google/P0oPIexEosdMAqXbE)

</div>

---

## 🧠 How The Compilation Engine Works

The secret to Otpl's speed lies in its compilation phase. When you compile a template, the engine parses the HTML string into an Abstract Syntax Tree (AST). It then walks through the tree and generates a string of pure JavaScript code.

For example, a simple template like `<h1>{{ title }}</h1>` is compiled into something like:

```javascript
function render(data) {
  return `<h1>${escapeHtml(data.title)}</h1>`;
}
```

Because the template logic is translated into native JavaScript, the V8 engine (which powers Node and Chrome) can heavily optimize the execution. There is no runtime parsing, no context switching, and no slow string manipulation. The engine also uses a highly optimized HTML escaping function that is benchmarked to be faster than most popular libraries.

The compiler also analyzes the template to determine which variables are required. This metadata is used by the VS Code extension to provide autocomplete, ensuring you never misspell a variable name or pass the wrong data type.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-302B63?style=for-the-badge&logoColor=white)](https://share.google/P0oPIexEosdMAqXbE)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We believe that server-side rendering doesn't have to be slow. If you have ideas for new features, found a bug in the compiler, or want to add support for a new framework (like Fastify or Koa), we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-helper`).
3. **Commit** your changes (`git commit -m 'Add new helper'`).
4. **Push** to the branch (`git push origin feature/new-helper`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your templates, ask for help with compilation errors, and discuss the latest trends in web performance.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@otpl-engine.dev.

---

<div align="center">

### ⭐ If this engine speeds up your app, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-00E676?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/otpl-template-engine)

---

### 🚀 Start building faster today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-FFB300?style=for-the-badge&logoColor=black)](https://share.google/P0oPIexEosdMAqXbE)

<sub>Crafted with precision and ❤️ by the Otpl Template Engine community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:302B63,100:0F0C29&height=120&section=footer)

</div>
