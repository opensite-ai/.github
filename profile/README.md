<img width="100%" height="auto" alt="OpenSite AI Page Spped Open Source Code Libraries" src="https://github.com/user-attachments/assets/79129f99-bbee-4ea0-8dc7-467255a4f9ea" />

# OpenSite AI

**High-Performance Open Source Libraries for Modern Web Development**

[![NPM](https://img.shields.io/badge/NPM-Packages-CB3837?style=flat&logo=npm)](https://www.npmjs.com/org/page-speed)
[![RubyGems](https://img.shields.io/badge/RubyGems-Gems-E9573F?style=flat&logo=ruby)](https://rubygems.org/profiles/jordanhudgens)
[![Crates.io](https://img.shields.io/badge/Crates.io-Rust-000000?style=flat&logo=rust)](https://crates.io/users/jordanhudgens)
[![Website](https://img.shields.io/badge/Website-OpenSite.ai-4285F4?style=flat&logo=google-chrome)](https://opensite.ai/developers)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/company/opensite-ai)

---

## About OpenSite AI

OpenSite AI is dedicated to engineering **practical, high-performance tools and libraries** for the global developer community. Every open source project we release is built to solve real-world problems with measurable performance gains.

Our mission is simple: **give back to the developer community** with production-tested tools that we know the value of—because we spent years fine-tuning them for our own high-performance website and AI platform.

### Why We Open Source

Each library in our ecosystem was **hand-picked from 50+ internal platform applications and modules** based on how helpful it has been for us. We don't release experimental code—we release battle-tested solutions that have proven their worth in production environments serving thousands of users.

---

## 🚀 Our Performance-Centric Philosophy

Performance isn't an afterthought—it's the foundation of everything we build. Whether you're working with **React hooks**, **Ruby gems**, or **Rust crates**, our libraries are engineered for:

- **Speed**: Optimized algorithms and minimal overhead
- **Core Web Vitals**: Built to improve LCP, INP, and CLS metrics
- **Tree-Shakability**: Import only what you need
- **Zero Configuration**: Sensible defaults that work out of the box
- **Production-Ready**: Thoroughly tested in high-traffic environments

---

## 📦 Open Source Libraries

### JavaScript/TypeScript (NPM)

#### [@page-speed/hooks](https://www.npmjs.com/package/@page-speed/hooks)
🚀 **Performance-optimized React hooks for Core Web Vitals, responsive images, lazy loading, and resource management.**

Drop-in implementations of web.dev best practices with zero configuration. Core performance tooling utilized by the high-performance OpenSite Octane™ website platform.

**Key Features:**
- Core Web Vitals optimization hooks
- Responsive image handling
- Intelligent lazy loading
- Resource preloading and prefetching
- Zero-config implementation

```bash
npm install @page-speed/hooks
```

---

#### [@page-speed/forms](https://www.npmjs.com/package/@page-speed/forms)
🚀 **Ultra-high-performance React form library with field-level reactivity and tree-shakable architecture.**

Type-safe form state management and validation designed for performance-critical applications.

**Key Features:**
- Field-level reactivity for minimal re-renders
- Tree-shakable exports for optimal bundle size
- TypeScript-first with full type inference
- Flexible validation schemas (sync and async)
- Multiple validation modes: `onChange`, `onBlur`, `onSubmit`

```bash
npm install @page-speed/forms
```

```jsx
import { useForm, Form } from '@page-speed/forms';

function MyForm() {
  const form = useForm({
    initialValues: { email: '' },
    validationSchema: {
      email: (value) => value.includes('@') ? undefined : 'Invalid email'
    },
    onSubmit: (values) => console.log('Submitted:', values)
  });

  return (
    <Form form={form}>
      <input
        name="email"
        value={form.values.email}
        onChange={(e) => form.setFieldValue('email', e.target.value)}
      />
      <button type="submit">Submit</button>
    </Form>
  );
}
```

---

### Ruby (RubyGems)

#### [domain_extractor](https://rubygems.org/gems/domain_extractor)
🔗 **Lightweight Ruby library for parsing URLs and extracting domain components with accurate multi-part TLD support.**

A high-performance URL parser and domain parser that excels at domain extraction tasks. Perfect for web scraping, analytics, URL manipulation, and multi-environment domain analysis.

**Key Features:**
- Accurate multi-part TLD parsing (co.uk, com.au, gov.br)
- Nested subdomain extraction
- Smart URL normalization
- Query parameter parsing
- Rails ActiveModel validator integration
- Batch URL processing
- IPv4 and IPv6 address detection

```bash
gem install domain_extractor
```

```ruby
require 'domain_extractor'

result = DomainExtractor.parse('https://api.staging.example.co.uk/path?query=value')

result[:subdomain]    # => 'api.staging'
result[:domain]       # => 'example'
result[:tld]          # => 'co.uk'
result[:root_domain]  # => 'example.co.uk'
result[:host]         # => 'api.staging.example.co.uk'
```

---

### Rust (Crates.io)

#### [markdown-ai-cite-remove](https://crates.io/crates/markdown-ai-cite-remove)
🧹 **High-performance Rust library for removing citations from ChatGPT, Claude, Perplexity, and other AI markdown responses.**

Removes inline citations, reference links, and bibliography sections with 100% accuracy. Built for AI content processing pipelines and markdown cleanup workflows.

**Key Features:**
- Removes inline citations `[1]`, `[2][3]`, etc.
- Strips reference link sections
- Cleans bibliography and source sections
- Zero-copy parsing for maximum performance
- Comprehensive AI platform support

```bash
cargo add markdown-ai-cite-remove
```

---

## 🛠️ Technology Stack

Our libraries are built with modern tooling and best practices:

| Platform | Technologies | Focus |
|----------|--------------|-------|
| **JavaScript/TypeScript** | React, TypeScript, Vite | Core Web Vitals, Performance Hooks |
| **Ruby** | Ruby 3.x, Public Suffix List | URL Parsing, Domain Extraction |
| **Rust** | Zero-copy parsing, Regex | High-throughput Text Processing |

---

## 🎯 Use Cases

### Web Performance Optimization
- Improve Lighthouse scores and Core Web Vitals
- Optimize React application rendering
- Implement lazy loading and resource management

### Analytics & Data Processing
- Parse and normalize URLs at scale
- Extract domain components for analytics pipelines
- Process AI-generated content for downstream use

### Web Scraping & Crawling
- Handle complex multi-part TLDs accurately
- Normalize and validate URLs
- Extract query parameters efficiently

---

## 🤝 Contributing

We welcome contributions from the developer community! Each repository has its own contribution guidelines, but here are some general principles:

1. **Fork** the repository you want to contribute to
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Reporting Issues

Found a bug or have a feature request? Please open an issue in the relevant repository with:
- Clear description of the issue or feature
- Steps to reproduce (for bugs)
- Expected vs. actual behavior
- Environment details (OS, language version, etc.)

---

## 📚 Documentation & Resources

- **Website**: [opensite.ai](https://opensite.ai)
- **Developer Portal**: [opensite.ai/developers](https://opensite.ai/developers)
- **Dev.to Articles**: [dev.to/opensite](https://dev.to/opensite)
- **LinkedIn**: [linkedin.com/company/opensite-ai](https://www.linkedin.com/company/opensite-ai)

---

## 📄 License

All OpenSite AI open source projects are released under permissive open source licenses. Check individual repositories for specific license details.

---

## 💡 About Octane™

Our open source libraries power **Octane™**, a high-performance visual website platform that allows businesses to dramatically improve their digital presence. The performance optimizations, hooks, and utilities you find here are the same ones driving thousands of production websites.

---

<p align="center">
  <strong>Built with ❤️ by the OpenSite AI team</strong>
  <br>
  <em>Performance is not optional—it's essential.</em>
</p>

---

### Keywords

`react hooks` `core web vitals` `performance optimization` `url parser` `domain extraction` `ruby gem` `rust crate` `npm package` `web performance` `lazy loading` `form validation` `typescript` `open source` `developer tools` `seo optimization` `pagespeed` `lighthouse` `ai tools` `markdown processing`
