# Build it button

<img width="1150" alt="Screenshot 2023-11-17 at 2 38 14 PM" src="https://github.com/jordansinger/build-it-figma-ai/assets/110813/885bc2a1-cd34-41c7-b36b-ed1d5783e453">

Draw and sketch UI in Figma and FigJam with this widget. Inspired by [SawyerHood/draw-a-ui](https://github.com/SawyerHood/draw-a-ui) and [tldraw/draw-a-ui](https://github.com/tldraw/draw-a-ui).

Make sure to replace `OPENAI_API_KEY` with your API key in the `code.js` file.

---

Below are the steps to get your widget running. You can also find instructions at:

https://www.figma.com/widget-docs/setup-guide/

Once you have created a brand new widget, you can copy the contents of this repository into the widget folder that is created by Figma.

This widget template uses TypeScript and NPM, two standard tools in creating JavaScript applications.

First, download Node.js which comes with NPM. This will allow you to install TypeScript and other
libraries. You can find the download link here:

https://nodejs.org/en/download/

Next, install TypeScript, esbuild and the latest type definitions by running:

npm install

If you are familiar with JavaScript, TypeScript will look very familiar. In fact, valid JavaScript code
is already valid Typescript code.

TypeScript adds type annotations to variables. This allows code editors such as Visual Studio Code
to provide information about the Figma API while you are writing code, as well as help catch bugs
you previously didn't notice.

For more information, visit https://www.typescriptlang.org/

Using TypeScript requires a compiler to convert TypeScript (widget-src/code.tsx) into JavaScript (dist/code.js)
for the browser to run. We use esbuild to do this for us.

We recommend writing TypeScript code using Visual Studio code:

1. Download Visual Studio Code if you haven't already: https://code.visualstudio.com/.
2. Open this directory in Visual Studio Code.
3. Compile TypeScript to JavaScript: Run the "Terminal > Run Build Task..." menu item,
   then select "npm: watch". You will have to do this again every time
   you reopen Visual Studio Code.

That's it! Visual Studio Code will regenerate the JavaScript file every time you save.
