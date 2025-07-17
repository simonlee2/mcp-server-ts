# MCP Server TypeScript Template

A simple template for creating MCP (Model Context Protocol) servers in TypeScript.

## Features

- **Addition Tool**: Demonstrates a basic tool that adds two numbers
- **Greeting Resource**: Shows dynamic resource generation with URL parameters
- **TypeScript**: Full TypeScript support with strict mode
- **Modern ES Modules**: Uses the latest JavaScript module system

## Quick Start

1. **Install dependencies**:
   ```bash
   pnpm install
   ```

2. **Build the server**:
   ```bash
   pnpm build
   ```

3. **Run the server**:
   ```bash
   ./build/index.js
   ```

## Usage

This template provides two examples:

### Tools
- `add`: Adds two numbers together
  ```json
  { "a": 5, "b": 3 }
  ```

### Resources
- `greeting://{name}`: Generates a personalized greeting
  ```
  greeting://Alice
  ```

## Extending

To add your own tools and resources:

1. Use `server.registerTool()` for new tools
2. Use `server.registerResource()` for new resources
3. Follow the existing patterns in `src/index.ts`

## Development

- Source code: `src/index.ts`
- Build output: `build/`
- TypeScript config: `tsconfig.json`

## License

MIT 