# Virtual Store Lab

## Author: Davee Sok / Chris Bortel

### Links and Resources:

<!-- - [ci/cd](http://xyz.com) (GitHub Actions) -->

- [Front-End Application](https://daveesvirtualstorelab.netlify.app/)
- [API used for Products & Categories](https://davee-auth-api-server.herokuapp.com/)
- [Lab36 Pull Request](https://github.com/davee-401-advanced-javascript/storefront/pull/1)
- [Lab37 Pull Request](https://github.com/davee-401-advanced-javascript/storefront/pull/2)

### Tests:

<!-- - How do you run tests?
- Any tests of note?
- Describe any tests that you did not complete, skipped, etc -->

Currently No Tests Written.

### UML:

<!-- Link to an image of the UML for your application and response to events -->

```
Pseduo Code


// Redux Store will have the following Reducers
    Categories
      States
        - activeCategory
        - category list
      Actions
        - initializeCategory

    Products
      States
        - products list
      Actions
        - initalizeProducts

    Carts
      States
        - cart
      Actions
        - addToCart
        - deleteFromCart


<App>
// Will need to get API Data and intialize
    Actions:
      - initalizeCategory
      - intializeProducts

  <Header/>
    States:
      - cart

  <SimpleCart/>
  // Will list out all the carts
    States:
      - cart
    Actions:
      - deleteFromCart

  <StoreFront>

    <Categories/>
      // Will list out all categories
          States:
            - categories
          Actions:
            - changeCategory

    <CurrentCategories/>
      // Will render active category
          States:
            - activeCategory
          Actions:
            - None

    <Products/>
      // Will filter list based on active category
          States:
            - activeCategory
            - products
          Actions
            - addToCart

    </StoreFront>
  <Footer/>
</App>


```
