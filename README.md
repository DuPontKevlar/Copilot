# Copilot
This feature is somewhat similar to Github Copilot's code suggestion. But instead of using AI, it sends your search query to Google, then retrieves StackOverflow and Github Gist answers and autocompletes them for you.
To configure setting options, open the settings page by using hotkey Meta + ,, or:

Click on the Cog icon in the bottom left
Choose Settings
Settings options
Tick the checkbox of the following provider to enable

Github Gist
Stackoverflow
Open AI
Open Router
For Code Search (from Github Gist, StackOverflow)

Max results: the max number of search results return
For Code Generator

Open AI: Api Key: OpenAI API Key, see how to get OpenAI API Key. Required when using OpenAI provider
Open AI: Model: Model used to generate code. Model list is available at https://platform.openai.com/docs/models
Open Router: Api Key: OpenRouter API Key, see how to get OpenRouter API Key. Required when using OpenRouter provider
Open Router: Model: Model used to generate code. Model list is available at https://platform.openai.com/docs/models
Ai: N: Number of generated code outputs. Default is 1
Ai: Temperature: Code output creativeness, higher value will make the output more random (value between 0.0-1.0). Default is 0.5
Please note when using OpenRouter, X-Title and HTTP-Referer will be set as GasbyAI

2. How to use
To trigger inline completion, you'll need to type //find {your keyword}. (start with //find, end with a dot .)

For example

//find binary search in javascript.
Make sure Inline Suggest is enabled from the VS Code Settings

Note: Use Alt+] and Alt+[ to move through suggestions

3. Installation for Development
Check out the installation video: https://youtu.be/MD-kzsF0Scg

To install and starting Captain Stack:

Clone this repository to your PC using git clone https://github.com/hieunc229/copilot-clone.git .. Please note there is a dot at the end of the command

Run npm install in the terminal to install dependencies

Now, you can start the extension. From the top menu, choose Run > Start Debugging.

This will:

Start a task npm: watch to compile the code and watch for changes
Open a new VSCode window (you should use the extension there)
Note: When you make changes, you should refresh that window to apply changes. To refresh, open Command Palette (Command+Shift+P on MacOS, or Ctrl+Shift+P on Windows), then choose "Developer: Reload window"
