https://stackblitz.com/angular/odpeknvxnlq?file=src%2Fapp%2Fcart%2Fcart.component.html


`
*ngFor is a "structural directive". Structural directives shape or reshape the DOM's structure, typically by adding, removing, and manipulating the elements to which they are attached. Directives with an asterisk, *, are structural directives.
`

Topics Studies so far:
1. *ngFor
2. *ngIf
3. Interpolation {{ }}
4. Property binding [ ]
5. Event binding ( )

### `Components`
Components define areas of responsibility in the user interface, or UI, that let you reuse sets of UI functionality. You've already built one with the product list component.

A component consists of three things:

  1. **A component class** that handles data and functionality. In the previous section, the product data and the share() method in the component class handle data and functionality, respectively.
  2. **An HTML template** that determines the UI. In the previous section, the product list's HTML template displays the name, description, and a "Share" button for each product.
  3. **Component-specific** styles that define the look and feel. Though product list does not define any styles, this is where component CSS resides.

An Angular application comprises a tree of components, in which each Angular component has a specific purpose and responsibility.

### `Angular Router`

The Angular Router enables you to show different components and data to the user based on where the user is in the application. The router enables navigation from one view to the next as users perform tasks such as the following:

1. Entering a URL in the address bar to navigate to a corresponding page.
2. Clicking links on the page to navigate to a new page.
3. Clicking the browser's back and forward buttons to navigate backward and forward through the browser history.

### `Services`

Services are an integral part of Angular applications. In Angular, a service is an instance of a class that you can make available to any part of your application using Angular's dependency injection system.

Services are the place where you share data between parts of your application. For the online store, the cart service is where you store your cart data and methods.

### `Pipes`
The line, <h4>{{ product.price | currency }}</h4> uses the currency pipe to transform product.price from a number to a currency string. A pipe is a way you can transform data in your HTML template. For more information about Angular pipes, see Pipes.

### `HttpClientModule`
Angular's HttpClientModule registers the providers your app needs to use a single instance of the HttpClient service throughout your app.

### `Forms in Angular`
Forms in Angular build upon the standard HTML forms to help you create custom form controls and easy validation experiences. There are two parts to an Angular Reactive form: the objects that live in the component to store and manage the form, and the visualization of the form that lives in the template.
* Angular's FormBuilder service provides convenient methods for generating controls. As with the other services you've used, you need to import and inject the service before you can use it:
* The ReactiveFormsModule provides the FormBuilder service, which AppModule (in app.module.ts) already imports.
* To gather the user's name and address, set the checkoutForm property with a form model containing name and address fields, using the FormBuilder group() method. Add this between the curly braces, {}, of the constructor.