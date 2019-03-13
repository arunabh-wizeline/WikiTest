---
ReleaseNotes: "First draft of the document."
Author: Arunabh
Date: March 13, 2019
---

# Managing github Wiki Offline

This is a small readme to access the github wiki. There may be alternative methods, but this one works.

**Follow these steps:**

1. [Clone Repository to Local](#clone-repository-to-local)
2. [Create Documentation](#create-documentation)
3. [Publish on github](#publish-on-github)

## Clone Repository to Local

Follow these steps to create a wiki in the repository:

1. Open browser > github.com.
2. Create repository or open repository to add wiki.
   **NOTE**: Wikis are only available for Public repositories. Contact the repository owner to enable wikis if they were disabled during creation.
3. If a wiki does not exist, follow these steps:
  a. Click **Create the first page**.
      The first page called **Home** is created with default text.
  b. Save the page.
4. Copy the link from the **Clone this wiki locally** section.

## Create Documentation

Documentation for github wiki follows these constraints:

- All files are markdown files.
- The name of the file (abc-xyz.md) translates to the page title (Abc Xyx).
- Do not add a title to the markdown document.
- Keep all files (md, png, or others) in the same directory as the home.md file.
- Format for image link: `![Alt Text](./ImageName.png)`

Follow these steps to create the source documentation for the wiki:

1. Open terminal.
2. Navigate to your working directory.
3. Type `git clone <copied link>`. The `<copied link>` is from Step 4 of the [Clone Repository to Local](#clone-repository-to-local) section.
   **NOTE**: The cloned repository includes the Home.md page. This is the default landing page for github wikis.
4. Create your different documents for the wiki in the directory.
5. Add the overview and links to other documents in the `Home.md` document in the following format:

```
  - [Document One](./Document-one)
  - [Document Two](./Document-two)
```

## Publish on github

Follow these steps to publish the wiki to github:

1. Open terminal.
2. Navigate to your working directory.
3. Type `git add .` to add the files to the commit.
4. Type `git commit -m "<commit message here>"` to commit the added files to the repository.
5. Type `git push` to push the files to github.
