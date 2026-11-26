# 2026-2027 Congressional App Challenge: Inkwell AI

This program was created by Ethan Cheng, a student and hack club member at Eleanor Roosevelt High School. It was created with his AP Computer Science Principals Class, and is the first major app creation project he worked on.

## Description
This program uses local AI models to check spelling and help refine text. It's aimed towards writers, students, and educators, who didn't want to pay larger services such as Grammarly's high subscription prices and didn't want their writing to be sent to external servers. It's these factors that prevent those groups of individuals from not being able to or preferring to use great AI grammar tools, so I decided to apply my recent interest in local AI models and create an app featuring this and fixing said problem for the Congressional App Challenge. I soon found that such models are more than capable to replace the simpler tools, and by building it myself, I could even talor specific commands for more niche use cases.

## How to Demo
Because my program is written on the Snap! platform, which is developed by UC Berkeley, I am unable to have the program run in GitHub Code Spaces, but I have attached the .xml file for the code itself, alongside the .html that shows it in a more understandable manner. Of course, there is no need of running those files since I have hosted my program online in the link below:

https://snap.berkeley.edu/snap/snap.html#present:Username=blockyethan&ProjectName=Ethan%20Cheng%20-%20CAC%20Inkwell%20App%20-%20Final

There are still a few more steps to properly run it! For starters, turn on Snap!'s JavaScript Extensions, by clicking on the cog at the top left, and clicking its checkbox. Then, be sure to install Ollama with a LLM within it, since that is where my program fetches the AI model. Also because the model would be running on-device, it is recommended to have a somewhat powerful or optimized device, like a Mac. For it to find this model, change the settings so it has the right local URL (it's usually: http://localhost:11434), as well as the right model name when is what Ollama identifies it as (this can be found in the model selection menu within the Ollama app). Lastly, you might have to run this command in the terminal/powershell, since Snap! lives on the web, which Ollama will reject requests from. Here is what you need to input:

**Windows Powershell:**
$env:OLLAMA_ORIGINS="*"
ollama serve

**MacOS Terminal:**
OLLAMA_ORIGINS="*" ollama serve

After all of this you can hopefully test out the program yourself!

## Features
- **Tools to fix grammar:** Within the code editor, there are multiple tools with their own AI prompts that ranges form common rewriting and proofreading, to more neache and specific tools that others are bound to also find useful.
- **Explanation of changes:** Once a tool is selected, the LLM would output its revised version, but also provide an explanation of its changes so the user can understand their mistakes or the change in tone.
- **Options for Outputs:** With the revised text, the user would then have the option to reject the reply, replace their current text with the revised version to further refine it, or copy it onto their universal clipboard.
- **Support for Many Models:** Since Inkwell AI uses Ollama to communicate with a local model, all the models supported through there could also be used to edit text the app.

## Built Using
1. Snap! Block Code: Particularly utilizing its pre-made block library, alongside its block system to understand and visualize code as a beginner
2. JavaScript: Certain advanced features were built using JavaScript Extensions as Snap! supports it, and is what allows it to communicate with local LLMs on the device, add to the user's universal clipboard, and extract font data from online.
3. Google Gemini AI: Used for certain areas of the block code to explain how Snap! worked and walk through them. This is since I am unfamiliar with Snap!, though I used other block code editors. It was also used to write all the JavaScript Extensions as I do not yet know the language. Nonetheless, most of the block coding was still done by me, from the text boxes, username integration, and navigation, to name a few.

## Screenshots
![Inkwell AI Start Screen](<./Inkwell AI - Start Screen.png>)
![Inkwell AI Editor Screen](<./Inkwell AI - Editor Screen.png>)
![Inkwell AI Settings Screen](<./Inkwell AI - Settings Screen.png>)

## Important Notes and Limiations
Because I built the entire program in Snap! and not Codespaces/VS Code, the hackatime extension would not be able to track the actual time I spent on this, and I instead thoroughly worked on this Readme file for an hour so I could qualify. That said, I have spent weeks working on the project, especially with documentation, planning, and feedback processes from my peers. I hope you understand the time it took me to compete this app as a beginner.

Also Note that Snap! is incapable of supporting proper text boxes with the way it was designed, so I had to find workarounds in implementing them. This makes that one of the most changing and largest aspect of the develop process, and could possibly break if used unideally.
