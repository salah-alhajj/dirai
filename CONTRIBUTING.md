# Contributing to DIRAI

First off, thank you for considering contributing to **DIRAI: Your AI-Powered Directory Navigator**! 🚀 We're thrilled to have you join the movement to make directory analysis more insightful and engaging. Every contribution, big or small, helps us make DIRAI shine even brighter. ✨

This guide provides everything you need to know to contribute effectively. Please take a moment to read through it before submitting your work.

## Ways You Can Contribute

There are many ways to make a difference in the DIRAI project:

-   **🐛 Bug Reports:** Found a pesky bug? Let us know! Open an issue on GitHub with a clear description of the problem, steps to reproduce it, and details about your environment (OS, Python version, etc.).
-   **🌟 Feature Suggestions:** Have a brilliant idea to make DIRAI even better? Share it by opening an issue on GitHub. We're always open to new ideas and enhancements.
-   **💻 Code Contributions:**  Help us squash bugs, implement new features, or optimize existing code. Every line counts!
-   **📖 Documentation Improvements:** Help us make the documentation clearer, more comprehensive, or more accurate. Great documentation is crucial for a great user experience.
-   **🧪 Testing:**  Put your testing skills to work by helping us verify new features or bug fixes.
-   **📢 Spreading the Word:** Share DIRAI with others who might find it useful. Tell your friends, colleagues, or online communities about it.

## Getting Started: Your Contribution Journey Begins

1. **Fork the Repository:** Fork the DIRAI repository to your own GitHub account. This creates a copy of the project under your account where you can make your changes.
    
2. **Clone Your Fork:** Clone the forked repository to your local machine.
    
    ```bash
    git clone https://github.com/salah-alhajj/dirai.git 
    cd dirai
    ```
    
3. **Create a Branch:** Create a new branch for your contribution. Use a descriptive name that reflects the nature of your work. This helps keep the `main` branch clean and organized.
    
    ```bash
    git checkout -b feature/my-awesome-feature
    ```
    
    or
    
    ```bash
    git checkout -b bugfix/fix-that-bug
    ```
    
4. **Set Up Your Development Environment:**
    
    ```bash
    pip install -e .[dev]
    ```
    This installs DIRAI in editable mode along with development dependencies like `pytest` for testing.
    
5. **Make Your Changes:** Implement your changes, write tests, and update documentation as needed.
    
6. **Commit Your Changes:** Commit your changes with clear and concise commit messages. We recommend following the [Conventional Commits](https://www.conventionalcommits.org/) specification for better commit message structure. This makes it easier to understand the history of the project.
    
7. **Push Your Changes:** Push your branch to your forked repository.
    
    ```bash
    git push origin your-branch-name
    ```
    
8. **Open a Pull Request:** Go to the original DIRAI repository on GitHub and open a pull request from your branch to the `main` branch.
    

## Development Guidelines: Best Practices for DIRAI

### Code Style: The DIRAI Way

-   Adhere to [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guidelines. We use `flake8` to enforce this. You can run `flake8` locally before committing to check for style issues.
-   Use meaningful variable and function names that clearly indicate their purpose.
-   Write clear and concise comments to explain complex logic or non-obvious code.
-   Keep functions and methods short and focused on a single task.

### Testing: Ensuring DIRAI's Reliability

-   Write unit tests for your code using the `pytest` framework.
-   Aim for high test coverage, ensuring that your tests cover all new functionality and edge cases.
-   Run tests locally before submitting a pull request to catch issues early:
    
    ```bash
    pytest
    ```
    

### Documentation: Illuminating the Path

-   Update the documentation (including the README) to reflect any changes you make.
-   Clearly document any new features or functionalities you add.
-   Ensure the documentation is easy to understand and follow.

## Pull Request Process: From Proposal to Integration

1. **Submit a Pull Request:** Once your changes are ready, submit a pull request to the `main` branch of the DIRAI repository.
    
2. **Describe Your Changes:** In the pull request description, provide a clear and detailed explanation of:
    
    -   The purpose of your changes.
    -   The problem you are solving (if applicable).
    -   The approach you have taken.
    -   Any relevant issue numbers.
    
    The more context you provide, the easier it will be for reviewers to understand your contribution.
    
3. **Code Review:** Your pull request will be reviewed by the maintainers. Be prepared to address feedback, answer questions, and make changes if necessary. This is a collaborative process, and we appreciate your patience and responsiveness.
    
4. **Approval and Merge:** Once your pull request is approved, it will be merged into the `main` branch, and your contribution will become part of DIRAI! 🎉
    

## Code of Conduct: Fostering a Positive Community

Please note that this project has a [Code of Conduct](CODE_OF_CONDUCT.md) (you'll need to create this file). By participating in this project, you agree to abide by its terms. We strive to create a welcoming and inclusive environment for everyone.

## Questions and Support: We're Here to Help

If you have any questions or need help with contributing, feel free to open an issue on GitHub or reach out to the maintainers. We're happy to assist you in any way we can.

## Thank You!

Thank you again for your interest in contributing to DIRAI. Your contributions are invaluable and help make DIRAI an even more powerful and user-friendly tool. We appreciate your time, effort, and dedication to the project! 🌟




<p align="center">
  Made with ❤️ by developers, for developers.
</p>
---