# Contributing to UAH Token List Toolkit

Thank you for your interest in contributing to this customized token list toolkit! This guide outlines the steps to efficiently add new tokens or contribute code improvements.

## Adding New Tokens

1.  **Fork** this repository to your own GitHub account.
2.  **Clone** your fork locally.
3.  **Create a New Branch:**
    ```bash
    git checkout -b feat/add-new-token-name
    ```
4.  **Add Token Data:**
    Modify the primary source file by adding your token data objects:
    `packages/token-lists/src/tokens/pancakeswap-default.json`

5.  **Run Compilation:**
    Use the pre-configured script (it includes the necessary workarounds):
    ```bash
    cd packages/token-lists
    yarn run makelist:pcs-default
    ```
    *(Ensure you run `yarn install` first if you haven't yet.)*

6.  **Commit Your Changes:**
    Commit both the source file and the generated list file (`lists/pancakeswap-default.json`):
    ```bash
    git add packages/token-lists/src/tokens/pancakeswap-default.json
    git add packages/token-lists/lists/pancakeswap-default.json
    git commit -m "feat: Add [Your Token Name] token and regenerate list"
    ```

7.  **Create a Pull Request (PR):**
    Push your branch to your fork and open a Pull Request against the `main` branch of this repository.

## Technical Contribution

If you have a solution to the Windows/Jest `TypeError` (instead of the current bypass) or other technical improvements, please open an Issue first to discuss your proposed change.