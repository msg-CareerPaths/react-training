# React Training Introduction

## Description
First, I would like to start by emphasizing with reader that the following read is quite verbose, but I would like to ask that you read the following carefully.

This is a roadmap/training for an introduction into the React Library consisting of several steps.
In each step, a set of theoretical concepts are explored, supported by reference documentation, book chapters, tutorials and videos.

In parallel, a simple application will be built with the learned concepts: the *Online Shop* application.
After the learning material for a given step was sufficiently explored either some new functionality will be added to this application or old functionality will be refactored.

## Working Mode

All the code written must be published on GitHub.

- Create your own repository on your personal account and give access to your mentor (make sure you specify your name in case you have an esoteric username).
- Commits must be pushed when each individual chapter is finished.
- [Create](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository) a `develop` branch from the `master` branch **before starting work**.
- **In order to request a code review from the mentors**, you must [open a pull request](https://help.github.com/en/articles/creating-a-pull-request) from the `develop` to the `master` branch. Inform them in your **daily standup** of this or through a PM.
- **Once the Pull Request is approved** by the mentors, merge it into `main` and create another branch from master to continue work.
- Take care to delete your `develop` branch then, go back inside your IDE to `main` and update it (git pull)
- Carry on your work by creating another `develop` branch and working on it
- Repeat ad infinitum (until the training has ended)

## Environment Setup

On your local machine install the following:
- You need to install [NodeJS](https://nodejs.org/en/) (recommended for most user version, 18.16.0 at moment of writing)
- You will need an IDE (Integrated Development Environment) so you can code
    - [VSCode](https://code.visualstudio.com/download)
    - [Webstorm](https://www.jetbrains.com/webstorm/) as an alternative to VSCode. Note if you are still a student you can use your student license on it, otherwise you can use the 30 days trial.
- You need to have [Git](https://git-scm.com) installed on your computer.
- Have also [Notepad++](https://notepad-plus-plus.org/downloads/) for a nicer basic file editing experience

## Online Shop

We will create a very basic online shop to showcase the functionalities of the React library.
The application will simply browse through a catalog of products. It will support the following functional requirements:
- Listing the products,
- Adding a new product,
- Updating an existing product,
- Deleting a product.

The online shop has a "shopping cart" functionality:
- The user may add items into the cart,
- He may increment and decrement the quantity of each product or even remove a product completely from the cart,
- Lastly, he can check out the cart and place an order (resulting in the creation of an order in the backend).

### Mock Backend
A mock backend alongside the instruction for starting it can be found [here](https://github.com/msg-CareerPaths/mock-backend).

### UI Design
Mockups describing the user interface structure can be found in the [**mockups**](https://github.com/msg-CareerPaths/react-training/tree/master/mockups) folder.
These mockups should be used as a guideline, but improvements or deviations from them is allowed.

## Notes
- If you find any link broken, **please** inform your mentor to give you an alternative.
- Try to speed up the videos to *1.5x/2x* if you find them too slow.
- Try to connect to the Backend from the Spring Training if you have training completed (you might need to change the port for your requests)

## Timeline
This timeline is just for guidance, take time to understand the concepts before moving on.

- **Day 1**: Chapter 0, Chapter 1, Chapter 2, Chapter 3
- **Day 2**: Chapter 4, Chapter 5
- **Day 3**: Chapter 5,
- **Day 4**: Chapter 6, Chapter 7, **Open a Pull Request**, Fix Review Remarks => Merge to Master => Create a new branch
- **Day 5**: Chapter 8
- **Day 6**: Chapter 9, Chapter 10
- **Day 7**: Chapter 10, **Open a Pull Request**, Fix Review Remarks => Merge to Master => Create a new branch
- **Day 8**: Chapter 11, Optional Chapters or Fix Review Remarks/Refactor Code

## ZScaler Issues (OPTIONAL - only when needed)

You might encounter ZScaler issues due to company bureaucracy. ZScaler is proxy that scan and routes the internet traffic of your device, blocking you from accesing certain internet endpoints.
Thus, if you encounter `SSL CERTIFICATE ERRORS`, `UNABLE TO GET LOCAL ISSUER CERTIFICATE` or simply connection issue this **may** point you to a ZScaler problem.

First steps:
- Download the certificate offered by the company
- Save the certificate in C:\zscaler.crt

### Webstorm Issues
- Go to File\Settings in your IDE
- Search for `Proxy` in the search bar
- Turn on the `Auto-detect proxy settings`
- Search for `Server Certificates`
- Press the `plus` icon in the Accepted Certificates tables and add the Zscaler certificate

### Git Issues
- Go to `C:\Users\<your_username>\AppData\Local\Programs\Git\mingw64\ssl\certs` and open `ca-bundle.crt` in Notepad
- Open in a parallel notepad instance the `zscaler.crt`
- **Copy** the content from `zscaler.crt` to the bottom of the `ca-bundle.crt` file (leave an empty space between)
- You can make `Git` trust the Windows certificate store by running in a terminal instance `git config --global http.sslBackend schannel`

### Node.js Issues
- Open windows search bar and type `environment`
- Select `Edit environment variables...` and select `Environment Variables` from the new window
- In User variables add a new one with the name `NODE_EXTRA_CA_CERTS` and the value being the `path to your saved certificate` (C:\zscaler.crt)
- Restart your computer