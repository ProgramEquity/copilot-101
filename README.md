# copilot-documentation Hack Pod 
Table of Contents: 
- [How to get started with installation ](https://github.com/ProgramEquity/copilot-documentation/tree/main#how-to-get-started-with-installation)https://www.youtube.com/watch?v=0dSKt4DgnyA
- [Best Practices](https://github.com/ProgramEquity/copilot-documentation/blob/main/README.md#best-practices)
  - For Prompt engineering inline
  - For Copilot Chat https://www.youtube.com/watch?v=whhq0-5ibac
- [Putting it into Practice in the Amplify Repo for Documentation](https://github.com/ProgramEquity/copilot-documentation/blob/main/README.md#putting-it-into-practice-in-the-amplify-repo-for-documentation-via-chat-prompts)
  - Readmes
  - Functions
  - Tests
  - Workflows
 

## How to get started with Installation 
https://www.youtube.com/watch?v=0dSKt4DgnyA

1. Prerequisites:
Ensure you have Visual Studio Code (VSCode) installed on your system. You can download it from https://code.visualstudio.com/.

2. GitHub Account:
You will need a GitHub account to access GitHub Copilot. If you don't have one, you can create an account at https://github.com/.

3. VSCode Extension Installation:
Open VSCode.
Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing Ctrl+Shift+X (Windows/Linux) or Cmd+Shift+X (macOS).
Search for "GitHub Copilot" in the search bar.
Click the "Install" button to install the extension.
4. Authentication:
After installation, you will be prompted to sign in with your GitHub account. Follow the on-screen instructions to authenticate.

5. License Activation:
If you have a GitHub Copilot subscription or a trial, you will need to activate your license.
6. Using GitHub Copilot:
GitHub Copilot will now be available to assist you while coding. You can start typing code, and it will provide context-aware suggestions and completions.

## Best Practices 
<img width="642" alt="Screenshot 2023-10-06 at 8 53 32 AM" src="https://github.com/ProgramEquity/copilot-documentation/assets/9143339/690ade6b-9b2f-4b5d-a404-835b475015b5">

1. Context Awareness
Provide context in your prompts to guide the model. Open up each file that is a dependency for the task at hand (Copilot can only draw context from open files in IDE not the entire codebase) 
2. Clarity and PrecisionWhen creating prompts or chat messages, be clear and precise in your instructions such as variable names or files or even the format you'd like the code. Mention the programming language, expected input, or the desired outcome.
3. 3. Start Simple
Begin with simple prompts and gradually increase complexity. This helps you understand how GitHub Copilot responds to different input.
4. Debugging and Refinement
Review and refine the generated code or chat responses carefully. Debugging may still be necessary.

### Copilot inline prompt engineering
- Use cases: auto complete code, documentation when using a readme 
- Ctrl + enter will create a large segment of code
- Having specificity in variable name will help create a pattern 

### Copilot Chat
- Use cases: documentation anywhere (including comments and explanations like ChatGPT), creating unit and API tests, refactoring code for a different language or complexity. 
- highlighting segments of code will help target your prompts
- Different prompts create different results when refactoring
  - Robust creates more validation
  - Readable creates comments
  - Faster creates more efficiency from an O notation compute

## Putting it into Practice in the Amplify Repo for Documentation via Chat prompts: 
Check out the project board here, depending on what you choose..here are some helpful prompts for
- Prompt engineering for readme/wiki for an API
- Functions
- Tests
- Workflows

### Readme: 
- Amplify readme: https://github.com/ProgramEquity/amplify
  - Improve readability
  - How would I get started with codespaces 
- API Wikis: https://github.com/ProgramEquity/amplify/wiki
  - Be sure to have the API files open as well https://github.com/ProgramEquity/amplify/tree/main/server/routes/api
  - highlight entire page and ask how do we use this API that is different than Public API
  - Which functions are using this API
  - Which test codes are we currently using 

### Functions: 
- Files are here: https://github.com/ProgramEquity/amplify/tree/main/server/routes/api
- To add comments: "Make this function more readable and concise"
- To create documentation in the discussion:
  - Ensure server files of [database](https://github.com/ProgramEquity/amplify/tree/main/server/db) are open: "Which data models does this function consume"
  - What dependencies does this function use
  - Bonus if you want to create issues for further work on the project: How would I refactor this to be more robust

### Tests: 
 - [Files are here](https://github.com/ProgramEquity/amplify/tree/main/server/__tests__)
 - highlight code snippet and type into chat "Explain this test to me"
 - general question and possible addition to wiki "why do we use jest framework", "what are advantages of jest over chai"
 - Bonus if you want to create issues for further work on the project: highlight code snippet and type into chat "how would I mock data for this" and "mock an array of data for this test". Make an issue out of the output. 
 - Bonus if you want to create issues for further work on the project: type in //add more post validation tests or //add in test for codes that aren't used yet

### Workflows:
- Files are here: https://github.com/ProgramEquity/amplify/tree/main/.github/workflows
- Create a wiki of all workflows by typing into chat "explain this to me and what endpoints are important" 
- Bonus: generate a mermaid.live graphic of all workflows
- Bonus: Make issues by asking to refactor for efficiency
- 


## Troubleshooting

- Reinstall the Copilot extension.
- Ensure you are signed into GitHub, either via CodeSpace or the web interface.
- If necessary, sign out of GitHub and then sign back in.
- Copilot will prompt you to allow access.
- Once access is granted, you can start using Copilot for enhanced coding assistance.
