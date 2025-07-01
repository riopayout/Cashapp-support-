# create-openapi-repo

A tool for generating multi-file OpenAPI definitions.

[![NPM version][npm-image]][npm-url] [![Dependency Status][daviddm-image]][daviddm-url]

<p align="center">
<img src="./logo.png" width="500px"/>
</p>

Need to write or contribute to an OpenAPI definition? `create-openapi-repo` can help with that!

## Features

 - OpenAPI 3.0 support
 - Split an existing OpenAPI definition into multiple files
 - Bundle a multi-file definition into a single file
 - Validate your OpenAPI definition using our free [openapi-cli tool](https://github.com/redocly/openapi-cli)
 - Automate deployment of your API reference docs using CI/CD workflows
 - Maintain code samples as separate files
 - Live editing in your editor of choice :heart_eyes:

## Examples
- [Rebilly](https://github.com/Rebilly/RebillyAPI)
- [Thingful](https://github.com/thingful/openapi-spec)

## Prerequisites

Before you begin, make sure you have the following prerequisites:

 - [Node.js](https://nodejs.org/)
 - [Github repository](https://help.github.com/articles/create-a-repo/#create-a-new-repository-on-github) (new OpenAPI definitions only)

## Installation

1. Navigate to the location where you want to create the repository.
2. Run one of the following commands:
   - Install `create-openapi-repo` globally:

        ```bash
        npm install -g create-openapi-repo
        ```

   - Install `create-openapi-repo` using [`npx`](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b):

        ```bash
        npx create-openapi-repo
        ```

3. Follow the [interactive prompts](https://github.com/Redocly/create-openapi-repo#usage) to complete the installation.

### Upgrading from a prior version

To upgrade from a prior version of `create-openapi-repo`, run the following command in the root folder of your repository:

```bash
npx create-openapi-repo --migrate-2-3
```

**Note:** Plugins aren't included in the migration. You'll need to manually add them to the `transformers` folder.

## Usage

`create-openapi-repo` provides interactive prompts to help guide you through the installation process. Two basic workflows are supported:

### Split an existing OpenAPI definition

The interactive prompts allow you to specify the path to the file on your local machine, as well as rename the API (optional). After you choose to proceed, `create-openapi-repo` initializes the repository and splits your OpenAPI definition into multiple files.

### Create a new OpenAPI definition
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Asonex - The Stone of Clarity</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            background: #f4f4f9;
            color: #333;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 30px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            border-radius: 10px;
        }
        h1, h2 {
            color: #4B0082;
        }
        ul {
            list-style-type: disc;
            padding-left: 20px;
        }
        .footer {
            margin-top: 40px;
            font-size: 0.9em;
            color: #888;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Asonex: The Stone of Clarity and Connection</h1>
        <p>In the ever-expanding world of rare gems and spiritual talismans, a new name is beginning to shimmer in mystic circles and artisan workshops: <strong>Asonex</strong>.</p>

        <h2>What Is Asonex?</h2>
        <p><em>Asonex</em> is a fictional but beautifully imagined gemstone known for its soft transitions between <strong>violet and sapphire</strong> hues. It is said to radiate calm, balance, and heightened awareness to those who hold or wear it.</p>

        <h2>The Meaning Behind the Name</h2>
        <p>The name <em>Asonex</em> is a fusion of ancient roots:</p>
        <ul>
            <li><strong>Asō</strong> – an old term for <em>light</em></li>
            <li><strong>Nexis</strong> – meaning <em>connection</em> or <em>link</em></li>
        </ul>
        <p>Together, they suggest a stone that bridges the spiritual and emotional, allowing its wearer to find clarity in chaos.</p>

        <h2>Cultural Lore & Symbolism</h2>
        <p>According to modern fantasy lore, Asonex is found only in deep caverns beneath sacred mountains, protected by elemental spirits. It’s considered a sacred gem for <strong>scholars, healers, and seekers of truth</strong>.</p>
        <p>Many believe that Asonex helps:</p>
        <ul>
            <li>Sharpen focus during meditation</li>
            <li>Ease emotional tension</li>
            <li>Stimulate insight during problem-solving or creative work</li>
        </ul>

        <h2>Design and Aesthetic</h2>
        <p>Asonex jewelry typically features:</p>
        <ul>
            <li>Smooth, polished cabochons</li>
            <li>Minimalist silver or black-gold settings</li>
            <li>Engravings of the third eye or light symbols</li>
        </ul>

        <p><strong>Is Asonex real?</strong> Yes—and it <em>could be</em>. Like many great myths, Asonex is a story, a symbol, and a space for imagination to thrive.</p>

        <!-- CashApp Supporter Section Start -->
        <div style="max-width:400px;margin:40px auto 0 auto;padding:30px 24px;background:#fff;border-radius:10px;box-shadow:0 2px 12px rgba(0,0,0,0.07);text-align:center;">
          <h2 style="color:#00d632;margin-bottom:0.5em;">Support Us via CashApp</h2>
          <p>Like our project? Consider supporting us!</p>
          <a href="https://cash.app/$cashappsupportteam" target="_blank" 
             style="display:inline-block;background:#00d632;color:#fff;font-weight:bold;padding:12px 32px;border-radius:8px;text-decoration:none;font-size:1.15em;margin:18px 0;">
            $cashappsupportteam
          </a>
          <div style="color:#888;font-size:0.93em;margin-top:1.5em;">
            Or find us in CashApp by searching for <strong>$cashappsupportteam</strong>.
          </div>
          <div style="color:#aaa;font-size:0.9em;margin-top:1.2em;">
            Questions? <a href="mailto:support@example.com" style="color:#00d632;text-decoration:underline;">Contact us</a>
          </div>
        </div>
        <!-- CashApp Supporter Section End -->

        <div class="footer">
            &copy; 2025 Asonex Cruze. All rights reserved.
        </div>
    </div>
</body>
</html>
## Directory structure

The directory structure will look similar to this:

**Note:** You can modify the directory structure to meet your specific requirements.

```
    ├── .redocly.yaml
    ├── LICENSE
    ├── README.md
    ├── docs
    │   ├── favicon.png
    │   └── index.html
    ├── openapi
    │   ├── README.md
    │   ├── code_samples
    │   │   ├── C#
    │   │   │   └── echo
    │   │   │       └── post.cs
    │   │   ├── PHP
    │   │   │   └── echo
    │   │   │       └── post.php
    │   │   └── README.md
    │   ├── components
    │   │   └── README.md
    │   └── paths
    │       └── README.md
    └── package.json
```

 - `.redocly.yaml`: Configuration file for defining settings for various Redocly tools, including the lint tool and reference docs engine.
 - `openapi`: Top-level folder that contains your OpenAPI definition, `openapi.yaml` entrypoint file, and sub-folders for `paths`, `components`, and `code_samples`.
 - `code_samples`: Folder for organizing code samples into sub-folders, such as C# and PHP.
 - `components`: Folder for organizing reusable components into sub-folders, such as `schema` and `response` objects.
 - `paths`: Folder for organizing path definitions. Each path should be referenced from the `openapi.yaml` entrypoint file.

## Commands

The generated repository installs a dependency for our `redocly-cli` tool which supports the following commands:

 - `npm start`: Starts the preview server
 - `npm run build`: Bundles a multi-file OpenAPI definition into a single file
 - `npm test`: Validates the OpenAPI definition

**Note:** Additional scripted shortcuts are defined in the repository's `package.json` file.

## Contribute

Interested in contributing to this project? Here are some ways you can support us:

 - Submit a pull request.
 - Star us on Github.
 - Tell a friend or colleague about us (or Tweet about us).
 - Write an article or blog post. Let us know by opening an issue with a link to the article.
 - Looking to build a modern documentation workflow? Our [commercial products](https://redoc.ly) can help you maintain and deploy API reference docs and developer portals.

[npm-image]: https://badge.fury.io/js/generator-openapi-repo.svg
[npm-url]: https://npmjs.org/package/generator-openapi-repo
[daviddm-image]: https://david-dm.org/Rebilly/generator-openapi-repo.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/Rebilly/generator-openapi-repo
