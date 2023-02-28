## Working Mode

The road-map consists of several steps. In each step, a set of theoretical concepts are explored, supported by reference documentation, book chapters, tutorials and videos. In parallel, a simple application will be built with the learned concepts: the **Online Shop** application.

After the learning material for a given step was sufficiently explored, either some new functionality will be added to this application or old functionality will be refactored.

All the code written must be published on GitHub. Commits must be pushed when each individual chapter is finished. In order to request a code review from the trainers, you must [**open a pull request**](https://help.github.com/en/articles/creating-a-pull-request) from the `develop` to the `master` branch.

## Environment

You can work using your local environment:

- You need to install [**NodeJS**](https://nodejs.org/en/) and [**VSCode**](https://code.visualstudio.com/download)
- **If you have finished the Spring Boot training** you can use that backend application together with the frontend one you will develop during this training. If not, you can use our [**Mocked Backend Application**](https://github.com/msg-CareerPaths/mock-backend)
- Fork the starting codebase from [**here**](https://github.com/msg-CareerPaths/react-training) to your own GitHub account

## Online Shop

The application will simply **browse through a catalog of products**. It will support:

- Listing the products,
- Adding a new product,
- Updating an existing product,
- Deleting a product.

The online shop has a **shopping cart** functionality:

- The user may add items into the cart,
- He may increment and decrement the quantity of each product or even remove a product completely from the cart,
- Lastly, he may checkout the cart and place an order (resulting in the creation of an order in the backend).

**Mockups** describing the user interface structure can be found in the [**mockups**](https://github.com/msg-CareerPaths/react-training/tree/master/mockups) folder.
These **mockups should be used as a guideline**, but improvements or deviations from them is allowed.
**We support custom styling** in order to make the application your own.
