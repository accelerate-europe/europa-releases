# Europa

Europa is an AI agent made by Accelerate Europe (Vienna, Austria; https://accelerate-europe.org). It runs on your computer: each project gets its own virtual machine there, and the agent reaches a model only through Europa's gateway, which holds your key.

> **Early prototype, not released.** There is no download yet, the source code is not public yet, and everything may change. Please do not rely on it for real or sensitive work.

## What it is

Europa is an AI agent in an ordinary app window. You give it a task, such as analysing data, researching a question, writing a report or changing some code, and it works through the task with its own tools, showing you each step and the files it makes.

- **Isolated.** Each project has a Linux virtual machine of its own. The agent can run code and install software there, but it sees only the project's files and any folders you add, and it never holds your API keys.
- **Your choice of model.** Use a European or US provider, any service with a compatible API, or a model on your own computer. What the agent works on goes to the provider you choose, under its terms.
- **Clear about where your work goes.** Europa shows who runs each part of a task and where, and you can limit how far your work may go.

For now Europa is built for Windows, on [Pi](https://github.com/earendil-works/pi) and [Gondolin](https://github.com/earendil-works/gondolin). Downloads will appear in this repository, under Releases.

## Disclaimer

Europa is provided "as is", without warranty of any kind, express or implied, and you use it at your own risk. AI agents make mistakes, so check its work and keep backups. To the fullest extent permitted by law, no one involved in making it is liable for any loss or damage arising from its use.

## Licence

Copyright © 2026 Matthias Samwald. The source code is planned for publication under the GNU Affero General Public License, version 3 only (AGPL-3.0-only).
