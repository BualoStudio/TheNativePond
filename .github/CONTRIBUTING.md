# Contributing Guide

Hello! Thank you for your interest in contributing to _The Native Pond_. This guide will help you get started.

## 0. 📖 Prerequisites

Before you start contributing, please make sure you have:

- Read this project's [README](https://github.com/BualoStudio/TheNativePond/edit/main/README.md) to get a general understanding of the project.
- Carefully read and comply with the [LICENSE](https://github.com/BualoStudio/TheNativePond/blob/main/LICENSE).
- Carefully read and comply with the [Code of Conduct](https://github.com/BualoStudio/TheNativePond/blob/main/.github/CODE_OF_CONDUCT.md).
- Read the [TheNativePond FlatbreadList](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/FlatbreadList.md) file.
- Read the [TheNativePond Values](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/Values-en.md) file, and do not contribute content that goes against the values.
- Have the TurboWarp editor ready: [TurboWarp Desktop](https://desktop.turbowarp.org/) (recommended) or [TurboWarp Webapp](https://turbowarp.org/editor).
- Search existing [Issues](https://github.com/BualoStudio/TheNativePond/issues) and [Pull Requests](https://github.com/BualoStudio/TheNativePond/pulls) to avoid duplicate work.

## 1. 🛠️ Fork this repository

1. Click the **Fork** button in the upper-right corner of the [TheNativePond](https://github.com/BualoStudio/TheNativePond) page.
2. Modify any basic information if needed, then click the **Create fork** button below.

## 2. 📂 Choose your contribution area

Since _The Native Pond_ is a multimedia game project, you only need to choose the area you wish to contribute to.

<details>

<summary>💻 Code</summary>

### 💻 Code

#### TurboWarp project files (.sb3)

> [!WARNING]
> Because TurboWarp project files are binary files and not suitable for code review, please do not submit Pull Requests directly against project files. Generally, we do not accept Pull Requests for project files.

If you absolutely need to modify a project file, please:

- Submit an Issue containing a complete modification proposal
- Or design a corresponding JavaScript custom extension
- Or [contact us](mailto:thenativepond@gmail.com)

If we consider your request reasonable and necessary, we may invite you to collaboratively modify the project file.

##### We do not accept:

- Pull Requests against project files submitted without prior discussion
- Modifications to Scratch Blocks
- Modifications to the TurboWarp kernel
- Large-scale refactoring submitted without prior discussion

#### Custom extensions (.js)

Because TurboWarp's built‑in functionality is somewhat limited for _The Native Pond_'s development needs, we use custom extensions to supplement missing features.

##### Accepted contributions:

- Custom extensions that introduce new functionality
- Bug fixes for existing custom extensions
- Performance optimisations for existing custom extensions
- API improvements for existing custom extensions
- Comment improvements and documentation supplements for existing custom extensions

##### We do not accept:

- Modifications to Scratch Blocks
- Modifications to the TurboWarp kernel
- Large-scale refactoring submitted without prior discussion

##### When writing JavaScript custom extensions, please:

- Use modern JavaScript
- Maintain code readability and consistent style
- Use meaningful variable names (follow the [Naming Conventions](https://github.com/BualoStudio/Icelet/wiki/Naming-Conventions))
- Avoid code duplication
- Add necessary comments
- Remove debugging code
- Do not submit minified code

##### Before submitting your contribution, please double‑check that:

- It runs correctly
- There are no console errors
- It does not affect other extensions
- Basic testing has been completed

</details>

<details>

<summary>🖌️ Art assets</summary>

### 🖌️ Art assets

> [!NOTE]
> We strongly recommend using **SVG** format for art assets. Except for illustrations, we do not accept Pull Requests in other image formats. Only in very special cases should .png, .jpg, .webp, or other image formats be used.

##### Accepted contributions:

- UI icons
- Game maps
- Item textures
- Illustrations (note: illustrations may use other image formats)
- Other vector assets

##### When contributing art assets, please:

- Use SVG vector graphics (except for illustrations)
- Ensure the asset is editable
- Minimise the number of nodes
- Follow the [Naming Conventions](https://github.com/BualoStudio/TheNativePond/wiki/Naming-Conventions)
- Maintain a consistent design style (see [TheNativePond Art Design Guidelines]())

</details>

<details>

<summary>🪗 Music & sound assets</summary>

### 🪗 Music & sound assets

> [!NOTE]
> For music and sound assets, we do not enforce a specific file format, but the file format should be one of the following: .mp3, .m4a, .ogg, .wav.

##### Accepted contributions:

- Background music
- UI (interaction) sound effects
- Notification sounds
- Ambient sounds

##### When contributing music & sound assets, please:

- Keep volume moderate (consistent with other audio files)
- Avoid clipping as much as possible
- Ensure you own the copyright to the asset, or confirm it is in the public domain, or that it can be released under the open‑source license used by this project for music assets.
- Ensure you have obtained the asset from a legitimate source

</details>

<details>

<summary>🌐 Localisation</summary>

### 🌐 Localisation

We are looking for people who can help translate _The Native Pond_ into languages other than Simplified Chinese. If you are interested, please read on.

##### Requirements for becoming a translator:

- You must be **proficient** in Simplified Chinese.
- For example, if you can understand Simplified Chinese videos on Bilibili without assistance, your Simplified Chinese level is high. If you need a translation tool to understand sentences, your level is not high enough.
- You must be a native speaker of the **target** language. (If you are not a native speaker but believe you are fluent enough, you may also apply. Please keep in mind that taking some language courses does not make you fluent. If you would not set your smartphone's system language to the target language, then your level is not sufficient!)

##### Accepted contributions:

- Support for new languages
- Corrections to errors in existing languages

##### When contributing localisation translations, please:

- Use consistent terminology
- Do not submit machine‑translated text directly
- Keep punctuation consistent
- Do not change variable names

##### Contribution steps:

1. Locate the language file (in the `/lang/` directory).
2. In the language file, you will see lines formatted like `"information"="I love you!",`.
3. Only modify the text inside the quotation marks on the right side of the equals sign.
4. Repeat step 3 until you have translated all lines.

</details>

<details>

<summary>💡 Other</summary>

### 💡 Other

Have another way you'd like to contribute? If so, please [contact us](mailto:thenativepond@gmail.com) to discuss your contribution.

</details>

## 3. 📡 Submit

As usual, commit your contributions to your forked repository. Different contribution areas correspond to different file locations:

.  
├── extensions/          JavaScript custom extensions  
├── assets/  
│   ├── images/          Images  
│   ├── sounds/          Audio  
│   └── fonts/           Fonts  
├── lang/                Localisation translations  
├── docs/                Documentation  
├── LICENSE  
└── README.md  

Place your contributions in the appropriate folder.

## 4. 🔗 Create a Pull Request

Navigate to the [TheNativePond](https://github.com/BualoStudio/TheNativePond) page, click the **Pull requests** tab, then click the **New pull request** button. Click the **Compare across forks** link and select your fork repository.

Review the changes, then click the **Create pull request** button.

## 5. 🎉 Wow! You did it!

Congratulations! You have completed your contribution to this project. Now you can wait for us to review your pull request.
