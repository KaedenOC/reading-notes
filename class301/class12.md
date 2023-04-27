# CRUD

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

## Status Codes

- **100's** - Informational. Indicates that the request was received and the process is continuing.

- **200's** - Success. Indicates that the request was successful.

- **300's** - Redirection. Indicates that further action is needed to complete the request.

- **400's** - Client Error. Indicates that there was an error on the client side.

- **500's** - Server Error. Indicates that there was an error on the server side.

- **202** - That the request has been accepted for processing, but the processing has not been completed yet.

- **308** - That the resource has been moved permanently to a new location and the client should update its URL.

- If an update didn't return data to a client, you would use the status code **204** No Content.

- You would use the status code **410** Gone, if a resource used to exist but no longer does.

- **403** -  'Forbidden' - The client does not have permission to access the requested resource.

## Build With Node.js, Express, and MongoDB

[Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

- We need to pull our MongoDB database string out of our server and put it into our .env file for security reasons, as we don't want to expose sensitive information in our code.

- **Middleware** is a function that sits between the client and the server and can modify the request or response as needed. It can also perform other tasks, such as logging or authentication.

- **app.use(express.json())** is middleware that allows our server to parse incoming requests with JSON.

- The **/:id** in a route is a parameter that allows us to access a specific resource based on its ID.

- **PUT** is used to update an entire resource, while PATCH is used to update only part of a resource.

- Set a default value for a field using the "default" property in the schema definition.

- **500** error status code means that there was a server error and the request could not be completed.

- Difference between a status 200 and a status 201 is that a 200 status code means that the request was successful, while a 201 status code means that the request was successful and a new resource was created as a result.

``` javascript
  
  //need to define middleware, must be defined before endpoints
  
  app.use(express.json());

//endpoint to add a book to the database

app.post('/books', postBook);

async function postBook(request, response, next) {
  try {
    //TODO: take in the data that comes in on the request
    let bookData = request.body;

    //TODO: have my model create the new instance of a book to my DB
    let createdBook = await Book.create(bookData)

    //TODO: send that on the response
    response.status(200).send(createdBook);

    //Thunderclient to test, change to POST, follow whats in schema
  } catch (error) {
    next(error);
  }
}

// ENDPOINT TO DELETE BOOK

async function deleteBook(request, response, next) {
  try {
    app.delete('/books/:bookID', deleteBook);   // '/books/:bookID'  <-- path param>

    let id = request.params.bookID;

    await Book.findByIdAndDelete(id);

    console.log(request.params);

    response.status(200).send('book deleted');

  } catch (error) {
    next(error);
  }
}

//thunderclient to test delete.. http://localhost:3001/books/(id of object goes here)






//FRONT END CONTAINER FORM BUTTON label for title, description, status in modal component?

onSubmit={this.handleBookSubmit} on Form

//ADDING A BOOK VIA 2 HANDLERS

// 1st handler - grab form data and build out a book object - run on form submission

handleBookSubmit = (event) => {
  event.preventDefault();
  //TODO: CONSTRUCT A CAT OBJ BASED ON THE FORM INPUT VALUES

  let bookObj = {
    title: event.target.title.value,
    description: event.target.description.value,
    status: event.target.status.checked
  } 
  //TODO: send this object to the back end - use a 2nd handler

  this.postBook(bookObj);
}
  console.log(bookObj);


postBook = async(bookObj) => {
  try {
    //TODO: build url for axios -> 
    let url = `${process.env.REACT_APP_SERVER}/books`

    //TODO: pass the url and the book data into axios on a POST and store the return in a variable
    let postBooks = await axios.post(url, bookObj);

    //TODO: update state with the newly created book
    this.setState({
      books: [...this.state.books, postBook.data]
    })
  } catch(error) {
    console.log(error.message);
  }
}

//TODO: HANDLER TO DELETE BOOKS BCUZ THIS IS WHERE STATE IS

deleteBook = async (bookID) => {
  try {
    //TODO: BUILD OUT THE URL FOR AXIOS
    let url = `${process.env.REACT_APP_SERVER}/books/${bookID}`

    console.log('url in delete', )
    //TODO: PASS THAT URL INTO AXIOS ON A DELETE
    await axios.delete(url);
    //TODO: UPDATE STATE
    let updatedBooks = this.state.books.filter(book => book._id !== bookID);

    this.setState({
      books: updatedBooks,
    })


  } catch(error) {
    next(error.message);
  }
}

// buttuon -> onClick={() => this.props.deleteBook(this.props.book._id)}



```