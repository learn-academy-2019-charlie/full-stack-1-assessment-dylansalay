# Full Stack 1 Assessment

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. What is Enzyme and what are some of the methods that it provides?
        Enzyme is a testing utility designed specifically to assert, manipulate and traverse a React Component's output. We can pair Enzyme with Jest, or another test runner, to test React applications.
        
        Some of the methods that Enzyme provides to us include simulate, find, contains, context and equals.
        
#### 2. What is the difference between dynamic and a static routes?
        Static routes allow us to map different components to different views, or pages of content. With static routing, we are declaring our routes as part of our apps initialization, before any rendering takes place. With dynamic routes, the routing occurs as the route is rendering. 

#### 3. What is a JSON API?
        A JSON API is an API that receives JSON requests and responds to those requests encoded in JSON format. By communicating in JSON instead of HTML/CSS/Javascript, we won't clutter the app up with support for all of those file types.
        
#### 4. What is a migration and why would you use one?
        A migration allows us to alter, or create a new version of, our database. Each time we run a migration, we create a new migration file and modify our schema.rb file by adding or deleting tables, entries, rows or columns.

#### 5. Explain how to set up a route in React.
        The first step to setting up a route in React is to install/add react-router-dom. Next we need to import BrowserRouter (as Router), Link, and Route from react-router-dom into App.js. We will also need to import each individual page component. In order to render the Router, and each individual route embedded within, we will need to add <Router> and each individual <Route> within our return. In each Route we will need to add a path that specifies a matcher for the browsers url, and a component that we want to render when there is a match. The link component should be used to establish links to each route. 
        
#### 6. When would you use a generate resource over a generate controller?
        rails g resource will generate a model file in the models directory, a migration file in our db/migrate directory, a view directory but no files, a controller file in our controller directory, and a resources routes in our routes.rb file. 
        rails g controller generates a controller file and the view files and test files associated with that newly created controller. 
        The key difference is that rails g controller does not create the model files we may need for our application, the migration files for our database, or a routes.rb file so that we can set up our CRUD operations. In other words, controller generators are not best for creating CRUD based features. 
        
#### 7. Explain the difference between a controller spec and a request spec.
        A controller spec is an RSpec wrapper for a Rails test. This allows us to simulate a single http request and specify an expected outcome. In July 2016, the Rails RSpec team released a statement requesting that we use request specs instead of controller specs. This is because request specs allow us to focus on a singular controller action while also involving the router, the middle-ware stack, and both rack requests and responses. This supposedly adds a realism factor to the tests and avoids many of the pitfalls associated with controller specs. 

#### 8. Describe the React component lifecycle. What are some of the lifecycle methods?
        The React component lifecycle consists of three primary phases: 
        1.) Mounting - when a component is put into the DOM.
            The Mounting phase consists of the constructor method, which is activated before the component is mounted and initializes the local state of the component. This phase also includes the render method and the componentDidMount method, which is called after all of the elements on the page have rendered correctly. componentDidMount is typically used to fetch data from an external API and call the setState method to re-render the element with updated data.
        2.) Updating - When something in the component is updated (state).
            The Updating phase also includes the render method but adds the componentDidUpdate method as well. componentDidUpdate is invoked after updating has occured and is usually used to compare current state/props to previous state/props. 
        3.) Unmounting - When a component is removed from the DOM.
            The Unmounting phase consists of the componentWillUnmount method. This is the last function to be called right before the component is to be removed from the DOM. It is generally used to perform clean up for any DOM elements or timers we've established in componentDidMount. 

#### 9. At this point in the program, what technologies/languages do you find yourself gravitating to?
        At the point I'm having a hard time deciding which direction I want to go. I really enjoy Ruby on Rails and working with PostgreSQL and Active Record. Alternatively, React and the front-end tools/languages we've used are really cool as well. I think I need to spend more time with both before I'm ready to decide which direction I want to focus on. 
