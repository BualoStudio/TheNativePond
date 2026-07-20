# CONTRIBUTING

Hello! Thank you for your interest in contributing to _TheNativePond_. This guide will help you get started.

## 0. Prerequisites

- [TurboWarp Webapp](turbowarp.org/editor) or [TurboWarp Desktop](https://desktop.turbowarp.org/)

<details>
<summary>If you have already contributed to this project before</summary>

### If you have already contributed to this project before

> [!WARNING]
>
> If you haven't cloned this repository, skip this section.

Make sure your local repository is up to date with the upstream repository:

```shell
git fetch --all
git checkout main
git pull upstream main --rebase
```

If you have a working branch, to make your branch up to date with the upstream repository:

```shell
git checkout <your-branch-name>
git rebase main
```

</details>

## 1. Fork this project

Click on the **Fork** button on the top right corner of the [TheNativePond](https://github.com/BualoStudio/TheNativePond) page.

## 3. Clone

```shell
git clone https://github.com/<your-github-username>/tnp.git
cd tnp
```

## 2. Create your working branch

```shell
git checkout -b <your-branch-name>
```

## 3. Install dependencies

```shell
corepack enable
pnpm install

# For Rust dependencies
# Not required if you are not going to develop on either crates or apps/tamagotchi
cargo fetch
```

> [!NOTE]
>
> We would recommend to install [@antfu/ni](https://github.com/antfu-collective/ni) to make your script simpler.
>
> ```shell
> corepack enable
> npm i -g @antfu/ni
> ```
>
> Once installed, you can
>
> - use `ni` for `pnpm install`, `npm install` and `yarn install`.
> - use `nr` for `pnpm run`, `npm run` and `yarn run`.
>
> You don't need to care about the package manager, `ni` will help you choose the right one.

## Choose the application you want to develop on

## 🌐 Localization

We hope _The Native Pond_ can be experienced by players all over the world. If you want to help translate the game into your language:

1. Fork this repository.
2. Find the language files (in the `/lang/` directory).
3. Add or update translations.
4. Submit a [Pull Request](https://github.com/BualoStudio/TheNativePond/pulls).

## 🤝 Join the Co-construction

_The Native Pond_ is not just our work; we hope it can become a "spiritual gas station" for all weary players. Whether you know about game development or code or not, you can contribute to this little pond!

We highly welcome Issues in the following forms:

### 1. 💡 New Content Suggestions

> [!IMPORTANT]
> 
> Before submitting suggestions for new content, please read our ["Flatbread List"](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/FlatbreadList.md) and ["Values"](https://github.com/BualoStudio/TheNativePond/blob/main/docs/game/Values.md) first!

1. **Memory Fragment Delivery**: Write a touching copy for the game, or share a nostalgic short essay with a sense of the era.
2. **Hometown Recipe Contribution**: Design a brand new recipe (e.g., how to make an authentic bowl of Hot Dry Noodles) and break down its preparation steps.

> [!TIP]
> 
> Want to make excellent derivative modifications or MODs for _The Native Pond_? Please refer to _[The Native Pond Technical Documentation](https://www.google.com/search?q=)_ and _[Icelet Development Guide](https://github.com/BualoStudio/Icelet/wiki), and comply with the [LICENSE](https://github.com/BualoStudio/TheNativePond/blob/main/LICENSE) file when distributing.

### 2. 🐛 Existing Issues

1. Report problems, bugs, and errors triggered by the game under specific circumstances.
2. Provide solutions to currently existing problems, bugs, and errors.

> [!NOTE]
> 
> Due to TurboWarp's single source file limitation, please do not submit Pull Requests directly to the source file. However, you can submit bugs to [Issue](https://github.com/BualoStudio/TheNativePond/issues).

## Commit

### Before commit

Please make sure lint (static checkers) and TypeScript compilers are satisfied:

```shell
pnpm lint && pnpm typecheck
```

If you are committing images, consider using AVIF format instead of PNG, JPG etc. You can convert existing images to AVIF by running:

```shell
pnpm to-avif <PATH_TO_IMAGE_OR_DIRECTORY1> <PATH_2> <PATH_3> ...
```

> [!NOTE]
>
> If you have [@antfu/ni](https://github.com/antfu-collective/ni) installed, you can use `nr` to run the commands:
>
> ```shell
> nr lint && nr typecheck
> ```

### Commit

```shell
git add .
git commit -m "<your-commit-message>"
```

### Push to your fork repository

```shell
git push origin <your-branch-name> -u
```

You should be able to browse the branch on your fork repository.

> [!NOTE]
>
> If this is your first time contributing to this project, you need to add the upstream repository too:
>
> ```shell
> git remote add upstream https://github.com/moeru-ai/airi.git
> ```

## Creating Pull Request

Navigate to [TheNativePond](https://github.com/BualoStudio/TheNativePond) page, click on the **Pull requests** tab, and click on the **New pull request** button, click on the **Compare across forks** link, and select your fork repository.

Review the changes, and click on the **Create pull request** button.

## Whooo-ya! You made it!

Congratulations! You made your first contribution to this project. You can now wait for the maintainers to review your pull request.
