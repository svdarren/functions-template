# Netlify Functions template
This template is a personal reuse starting point for Netlify functions.  This is general, but assumes the function will be used as part of a JAMstack project or environment.

* [JAMstack WTF](https://jamstack.wtf) Starting explanation of JAMstack.
* [The JAMstack: It’s Pretty Sweet](https://medium.com/memory-leak/the-jamstack-its-pretty-sweet-e0834e4e6bb7) - good article describing the progression to JAMstack and it's ecosystem.
![JAMstack](https://assortment.io/uploads/assortment-moves-to-jamstack/jamstack-definitions.png)

# Toolchain Summary
1. First, there needs to be repository.  Our environment needs this to exist first, and this template project can be cloned to start.
2. Next, we need our development environment.  GitPod launches from the repo in GitHub.
3. GitPod starts up with the required developer tools and dependencies based on the files in this project's repo.  RPM, the package manager, is called by GitPod to install everything before we start.
4. Last, when we save edits and check into GitHub, the edits are auto deployed to Netlify for hosting.

***


# ![GitHub](https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/GitHub_logo_2013.svg/200px-GitHub_logo_2013.svg.png)

GitHub is a cloud repository based on Git and coding platform.

### GitHub repo
### GitHub Pages
* [GitHub Pages](https://pages.github.com/) - Pages is a web hosting option based on Jeykll.  It can be as simple as a README.md.  This is an alternative to hosting with Netlify.
### GitHub Actions
Actions provide workflow automation within GitHub.  Actions does not currently expose and HTTP address, so not a good option to trigger from a Webhook.
* [GitHub Actions now supports CI/CD](https://github.blog/2019-08-08-github-actions-now-supports-ci-cd/) - blog post announcing CI support for Actions.

# ![GitPod](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Gitpod-ddd.svg/200px-Gitpod-ddd.svg.png)

* [Gitpodifying — The Ultimate Guide](https://www.gitpod.io/blog/gitpodify/) - good startup guide on how to setup the GitPod environment in .gitpod.yml.
* [What should go in the yml vs dockerfile?](https://spectrum.chat/gitpod/general/how-to-save-loadtime-with-npm-installs-overlap-between-gitpod-yml-and-dockerfile~c2d31366-b6c4-4f9b-9181-eabe5288b6cf?m=MTU3MzcxNDczOTEyNA==) - Comments from GitPod team in this thread.
* [GitPod Docs](https://www.gitpod.io/docs/) - official documentation
* [Awesome Online IDE](https://ide.ceriously.com/) - List of Cloud based IDEs, like GitPod.


# ![NPM - Node Package Manager](https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Npm-logo.svg/200px-Npm-logo.svg.png)

* [No need for globals — using npm dependencies in npm scripts](https://firstdoit.com/no-need-for-globals-using-npm-dependencies-in-npm-scripts-3dfb478908) - This Medium article does a good job explaining what is a devDependancy and what is not.  Also shows how to make simple command line commands for common tasks.
* [Learning npm the Node Package Manager](https://www.linkedin.com/learning/learning-npm-the-node-package-manager-3):heavy_dollar_sign: - LinkedIn Learning course
* [NPM Style Guide](https://github.com/voorhoede/npm-style-guide) - general style guidance
* [NPM Standard Script Names](https://github.com/voorhoede/npm-style-guide#use-standard-script-names) - common names for NPM script sections


# ![Netlify](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b8/Netlify_logo.svg/200px-Netlify_logo.svg.png)
### Setup
* [Snippets help doc](https://docs.netlify.com/site-deploys/post-processing/snippet-injection/) - Snippet Injection is for adding a section of code to all served files.  This is for analytics, tracking, etc.
### Functions
* [Building Serverless CRUD apps with Netlify Functions & FaunaDB](https://www.netlify.com/blog/2018/07/09/building-serverless-crud-apps-with-netlify-functions-faunadb/) - Good example on initial Lambda function setup.
* [Build serverless functions with JavaScript](https://docs.netlify.com/functions/build-with-javascript/) - Official docs page describing how to build lambda functions with JavaScript.  Explicitly states the URL for triggering the function remotely.
### Tools
* [netlify-cli](https://github.com/netlify/cli) - GitHub repo for CLI tools.
* [netlify-lambda](https://github.com/netlify/netlify-lambda) - GitHub repo for optional netlify-lambda tools.
* [Netlify CLI Command List](https://cli.netlify.com/) - instructions for the CLI tools.
* [Netlify Dev](https://github.com/netlify/cli/blob/master/docs/netlify-dev.md) - part of the CLI package, this explains the Netlify Dev command.


# REST APIs, Webhooks, and Workflow Automation
### Tools
* [Webhook.site](https://webhook.site/) - Helper site for Webhook callbacks
* [API Tester](https://www.apitester.com/) - Helper site for testing HTTP calls
* [Zapier](https://zapier.com/) - A GUI-driven service for building simple workflows.  Can create automations without code, but without any middleware code options.
### APIs
* [GitHub Webhooks](https://developer.github.com/webhooks/) - Get trigger events from GitHub to other apps.
* [Eventbrite Webhooks](https://www.eventbrite.com/platform/docs/webhooks) - Events from Eventbrite ticking service.
