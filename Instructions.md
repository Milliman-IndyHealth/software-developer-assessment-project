# Intern Candidate Project Instructions

Welcome! This project is part of your evaluation for our Software Developer Intern position. You will be working with a Blazor web application that has a few bugs to fix and features to implement. Please read these instructions carefully before getting started. Please feel free to use any AI tools that you would like, but make sure that you understand the changes that are being made so that you can explain them during follow up conversations.

---

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- [**Latest .NET 10 SDK**](https://dotnet.microsoft.com/en-us/download/dotnet/10.0)
- [**Visual Studio 2026**](https://visualstudio.microsoft.com/) (Community edition or higher), [**Visual Studio Code**](https://code.visualstudio.com/) with the C# Dev Kit extension, or your preferred code/text editor.
- [**Git**](https://git-scm.com/downloads) installed and available on your command line.
- A [**GitHub account**](https://github.com/) (free tier is fine).

> **Note:** If you do not have these tools installed or can't install them for some reason and need assistance, please reach out so that we can identify a resolution.

---

## Getting Started

1. **Fork the repository**
   - Navigate to the project repository on GitHub: [**Milliman-IndyHealth/software-developer-assessment-project**](https://github.com/Milliman-IndyHealth/software-developer-assessment-project)
   - Click the **Fork** button in the upper-right corner to create a copy under your own GitHub account.
   - **Important:** Make sure your fork is set to **Private**. On the fork-creation page, check the option to make the repository private. If your GitHub plan does not support private forks, see the note below.

   > **Note:** If you are unable to create a private fork, you may instead create a **new private repository** on your account, clone the original repo locally, change the remote to point to your new private repo, and push. Reach out if you need help with this.

2. **Clone your fork** to your local machine:
   ```
   git clone https://github.com/<your-username>/software-developer-assessment-project.git
   ```
   Replace `<your-username>` with your GitHub username.

3. **Open the project** in Visual Studio, Visual Studio Code, or your preferred code editor.

2. **Run the application**:
   - **Visual Studio**: Press `F5` or click the green "Run" button.
   - **Command line**:
     ```
     dotnet run
     ```
     **OR**
     ```
     dotnet watch run
     ```
   - Depending on the IDE and your configuration the application may open in your browser. If it doesn't, navigate to the URL shown in the terminal output in a browser window (typically `http://localhost:5277`).

3. **Verify the application is running** by confirming you can see the Home page in your browser.

> **Note:** The first time the application runs you may be asked to generate and trust a self-signed development certificate.

---

## What You Need to Accomplish

Your task is to fix **4 bugs** and implement **3 features** in the application. Details for each are below.

### Bugs to Fix

1. **"Hello, world!" on the Home page should include your name**
   - The Home page currently displays "Hello, world!"
   - Change it to display "Hello, \{Your Name\}" (with your actual name)
   - Your name can be hard-coded in the text

2. **The Reset button on the Counter page doesn't work**
   - Navigate to the Counter page and try the Reset button
   - The Reset button should reset the counter back to **0** when clicked
   - Find and fix the issue so that it works correctly

3. **The Weather forecast data only shows 5 days instead of 15**
   - Navigate to the Weather page
   - The forecast table should display **15 days** of future data, but currently only shows 5
   - Find and fix the issue

4. **The wrong favicon is being used**
   - The application is currently using `favicon.png` but should use `favicon.ico`
   - The `favicon.ico` file is already included in the `wwwroot` folder
   - Update the application to reference the correct file

### Features to Implement

1. **Create an "About Me" page**
   - Create a new `.razor` component in the `Components/Pages` folder
   - The page should be accessible at the URL `/aboutme`
   - Add a link to the new page in the NavMenu (left sidebar)
   - The page should have a header that says **"About Me"**
   - Include the following content on the page:
     - Your name
     - A list of your technical skills
     - A description of what makes you the best choice for this position

2. **Add a "Decrement Count" button to the Counter page**
   - Add a new "Decrement Count" button **before** the existing "Increment Count" button
   - Clicking the button should decrease the count by 1
   - The count should **never go below 0**
   - When the count is already 0, clicking the button should have no effect

3. **Add a link to your GitHub profile in the header**
   - Add a link to your GitHub profile (or another professional profile if you don't have GitHub)
   - The link should be placed in the application header — look for the `<!--GitHub Profile Link-->` comment in the code
   - The link should open in a **new tab** when clicked
   - The link can be displayed as an icon or text — your choice

---

## Submitting Your Work

1. **Commit and push** all of your changes to your forked repository:
   ```
   git add .
   git commit -m "Completed assessment"
   git push origin main
   ```
2. **Grant repository access** — add the following GitHub users as collaborators on your fork so we can review your work:
   - `michael-reisz`
   - `tom-puckett`

   To add collaborators: go to your fork on GitHub → **Settings** → **Collaborators** → **Add people**.

3. **Send a notification email** to `IndyRecruiting@milliman.com` (CC `michael.reisz@milliman.com` and `tom.puckett@milliman.com`) with:
   - A link to your forked repository.
   - Confirmation that you have granted access to the reviewers listed above.

---

## Evaluation Criteria

Your submission will be evaluated on the following areas:

### Bug Fixes (30%)
- Did you correctly identify and fix all 4 bugs?
- Do the fixes work as expected without introducing new issues?

### Feature Implementation (45%)
- Are all 3 features implemented according to the requirements?
- Does the "About Me" page include all required content and is it accessible from the NavMenu?
- Does the Decrement button work correctly, including the edge case of not going below 0?
- Does the GitHub profile link open in a new tab and appear in the correct location?

### Code Quality (25%)
- **Cleanliness**: Is your code free of unused code, commented-out blocks, and unnecessary complexity?
- **Consistency**: Does your code follow the patterns and conventions already established in the project?
- **No regressions**: Does existing functionality still work after your changes?

### Bonus Observations (not scored, but noted)
- Did you go above and beyond on any task?
- Did you consider accessibility in your implementation?
- Did you handle any edge cases beyond what was specified?
- Is the "About Me" page content thoughtful and well-presented?

---

## Tips for Success

- **Read through the existing code** before making changes — understand the patterns being used
- **Test your changes** after each bug fix or feature implementation
- **Don't overthink it** — the tasks are designed to be straightforward
- **Be able to explain how your application works** - In follow up conversations you will likely be asked about your submission
- **Commit often** — small, well-described commits help us understand your thought process
- If something is unclear, make your best judgment and document it in your notification email

---

## Questions?

If you have questions about the setup or requirements, please reach out to `michael.reisz@milliman.com`. We want to evaluate your technical skills, not your ability to work through ambiguous setup issues.

Good luck!
