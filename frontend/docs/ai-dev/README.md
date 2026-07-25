# AI Development Notes
This document records how AI tools were used during the development of the ATSEA scoreboard project. The project combines a React frontend, a Node-based WebSocket server, and an OBS-compatible overlay experience.

## List of AI tools, services, models, and their purposes
- GitHub Copilot: used for code suggestions, refactoring, boilerplate generation, and debugging help in TypeScript and React files.
- Claude: used for explaining code, brainstorming solutions, and reviewing logic.
- Codex: used for generating or refining code snippets and helping with implementation tasks.

### List of AI agents, including roles and skills
- Coding assistant: helped create and refine UI components, hooks, and server logic.
- Debugging assistant: helped trace issues in socket events, state updates, and rendering behavior.
- Review assistant: helped check for missing types, edge cases, and maintainability concerns before finalizing changes.

## Development Approach with AI
### Key prompts used
- “Help me create a React component for the scoreboard overlay with props for team names and scores.”
- “Review this TypeScript code for possible state or typing issues.”
- “Suggest how to connect this overlay UI to the WebSocket server without breaking the current flow.”
- "Give a basic structure on how to create a timer for the tournament"
- "Improve the design for the dropdown box"

### List of key review points and the corresponding decision made.
- UI structure: AI suggestions were used to organize components clearly, but final layout decisions were reviewed manually to match the intended overlay design.
- State handling: AI helped simplify state updates, but the final logic was checked carefully to avoid race conditions in real-time updates.
- Socket communication: event flow and reconnect behavior were reviewed closely because incorrect handling could break the scoreboard experience.
- Type safety: TypeScript definitions were improved with AI help, especially around scoreboard data and overlay props.
- OBS compatibility: visual and layout choices were checked against the overlay requirements so the result would remain usable in streaming setups.

## Reflection
- What worked well: AI was especially helpful for speeding up repetitive coding tasks, suggesting component structure, and explaining TypeScript issues quickly.
- What failed: the codes still required human judgment to make sure the experience felt correct and reliable. The prompt often does not give the results you wanted so you will still have to understand the code and how they work.
- Changes made: the workflow leaned on AI for implementation speed, while final decisions focused on maintainability, clarity, and project-specific requirements.
- Overall takeaway: AI is best used as a fast partner for drafting and refining work, but it is still important that all projects will need human review.
