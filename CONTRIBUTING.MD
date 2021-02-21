# Contributing to MONK

we are really excited that you are interested in contributing to MONK!

The following guidelines should assure seamless and qualitative integration of your future contributions to the MONK ecosystem. 

Contributions thereby may include but are not limited to the integration of 3rd-party modules to the <a href="https://github.com/dicama/monk-modules">MONK Modulestore</a> (via PRs),
developments for our <a href="https://github.com/dicama/monk-app">MONK-App</a> and involved packages (via PRs),
bug fixing, beeing an excellent community member and help filing issues either for <a href="https://github.com/dicama/monk-app/issues">MONK-App</a>/<a href="https://github.com/dicama/monk-modules/issues">MONK-Modules</a> or providing valuable feedback in any sense. Before filing an issue always check the corresponding issue-tracker for potential duplicates.  

Community members who gained our trust and demonstrated strong commitment may be granted with commit access and join the MONK core team in the future. 

Most importantly as stated in our code of conduct: "Be excellent to each other"


## Contributing with MONK-modules:

Before starting to `#hackaway` with your module, we recommend to get in touch with our MONK audit team first either by filing an issue on
<a href="https://github.com/dicama/monk-modules/issues">MONK-Modules</a> or via mail. Thereby, we know what you are up to
and could provide you valuable first feedback from our expert community as well as potential users. 

The following figure highlights our core-workflow to integrate your contribution within the MONK-Modulestore

<img src="https://github.com/dicama/dicama/blob/dicama-imgs-1/module_contribution.svg" width="800">

### (1) Create a Pull Request (PR)
All PRs to the modulestore require peer-review by the MONK audit team to ensure 

* `Operability`
* `Security`
* `Usability`
* `Integrity`

Therefore, the audit team evaluates in two phases your module contribution in order to ensure that all key requirements for integration are met. 

#### Before filing a PR please check the following `prerequisites`:

- Ensure that your module is designed to build against the current stable release of the <a href="https://github.com/dicama/monk-app">MONK-App</a> as well as Flutter SDK.
- Verify dartanalyzer in <a href="https://github.com/dicama/monk-app">MONK-App</a> isn't throwing any warning or errors while your module is running or integrated
- Ensure your modules follow the app spec
- Ensure your code is properly formatted 
- Avoid adding an onerous amount of blobs to the repo

This saves valuable time for both sides as this could otherwise lead to a direct rejection followed by a potential re-submission. While the prerequisites above must be satisfied prior to having your pull request reviewed by our audit team, reviewers may ask you to complete additional tests in order to ensure operability.

In case you are facing issues, please reach out to the community and <a href="https://github.com/dicama/monk-modules/issues">file an issue</a>. Avoid situations in which you spend a lot of time hacking while not getting the feedback you might deserve in the first place.

After filing your PR our audit team will evaluate contributions in two phases. Wherein phase 1 technical aspects (code reviews & security tests) will be performed while in phase 2 your module will undergo a closed user-test (also see the following table).

(2-a) Audit | (2-b) Audit
------------ | -------------
:black_square_button: `Operability`of the module within MONK App|:black_square_button: `Integrity` within the ecosystem and interoperability 
:black_square_button: `Security` and potential vulnerability issues  |:black_square_button: `Usability`aspects as well as user tests


After finishing each of these tests, our audit team will get back to you with feedback to your contribution as well as user inputs. In case our audit team labels your module with a green checkmark :white_check_mark:, your module will be pushed to <a href="https://github.com/dicama/monk-modules/issues">MONK-Modules Master</a> and available for users in the Modulestore of MONK. 

## Contributing to the MONK-App

We are looking forward to see any contribution to the MONK ecosystem App via PRs. As the integral part of our modular framework is located within the development of the MONK App, we recommend contributors to contact our technical core team beforehand any major developments. This should ensure the integraty and consitance of the work, since you may need to get familiar with our current technical roadmap and processes involved (i.e. tree hygiene) to avoid common pitfalls. Getting in touch early on might be also a opportunity for us to involve you within the team and build a direct communication pipeline from the get-go. Nevertheless, we always try our best to keep you up-to-date about our future pipelines and roadmaps on GitHub. 

Similar to the process for contributions to MONK-Modules, 

Before submitting a pull request, please make sure the following is done.

1. Either fork the <a href="https://github.com/dicama/monk-app">MONK-App Repository</a> and create your branch from master or clone the repository with the 'git clone' command

```git
git clone git@github.com:dicama/monk.git
```

2. Install IDEs: Download either Android Studio/IntelliJ Idea or Visual Studio Code, with the respective [Flutter editor plugins](https://flutter.dev/docs/get-started/editor). For more information about the installation procedure of Flutter, we refer to the Single Source of Truth by checking the [official install guide](https://flutter.dev/docs/get-started/install) as well as the [official documentation](https://flutter.dev/docs).

3. Install all dependencies from pubspec.yaml by running `flutter packages get` from the project root (see [using packages documentation](https://flutter.dev/docs/development/packages-and-plugins/using-packages#adding-a-package-dependency-to-an-app)). Pubspec.yaml thereby manages all assets and dependencies for
MONK. 

### Create a Pull Request (PR) for the MONK Ecosystem App
All PRs require peer-review by the MONK audit team to ensure 

* `Operability`
* `Security`
* `Usability`
* `Integrity`

#### Before filing a PR please check the following `prerequisites`:

- Ensure that the app is designed to build against the current stable version of Flutter SDK.
- Verify dartanalyzer isn't throwing any warning or errors
- Ensure your modules follow the app spec
- Ensure your code is properly formatted 
- Avoid adding an onerous amount of blobs to the repo

Our dev team will get in touch with you upon your PR is filled. 


## Fork your own Digital Cancer Management App

We are also looking forward to own cross-platform applications build on the MONK app framework!

In case you plan to create your own app, feel free to get in touch with us and discuss your ideas. We and the community around MONK are eager to help you with feedback
and potential co-creation developments. 

#### If you build your own App, make sure to
- Replace all graphical assets attached to MONK with your own (Splashscreens, Heroimages etc.)
- Replace direct textual or legal content (i.e. data privacy statements) 
- Exclude the MONK Modulestore from your App

> Note: If you plan to use MONK Modules, please get in touch with us to discuss incopoeration of specific modules and dependencies. Please note, that we would also have to inform 3rd party module providers about a potential incoperation.
> 

## Submitting a "good" bug report?

Bugs in MONK are tracked as Issues within <a href="https://github.com/dicama/monk-app/issues">MONK-App Issue Tracker</a>/<a href="https://github.com/dicama/monk-modules/issues">MONK-Modules Issue Tracker</a>.  

By filing an issue please always try to describe the problem in all details possibile for you. The following template strucutre may help you and 
our dev team to reproduce and solve the corresponding issues. 

* **Use a clear, comprehensive and descriptive title** for the problems addressed.
* **Describe the exact steps leading to the issue** - despite mentioning the workflow about 'What you did' also mention the 'How'. I.e. navigating with gestures, button clicks, inputs you provided
* **Describe the resulting behavior of the app** 
* **Explain which behavior you expected to see**
* **Include attachments like screenshots or videos if possible** 
* **Include details about your mobile device** like OS version, screensize


And now we are looking forward to your contributions!
