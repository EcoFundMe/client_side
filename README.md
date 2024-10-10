# EcoFundMe
EcoFundMe: The Climate-Financing Crowdfunding Web3 Protocol

EcoFundMe is revolutionizing the way we fund climate projects and organizations. Our protocol harnesses the power of the decentralized Web3 ecosystem to bring together a community of like-minded individuals who are passionate about making a difference.

With EcoFundMe, you can support your favorite projects with ease, and earn rewards for your contributions. Our protocol is built on blockchain technology, ensuring that your investments are secure and transparent. You'll have full control over your funds, and be able to track your funds progress in real-time.

We believe everyone should be able to bring their ideas to life, regardless of their background or financial resources. That's why we've created a protocol that's accessible to everyone and focused on inclusivity and fairness.



## Table of Contents
- [Prerequisites](#prerequisites)
- [Setting Up the Project](#setting-up-the-project)
- [Running the Project](#running-the-project)
- [Common Issues and Solutions](#common-issues-and-solutions)
- [Project Structure](#project-structure)
- [Making Changes](#making-changes)
- [Using Git to Save Your Changes](#using-git-to-save-your-changes)
- [Contributing to the Project](#contributing-to-the-project)
- [Getting Help](#getting-help)
- [Learning More](#learning-more)

## Prerequisites

Before you can run this project, you need to install some tools. Don't worry if you don't know what these are - we'll explain each one:

1. **Git** - This helps you download and manage code
   - Go to [Git website](https://git-scm.com/)
   - Download the installer for your operating system:
     - Windows: Click "Download for Windows"
     - Mac: Click "Download for macOS"
   - Install Git:
     - Windows: Run the installer you downloaded. Click "Next" on each screen (the default options are fine)
     - Mac: Double click the downloaded file and follow the instructions
   - To verify installation:
     - Open Terminal (Mac) or Command Prompt (Windows)
     - Type `git --version` and press Enter
     - If you see a number like `2.35.1`, it worked!

2. **Node.js** - This is the engine that runs our code
   - Go to [Node.js website](https://nodejs.org/)
   - Download the "LTS" version (LTS means Long Term Support - it's the stable version)
   - Install it like any other program on your computer
   - To verify installation:
     - In Terminal (Mac) or Command Prompt (Windows)
     - Type `node --version` and press Enter
     - If you see a number like `v18.17.0`, it worked!

3. **Visual Studio Code** - This is where we'll write and edit code
   - Download from [Visual Studio Code website](https://code.visualstudio.com/)
   - Install it like any normal program

## Setting Up the Project

1. **Download the project**
   - Open Terminal (Mac) or Command Prompt (Windows)
   - Navigate to where you want to put the project:
     ```bash
     # On Windows, you might use:
     cd C:\Users\YourUsername\Documents

     # On Mac, you might use:
     cd ~/Documents
     ```
   - Clone (download) the project:
     ```bash
     git clone [your-repository-url]
     ```
   - If the above command gives an error, make sure you replaced [your-repository-url] with the actual URL of your project

2. **Open the project**
   - Open Visual Studio Code
   - Go to File → Open Folder
   - Find and select the project folder you just created
   - If asked "Do you trust the authors of the files in this folder?", click "Yes"

3. **Open the Terminal in Visual Studio Code**
   - Go to View → Terminal
   - A new panel will open at the bottom

4. **Install project dependencies**
   - In the terminal, type this command and press Enter:
     ```bash
     npm install
     ```
   - This might take a few minutes. You'll see lots of text scrolling by - that's normal!

## Running the Project

1. **Start the development server**
   - In the terminal, type:
     ```bash
     npm run dev
     ```
   - Wait until you see a message saying something like "ready - started server on 0.0.0.0:3000"

2. **View your project**
   - Open your web browser
   - Go to `http://localhost:3000`
   - You should see your project running!

## Common Issues and Solutions

### Git-related issues

#### "git is not recognized as an internal or external command"
- This means Git isn't installed correctly or needs a computer restart
- Try restarting your computer
- If that doesn't work, try reinstalling Git

#### "fatal: could not create work tree dir" error
- This usually means you don't have permission to create folders in that location
- Try running Command Prompt or Terminal as administrator (Windows) or using sudo (Mac)
- Or try cloning the repository to a different location

### Node.js issues

#### "npm not found" error
- This means Node.js isn't installed correctly
- Try reinstalling Node.js

#### "Port 3000 already in use" error
- Something is already running on port 3000
- Try closing other programs or tabs
- Or, in the terminal, press Ctrl+C (Windows) or Cmd+C (Mac) to stop the server, then try:
  ```bash
  npm run dev -- -p 3001
  ```
  This will run the project on port 3001 instead

## Project Structure

Here's what some important files and folders do:

- `pages/` - This is where your website's pages live
- `public/` - Put images and other files here
- `styles/` - This is where the appearance of your website is controlled
- `package.json` - Lists all the code libraries your project needs

## Making Changes

1. Most files ending in `.js` or `.tsx` contain your website's content
2. After making changes, save the file
3. The website will automatically update in your browser

## Using Git to Save Your Changes

After making changes, you can save them using Git:

1. **See what files you've changed**
   ```bash
   git status
   ```

2. **Prepare your changes to be saved**
   ```bash
   git add .
   ```

3. **Save your changes**
   ```bash
   git commit -m "Describe what you changed"
   ```

4. **Upload your changes**
   ```bash
   git push
   ```

## Contributing to the Project

We welcome contributions from everyone, even if you're new to coding! Here's how you can contribute:

### Setting Up for Contributing

1. **Fork the repository**
   - Go to the project's GitHub page
   - Click the "Fork" button in the top right
   - This creates your own copy of the project

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/PROJECT-NAME.git
   cd PROJECT-NAME
   ```
   Replace YOUR-USERNAME with your GitHub username and PROJECT-NAME with the repository name

3. **Set up the upstream remote**
   ```bash
   git remote add upstream https://github.com/ORIGINAL-OWNER/PROJECT-NAME.git
   ```
   Replace ORIGINAL-OWNER and PROJECT-NAME with the appropriate values

### Making Contributions

1. **Create a new branch for your feature**
   ```bash
   git checkout -b feature-name
   ```
   Replace 'feature-name' with a short description of your change (e.g., 'add-dark-mode')

2. **Make your changes**
   - Write your code
   - Test it to make sure it works
   - Add or update documentation if needed

3. **Commit your changes**
   ```bash
   git add .
   git commit -m "Description of your changes"
   ```
   Try to write a clear commit message that explains what you did

4. **Push your changes**
   ```bash
   git push origin feature-name
   ```

5. **Create a Pull Request (PR)**
   - Go to the original project's GitHub page
   - Click "Pull Requests"
   - Click "New Pull Request"
   - Click "compare across forks"
   - Select your fork and branch
   - Click "Create Pull Request"
   - Fill out the PR template if there is one

### Keeping Your Fork Updated

Before making new changes, always update your fork:

```bash
# Switch to main branch
git checkout main

# Get updates from the original repository
git fetch upstream

# Update your fork's main branch
git merge upstream/main

# Push the updates to your GitHub fork
git push origin main
```

### Contribution Guidelines

1. **Code Style**
   - Use consistent indentation (2 spaces)
   - Follow existing naming conventions
   - Add comments to explain complex code

2. **Commit Messages**
   - Start with a verb (Add, Fix, Update, etc.)
   - Keep it under 50 characters if possible
   - Use the description field for more details

3. **Pull Requests**
   - One feature or fix per PR
   - Update documentation if needed
   - Make sure all tests pass
   - Respond to any feedback

### For Beginners

If you're new to coding or open source, you can:
1. Start with issues labeled 'good first issue' or 'beginner-friendly'
2. Improve documentation
3. Report bugs you find
4. Add tests

Don't be afraid to ask for help! You can:
- Comment on the issue you're working on
- Join our [Discord/Slack] community
- Reach out to maintainers

### Code Review Process

After you submit a PR:
1. Maintainers will review your code
2. They might request changes
3. Once approved, your code will be merged

Don't worry if you're asked to make changes - it's normal and helps maintain code quality!

## Code of Conduct

We want to foster an inclusive and respectful community. Please:
- Be kind and courteous
- Respect different viewpoints
- Give and receive constructive feedback
- Focus on what's best for the community

Any form of harassment or disrespectful behavior is not tolerated.

## Getting Help

If you run into problems:
1. Double check all the steps above
2. Look for error messages in the terminal - they often tell you what's wrong
3. Google the error message - this is what professional programmers do too!
4. Check the project's documentation
5. Look for similar issues on GitHub
6. Ask in the project's [Discord/Slack] channel
7. Comment on the relevant issue

## Learning More

Ready to learn more? Here are some great resources:
- [Next.js Tutorial](https://nextjs.org/learn) - Official tutorial
- [Git Tutorial](https://www.atlassian.com/git/tutorials/what-is-git) - Learn more about Git
- [freeCodeCamp](https://www.freecodecamp.org/) - Free coding lessons
- [MDN Web Docs](https://developer.mozilla.org/) - Comprehensive web development documentation

---

Remember, everyone starts somewhere. Don't be afraid to make mistakes - that's how you learn!
