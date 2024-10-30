# npm-package-starter

A template for creating npm packages with TypeScript, Prettier, and automated testing. This starter provides essential scripts for building, formatting, linting, testing, and releasing your package.

## Getting Started

### Prerequisites

- **Node.js** (v14 or later recommended)
- **npm** (v6 or later)

### Installation

Clone this repository and install the dependencies:

```bash
git clone https://github.com/ramthenmala/npm-package-starter
cd npm-package-starter
npm install
```

### Scripts

Here’s an overview of the scripts included in this starter:

#### 1. **Build**

Compile TypeScript code into JavaScript.

```bash
npm run build
```

#### 2. **Code Formatting**

Use Prettier to format code. This starter includes scripts to both format code and check if the code is correctly formatted.

- **Format Code**  
  Automatically format all files in the project:
  ```bash
  npm run format
  ```

- **Check Formatting**  
  Check if the code is formatted correctly (without modifying files):
  ```bash
  npm run check-format
  ```

#### 3. **Linting**

Lint the TypeScript code by running the TypeScript compiler.

```bash
npm run lint
```

#### 4. **Check Exports**

This script ensures all exports are correctly configured, using `attw` to validate against common module resolution issues.

```bash
npm run check-exports
```

#### 5. **Run All CI Scripts**

This script will run the build, format check, exports check, lint, and test scripts in sequence to ensure everything passes before publishing.

```bash
npm run ci
```

#### 6. **Testing**

Testing is handled with [Vitest](https://vitest.dev/), a fast and lightweight testing framework.

- **Run All Tests Once**  
  Run the tests a single time for CI purposes:
  ```bash
  npm run test
  ```

- **Watch Mode**  
  Run tests in watch mode during development:
  ```bash
  npm run dev
  ```

#### 7. **Local Release**

Use [Changesets](https://github.com/changesets/changesets) to manage and publish versioned releases.

- **Version Update**  
  Increment the package version and prepare for release:
  ```bash
  npm run local-release
  ```

### Publishing

This package is configured to run all checks before publishing. Once you’re ready to publish, make sure to log in to npm and publish with:

```bash
npm publish
```

### Contributing

Contributions are welcome! If you’d like to make changes, please open a pull request.