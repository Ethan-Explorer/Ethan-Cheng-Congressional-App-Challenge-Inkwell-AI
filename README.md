# 2026-2027 Congressional App Challenge: Inkwell AI

This program was created by Ethan Cheng, a student and follow hack club member at Eleanor Roosevelt High School. It was created with his AP Computer Science Principals Class, and is the first major app creation project he worked on.

## Description
This program uses local AI models to check spelling and help refine text. Its aimed towards writers. students, and educators, who didn't want to pay larger services such as Grammarly's high subscription prices and didn't want their writing to be sent to external servers. Its these factors that prevent such group of indivudals to not be abel to or prefer to use these great AI tools, but after just recently looking into local AI models due to their recent increase in popularity, I decided that such models are more than capable to fix simple spelling and developing my own program for the congressional app challenge would allow me to even talor specific commands for more neche needs.

## How to Demo
Becuase my program is written on the Snap! platform, which is developed by UC Berkely, I am unable to have the program run in github code spaces, but I have attached the .xml file for the code iself, alongside the .html that shows it in a more understandable manner. Of course, there is no need of running those files since I have hosted my program online in the link below:

https://snap.berkeley.edu/snap/snap.html#present:Username=blockyethan&ProjectName=Ethan%20Cheng%20-%20CAC%20Inkwell%20App%20-%20Final

There are still a few more steps to properly run it! For starters, turn on Snap!'s JavaScript Extensions, by clicking on the cog at the top left, and clicking its checkbox. Then, be sure to install Ollama with a LLM wthin it, since that is where my program fecthes the AI model. For it to find this model, change the settings so it has the right local URL (Its usually: http://localhost:11434), as well as the right model name when is what Ollama identifes it as (this can be found in the model selection menu within the Ollama app). Lastly, you might have to run this command in the terminal/powershell, since Snap! lives on the web, which Ollama will reject requests form. Here is what you need to input:

**Windows Powershell:**
$env:OLLAMA_ORIGINS="*"
ollama serve

**MacOS Terminal:**
OLLAMA_ORIGINS="*" ollama serve

After all of this you can hopfully test out the program yourself!

## Screenshots
![Inkwell AI Start Screen](<./Inkwell AI - Start Screen.png>)
![Inkwell AI Editor Screen](<./Inkwell AI - Editor Screen.png>)
![Inkwell AI Settings Screen](<./Inkwell AI - Settings Screen.png>)

## Features
- **Tools to fix grammer:** Within the code editor, there are mutipule tools with their own AI prompts that renages form common rewriting and proofreading, to more neache and speicifc tools that others are bound to also find useful.
- **Expliantion of changes:** Once a tool is selected, the LLM would output its revised version, but also provide a explination of its changes so the user can understand their mistakes or the change in tone.
- **Options for Outputs:** With the revised text, the user would then have the option to reject the reply, replace their current text with the revised version to further refine it, or copy it onto their universal clipboard
- **Support for Many Models:** Since Inkwell AI uses Ollama to communitate with a local model, all the models suppored through there could also be used to edit text the app.

## Built With
1. Snap! Block Code: Perticualrly utilizing its pre-made block libary, alonsgide its block system to undertsand and viusalize code as a beginner
2. JavaScript: Certain advanced features were built using JavaScript Extensions as Snap! supports it, and is what allows it to communicate with local LLMs on the device, add to the user's univeral clipboard, and extract font data from google.
3. Google Gemini AI: Used for certain areas of the block code to expain how Snap! worked and walk through them. This is since I am unfilumlar with Snap!, though I used other block code editors. It was also used to write all the JavaScript Extensions as I do not yet know the language. Nonetheless, most of the block coding was still done by me, from the text boxes, usernmae intergartion, and naviuagtion, to name a few.

## Important Notes and Limiations
Becuase I built the entire program in Snap! and not codespaces/VS Code, the hackatime extension would not be able to track the actaul time I spent on this, and I instead thoughly worked on this Readme file for an hour so I could qualify. That said, I have spent weeks working on the project, especally with documentation, planning, and feedback processes from my peers. I hope you understand the time it took me to compete this app as a beginner.
Also Note that Snap! is incabale of supportiung proper text boxes with the way it was designed, so I had to find workarounds in impenting them. This makes that one of the most changeing and largerest aspect of the develop porcess, and could posibly break if used unidealy.