# GraphvizOnline AI

Based on [GraphvizOnline](https://github.com/dreampuf/GraphvizOnline) by [dreampuf](https://github.com/dreampuf/)

This enhanced version adds AI-powered diagram creation and editing capabilities to the original GraphvizOnline tool, allowing you to create and modify [GraphViz](http://www.graphviz.org/) diagrams using natural language.

## Live Demo

**[Try GraphvizOnline AI now at graphvizAi.maximilian.sh](https://graphvizAi.maximilian.sh)**

## New Features

-   **AI Chat Interface**: Create and modify diagrams by chatting with an AI assistant
-   **Modern UI**: Refreshed design with a unified top navigation bar and improved layout
-   **Enhanced Visualization**: Better zooming and panning controls for both SVG and PNG outputs
-   **Diff Highlighting**: Visual highlighting of changes when the AI suggests modifications
-   **Responsive Layout**: Collapsible panels for better use of screen space

## Setup & Usage

### API Key Requirement

This application requires a Groq API key to function:

1. Sign up for a Groq account at [groq.com](https://groq.com)
2. Generate an API key from your Groq dashboard
3. Enter the API key in the application by clicking the "API Key" button in the top navigation bar
4. Save the key (it will be stored in your browser's localStorage)

### Using the AI Assistant

Once your API key is set up:

1. Type a description of the diagram you want to create in the chat input
2. The AI will suggest Graphviz code to create your diagram
3. Review the highlighted changes in the editor
4. Accept or reject the suggested changes using the buttons that appear
5. Continue the conversation to refine your diagram

## Original GraphvizOnline Features

### Graph from URL / Gist

You can display a graph defined in a gist, or any other publically available url by adding a `?url=` parameter to the GraphvizOnline url

Example: https://graphvizAi.maximilian.sh/?url=https://gist.githubusercontent.com/timabell/da08616ecb8693d524b8eab3b7b51018/raw/0e205c341b40641206a55c9f96b5db9b8fa581bc/graph.gv

Using https://gist.github.com/ allows you to share and version your graph definitions.

### Presentation mode

If you would like to display just the graph and not the graph input, you can add a `?presentation` query param. This can be helpful when generating links with the graph already prefilled.

## Technologies Used

-   [Groq API](https://groq.com) - Powers the AI assistant using qwen-2.5-coder-32b model
-   [viz.js](https://github.com/mdaines/viz.js) - JavaScript port of Graphviz
-   [ACE-editor](http://ace.ajax.org/) - Code editor component
-   [svg-pan-zoom](https://github.com/ariutta/svg-pan-zoom) - Enhanced SVG navigation

## Deployment

To deploy this application:

1. Ensure you have added your own Groq API key using the UI
2. Push the repository to GitHub
3. Enable GitHub Pages in your repository settings or deploy to your preferred host
4. The official deployment is available at [graphvizAi.maximilian.sh](https://graphvizAi.maximilian.sh)

## Author

-   [Maximilian](https://github.com/maximilian-sh) - AI enhancements and modern UI
-   [dreampuf](https://github.com/dreampuf/) - Original GraphvizOnline creator

## License

GraphvizOnline AI is licensed under BSD-3 license. The dependencies:

-   [viz.js](https://github.com/mdaines/viz.js/blob/master/LICENSE) MIT
-   [ACE-editor](https://github.com/ajaxorg/ace/blob/master/LICENSE) BSD-2
