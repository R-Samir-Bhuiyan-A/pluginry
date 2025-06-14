# 🧩 Pluginry

> A modular, pluggable Node.js framework — your blank canvas to build apps, APIs, or tools using fully customizable, installable plugins.

---

## 🚀 What is Pluginry?

**Pluginry** is a developer-first Node.js framework built from the ground up to be:

- 🧱 **Modular:** Everything is a plugin — routes, services, middleware, CLI tools, even core features.
- 🧩 **Pluggable:** Create or install premade plugins to extend functionality.
- 🖼️ **Blank Canvas:** Start from zero — only add what you need.
- ⚡ **Extensible:** Designed to scale from tiny microservices to large API backends or full app backends.
- 🛠️ **Hackable:** Transparent internals and accessible APIs for custom extensions.

---

## 🌐 Vision & Philosophy

Pluginry is **not a framework with opinions** — it’s a **platform to build your own custom backend**. Think of it like WordPress for backend developers, but built on Node.js and designed for APIs, tools, or full applications.

---

## 📦 Key Concepts

### 1. **Core**
A lightweight runtime engine that loads plugins, configures the environment, and starts your app.

### 2. **Plugins**
Self-contained units that can:
- Add routes
- Register services or helpers
- Hook into middleware chains
- Define CLI commands
- Include lifecycle events

### 3. **App Manifest**
A simple JSON or YAML file that declares what plugins should be loaded, and their order.

### 4. **Sandbox**
Each plugin runs in an isolated but connected context with scoped access to the Pluginry API.

---

## 🧱 Architecture Blueprint

### Core Engine Responsibilities:
- Load config
- Resolve & load plugins
- Expose shared context (`app`, `config`, `logger`, etc.)
- Manage lifecycle hooks (`onInit`, `onStart`, `onStop`)
- Mount routes and middlewares
- Run CLI if invoked directly

---

## 📁 Project Structure (Planned)
---

## ⚙️ Functional Goals (MVP v1)

### 🔌 Plugin System
- [ ] Plugin loader and registration
- [ ] Lifecycle hooks: `onLoad`, `onInit`, `onStart`, `onStop`
- [ ] Plugin manifest parsing (local or NPM-based)
- [ ] Plugin dependency tree resolution
- [ ] Plugin sandbox environment

### 🌐 HTTP Server (Express or Fastify-based)
- [ ] Plugin-defined routes and routers
- [ ] Plugin-defined middlewares
- [ ] Plugin-defined error handlers
- [ ] Custom route mounting support

### 🧰 Utility API
- [ ] Shared logger, config, env
- [ ] Plugin-local storage
- [ ] Access to app-wide services

### 🖥️ CLI
- [ ] `pluginry init` - create a new project
- [ ] `pluginry add` - add plugin from registry or local path
- [ ] `pluginry run` - start the app
- [ ] `pluginry list` - list loaded plugins and their hooks

---

## 🔮 Future Phases

### 📦 Plugin Registry
- Plugin discovery
- Plugin marketplace (possibly through npm or custom server)

### 📄 File-based Routing (optional plugin)
- Auto route generation based on file structure

### 💾 Database Plugin Layer
- ORM plugins (like Sequelize, Prisma)
- Migration plugins

### 🧑‍🤝‍🧑 Auth & RBAC Plugins
- Role-based access plugins
- JWT / OAuth plugins

### 🧪 Plugin Testing Harness
- Plugin test isolation
- Integration test utilities

### ⚡ Hot Reloading & Dev Mode
- Auto-reload plugins on file change

---

## 🛠️ Example Use Cases

- Build a RESTful API using plugin-defined endpoints.
- Create a microservice architecture with only what you need.
- Install plugins to handle authentication, validation, or payment.
- Share plugins across your internal tools or across teams.
- Build a custom CLI tool powered by Pluginry plugins.

---

## 📌 Guiding Principles

- **Minimal Core** – Start small, add features through plugins.
- **Developer First** – Transparent, hackable, and extensible.
- **Community-Driven** – Easy to build, share, and publish plugins.
- **Use What You Need** – No bloat, no assumptions.

---

## 🤝 Contributing

Pluginry will welcome contributors of all types — plugin creators, core developers, docs writers, testers.

Guidelines, roadmap, and plugin development documentation will live in the [`/docs`](./docs) folder.

---

## 🧪 Plugin Example Ideas (Coming Soon)

| Plugin Name       | Description                                 |
|-------------------|---------------------------------------------|
| `@pluginry/logger` | Adds a global logging service               |
| `@pluginry/router` | Mounts route definitions                    |
| `@pluginry/cli`    | Adds custom CLI commands                    |
| `@pluginry/db`     | ORM abstraction for SQL/NoSQL               |
| `@pluginry/auth`   | JWT or session-based auth                   |
| `@pluginry/ui`     | Static UI hosting or frontend bundler       |

---

## 📅 Development Timeline

| Phase | Features | ETA |
|-------|----------|-----|
| ✅ Phase 0 | Planning, structure, goals | DONE |
| 🛠️ Phase 1 | Core + Plugin loader + CLI | In Progress |
| ⏭️ Phase 2 | Web server + routing + example app | Soon |
| 🔜 Phase 3 | Plugin registry, DB plugins, Auth | Future |
| 🧪 Phase 4 | Testing tools, docs, community | TBD |

---

## 🔗 License

MIT License — open to community innovation.

---

> Build your backend, your way. One plugin at a time.

— **The Pluginry Team**
