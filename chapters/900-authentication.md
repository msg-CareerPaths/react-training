# 8. Authentication [3-4 hours]

**Goal:**
- Get familiar with Protected Routes
- Protect your app routes from unauthorized access.

## Mandatory Materials

**Videos**
- [React Router: Authentication and Protected Routes](https://youtu.be/X8eAbu1RWZ4)

**Reading**
- [Authentication React Router v6](https://blog.logrocket.com/authentication-react-router-v6/) (suggested)

### Notes from the Mock Backend
- It uses JWT for authentication.
- Only the authentication module paths are secured.
    - `http://localhost:3000/api/auth/profile` needs a JWT token in the request headers for it to work.
    - The other API paths are not secured.
- Check `src/assets/users.json` for more information regarding already available users.

## Online Shop:

> Create a new login view, containing a text input for the username, a password input for the password and a login button.
>
> Add somewhere in your application information about the current logged-in user (for Mock API call `/api/auth/profile`).
>
> Also add a logout button, which when called, removes the token from the localstorage and redirects the user to the login page.
>
> Automatically redirect the user to the login view each time you receive a 401 response on a request. When pressing the login button, send an appropriate request to the backend. If the request succeeds, redirect the user to the product page, otherwise display an error message.
>
> Use the roles returned by the backend to disable the edit, create and delete buttons if the user is not an administrator. Only allow customers to view the shopping cart and to add products in it.
