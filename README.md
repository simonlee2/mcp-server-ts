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
   pnpm start
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

## Development

### Available Scripts

- **`pnpm dev`** - Watch mode development (auto-rebuilds on changes)
- **`pnpm build`** - Build the project
- **`pnpm start`** - Run the built server
- **`pnpm clean`** - Clean build directory
- **`pnpm lint`** - Check code for linting issues
- **`pnpm lint:fix`** - Auto-fix linting issues
- **`pnpm format`** - Format code with Prettier
- **`pnpm type-check`** - Check TypeScript types without building

### Development Workflow

1. **Start development**:
   ```bash
   pnpm dev
   ```
   This starts TypeScript in watch mode - your code will auto-rebuild on changes.

2. **Code quality** (run before committing):
   ```bash
   pnpm lint:fix
   pnpm format
   pnpm type-check
   ```

3. **Test your server**:
   ```bash
   pnpm build
   pnpm start
   ```

### Code Quality

This template includes:
- **ESLint** - TypeScript linting with recommended rules
- **Prettier** - Code formatting
- **TypeScript** - Strict type checking

### Project Structure

- `src/index.ts` - Main server implementation
- `build/` - Compiled output
- `tsconfig.json` - TypeScript configuration
- `.eslintrc.js` - ESLint configuration (create as needed)
- `.prettierrc` - Prettier configuration (create as needed)

## Extending

To add your own tools and resources:

1. Use `server.registerTool()` for new tools
2. Use `server.registerResource()` for new resources
3. Follow the existing patterns in `src/index.ts`
4. Run `pnpm lint:fix` and `pnpm format` to maintain code quality

## License

MIT 