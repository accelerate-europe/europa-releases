# Europa

Europa is an AI agent made by Accelerate Europe (Vienna, Austria; https://accelerate-europe.org). It runs on your computer: each project gets its own virtual machine there, and the agent reaches a model only through Europa's gateway, which holds your key.

> **An early version, for trying out.** Europa 0.2.0 is the first you can download, for Windows. Expect rough edges, and do not rely on it yet for real or sensitive work: the source code is not public yet, and everything may change.

## Download

**Windows 10 or 11, 64-bit:** open the [latest release](https://github.com/accelerate-europe/europa-releases/releases/latest) and download the file ending in `-setup.exe` (about 80 MB).

A version for Mac is in the works.

## Install and start

1. **Open the file you downloaded.** Europa installs for you alone and needs no administrator.
2. **If Windows says "Windows protected your PC",** choose "More info", then "Run anyway". Windows says this because the installer is not yet signed with a code-signing certificate.
3. **On its first start, Europa downloads its agent** (about 450 MB, once).
4. **Connect a model provider.** This is a service that runs the AI models; you pay it for what you use. Europa recommends a European one, and opens its page so you can get a key. Europa shows what each conversation costs.
5. **Try it with the sample report:** Europa adds a short made-up report and a task to start from.

If "Windows Hypervisor Platform" is off on your computer, Europa still starts, but runs the agent more slowly. It offers to turn the feature on, which takes an administrator's permission and a restart of Windows.

## Updates

Europa looks for a new version when it starts, and once a day. It fetches one small file from this repository, which tells nothing about you or your work. When there is a new version, Europa says so, and installs it only when you choose "Restart and update". It installs only versions that carry Europa's signature. You can turn the daily look off in Settings › About.

## What it is

Europa is an AI agent in an ordinary app window. You give it a task, such as analysing data, researching a question, writing a report or changing some code. It works through the task with its own tools, showing you each step and the files it makes.

- **Isolated.** Each project has a Linux virtual machine of its own. The agent can run code and install software there, but it sees only the project's files and any folders you add, and it never holds your API keys.
- **Your choice of model.** Use a European or US provider, any service with a compatible API, or a model on your own computer. What the agent works on goes to the provider you choose, under its terms.
- **Clear about where your work goes.** Europa shows who runs each part of a task and where, and you can limit how far your work may go.

Europa has no account of its own and sends no usage data. Apart from the model provider you choose and the services you add yourself (such as MCP servers or packages), it reaches:

- this repository on GitHub, for the agent and for updates;
- the European Central Bank, for the dollar's daily rate, so it can show costs in euros;
- the search service it shows you, when you let the agent search the web.

Europa is built on [Pi](https://github.com/earendil-works/pi) and [Gondolin](https://github.com/earendil-works/gondolin).

## Problems and questions

Please open an issue in [this repository's Issues](https://github.com/accelerate-europe/europa-releases/issues): what you did, what you expected, and what happened instead. Issues are public, so leave out anything private.

Europa writes what it does to `%LOCALAPPDATA%\Europa\logs\europa.log`, which helps when something goes wrong. Look through it before you share any of it.

## Disclaimer

Europa is provided "as is", without warranty of any kind, express or implied, and you use it at your own risk. AI agents make mistakes, so check its work and keep backups. To the fullest extent permitted by law, no one involved in making it is liable for any loss or damage arising from its use.

## Licence

Copyright © 2026 Matthias Samwald. The source code is planned for publication under the GNU Affero General Public License, version 3 only (AGPL-3.0-only).

The installer includes QEMU (GNU GPL 2.0) and Node.js (MIT). Where to find their source code is listed in `notices\README.txt` of the installed program.
