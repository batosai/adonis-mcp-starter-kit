# AdonisJS(v7) Slim MCP Starter Kit

This repository provides the smallest possible AdonisJS application with the framework core and the Japa test runner, enhanced with MCP (Model Context Protocol) support.

It is designed as a minimal starting point for building AdonisJS applications that need to expose or integrate MCP capabilities (e.g., AI tool integration, structured context exchange, or agent-driven workflows), while keeping the codebase clean and lightweight.

# Tech Stack

<table>
  <tr>
    <td><strong>Backend</strong></td>
    <td>
      <a href="https://adonisjs.com">AdonisJS 7.x</a> - Full-featured Node.js framework
    </td>
  </tr>
  <tr>
    <td><strong>Package</strong></td>
    <td>
      <a href="https://adonis-mcp.jrmc.dev">AdonisJS MCP</a> - Model Context Protocol for AdonisJS
    </td>
  </tr>
  <tr>
    <td><strong>Testing</strong></td>
    <td>
      <a href="https://japa.dev">Japa</a> - Delightful testing framework with browser testing support
    </td>
  </tr>
  <tr>
    <td><strong>TypeScript</strong></td>
    <td>
      Full TypeScript support with strict mode enabled
    </td>
  </tr>
</table>

# Installation

```bash
npm init adonisjs@latest -- -K="batosai/adonisjs-mcp-starter-kit" --skip-migrations
cd adonisjs-app
npm run dev
```


## Start Developing

```bash
# Run the development server with hot reload
node ace serve --hmr

# Run tests
node ace test

# Type check both backend and frontend
npm run typecheck

# Lint your code
npm run lint

# Build for production
npm run build

# Start production server
npm start

# Create tool
node ace make:mcp-tool [tool name]

# Create resource
node ace make:mcp-resource [resource name]

# Create prompt
node ace make:mcp-prompt [prompt name]

```

Your app will be running at `http://localhost:3333`


## Exemple config server MCP in your app

You can use it as an HTTP server or via stdio (once published on npm).

```bash
npm start
{
  "name-server-mcp": {
    "command": "npx",
    "args": ["package-name"]
  },
  "name-server-mcp-http": {
    "url": "https://your-domaine.com/mcp",
    "headers": {
      # "Authorization": "Bearer token"
    }
  }
}
```


---

## Learn More

<table>
  <tr>
    <td>
      <a href="https://docs.adonisjs.com"><strong>📖 AdonisJS Docs</strong></a>
      <br>
      <span>Complete guide to AdonisJS</span>
    </td>
    <td>
      <a href="https://adonis-mcp.jrmc.dev"><strong>📖 AdonisJS MCP Docs</strong></a>
      <br>
      <span>Complete guide to AdonisJS MCP</span>
    </td>
  </tr>
</table>

## Contributing

This MCP starter kit is maintained by the Jeremy Chaufourier. Found a bug or have a suggestion? [Open an issue](https://github.com/batosai/adonisjs-mcp-starter-kit/issues) or submit a pull request!

---

## License

This MCP starter kit is open-sourced software licensed under the [MIT license](LICENSE).
