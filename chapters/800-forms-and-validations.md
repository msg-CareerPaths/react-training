# 8. Forms and Validations [4-6 hours]

**Goal:**
- Dive in how to manage forms in React
- Create forms to create and update products

## Mandatory Materials

**Videos**
- [React Hook Form Tutorial](https://youtu.be/RkXv4AXXC_4)
- [React Hook Form with Zod](https://youtu.be/cc_xmawJ8Kg)

**Reading**
- [React Hook Form: Quickstart](https://www.react-hook-form.com/get-started#Quickstart)
- [Zod Basic Usage](https://zod.dev/?id=basic-usage)
- [React Hook Form: Validations using Zod](https://dev.to/majiedo/using-zod-with-react-hook-form-using-typescript-1mgk)
- [Container vs Presentational Components in React](https://medium.com/@yassimortensen/container-vs-presentational-components-in-react-8eea956e1cea)


## Online Shop

Recall that the logic should be added to the `container` components and the presentational part in his named counterpart.
>
> Install React Hook Form library and Zod validations by running `npm install react-hook-form zod @hookform/resolvers`
> 
> Add a new "Edit" button on the detail page. Pressing it should open a new view, which uses reactive forms to update the properties of the product. 
> 
> The view should have two buttons: "Cancel" (which undo's all the changes) and "Save" (which calls the backend to persist the changes).
>
> Add some validation to your form (ex: check that the fields are not empty, that the price and weight inputs contain only numbers, etc.)
>
> Also create a new "Add" button on the product list. Pressing this button should open a view for creating a new product (which has the same structure and buttons as the edit view).

## Further Resources

- [React Hook Form: Code Examples](https://github.com/react-hook-form/react-hook-form/tree/master/examples)
