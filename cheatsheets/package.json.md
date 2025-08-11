# Package JSON

The `package.json` file is the central manifest for a **Node.js** project or **npm** package.
It defines the **identity**, **configuration**, and **behavior** of the package, serving both human readers and automated tools.
It contains metadata, scripts, dependencies, environment requirements, entry points, and publishing settings.

---

### **Metadata**

| Field          | Description                                                     |
| -------------- | --------------------------------------------------------------- |
| `name`         | Unique identifier of the package in npm (lowercase, no spaces). |
| `version`      | Version number following [semver](https://semver.org/).         |
| `description`  | Brief and clear summary of the package’s purpose.               |
| `keywords`     | List of search keywords for discovery and indexing.             |
| `homepage`     | Official website or main documentation URL.                     |
| `license`      | License type, following SPDX standards.                         |
| `author`       | Name and contact of the main author.                            |
| `contributors` | List of people who contributed to the project.                  |

---

### **Repository and Bugs**

| Field         | Description                                                   |
| ------------- | ------------------------------------------------------------- |
| `repository`  | Type and URL of the source code repository (e.g., Git).       |
| `bugs`        | URL and/or email for reporting issues and bugs.               |
| `GitHub URLs` | Additional links to the repository or organization on GitHub. |

---

### **Files and Structure**

| Field         | Description                                                          |
| ------------- | -------------------------------------------------------------------- |
| `files`       | List of files and directories included when publishing the package.  |
| `directories` | Mapping of internal directory locations (e.g., `lib`, `bin`, `man`). |
| `man`         | List of manual pages bundled with the package.                       |

---

### **Entry Points and Executables**

| Field     | Description                                                      |
| --------- | ---------------------------------------------------------------- |
| `main`    | Main entry file loaded via `require()` or `import`.              |
| `browser` | Alternative entry point for browser environments.                |
| `exports` | Export map for environment-specific entry points or subpaths.    |
| `bin`     | CLI command names and their corresponding executable file paths. |

---

### **Scripts and Configuration**

| Field     | Description                                            |
| --------- | ------------------------------------------------------ |
| `scripts` | Automation commands executable via `npm run`.          |
| `config`  | Custom configuration parameters accessible to scripts. |

---

### **Dependencies**

| Field                  | Description                                                     |
| ---------------------- | --------------------------------------------------------------- |
| `dependencies`         | Packages required at runtime in production.                     |
| `devDependencies`      | Packages needed only for development.                           |
| `peerDependencies`     | Dependencies expected to be provided by the consumer’s project. |
| `peerDependenciesMeta` | Additional metadata for `peerDependencies` (e.g., optional).    |
| `optionalDependencies` | Dependencies that can be installed but are not critical.        |
| `bundleDependencies`   | Dependencies bundled with the distributed package.              |
| `overrides`            | Version overrides for dependencies (npm 8+).                    |

---

### **Non-Standard / External Dependencies**

| Field                      | Description                                         |
| -------------------------- | --------------------------------------------------- |
| `URLs as Dependencies`     | Dependencies installed directly from URLs.          |
| `Git URLs as Dependencies` | Dependencies pulled directly from Git repositories. |
| `Local Paths`              | Dependencies referenced via local filesystem paths. |

---

### **Environment and Compatibility**

| Field        | Description                                       |
| ------------ | ------------------------------------------------- |
| `engines`    | Supported Node.js or npm versions.                |
| `devEngines` | Node.js or npm versions required for development. |
| `os`         | Supported operating systems.                      |
| `cpu`        | Supported CPU architectures.                      |
| `libc`       | Supported C libraries (e.g., `glibc`, `musl`).    |

---

### **Publishing and Organization**

| Field           | Description                                                     |
| --------------- | --------------------------------------------------------------- |
| `private`       | Prevents the package from being published to npm.               |
| `publishConfig` | Publishing configuration (e.g., registry URL).                  |
| `funding`       | Funding and sponsorship details.                                |
| `workspaces`    | Monorepo configuration for managing multiple packages together. |

---