# More CRUD

[CRUD Basics](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)

- Use the HTTP methods **PUT** or **PATCH** to update a record through an API. PUT is used for complete updates while PATCH is used for partial updates.

[Speed Coding: Building a CRUD API](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

- CRUD operations (Create, Read, Update, Delete) are used to perform actions on resources in a RESTful API. In other words, RESTful APIs use CRUD operations to manipulate resources.

- Five steps to create a RESTful API:

1. Identify the resources.

2. Define the endpoints.

3. Choose the appropriate HTTP methods for each endpoint, GET, POST, PUT, PATCH, or DELETE.

4. Specify the data to be returned, JSON, XML.

5. Document the API.

``` javascript
// lab notes 

// ENDPOINT TO UPDATE A BOOK //findByIdAndUpdate() backend

app.put('/books/:bookID', updateBook);

async function updateBook(request, reponse, next) {
  try {
    //TODO: grab the id from the request.params and data from the request.body
    let id = request.params.bookID;
    let bookData = request.body;

    //TODO: use the model method of findByIDAndUpdate and pass in the id, data, options object
    // 3 args, Id, data, options object -> { new: true, overwrite: true }
    let optionsObj = { new: true, overwrite: true };
    let updatedBook = await Book.findByIdAndUpdate(id, bookData, optionsObj);

    //TODO: send on the response, the updated book
    response.status(200).send(updatedBook);
    this.updateBook(bookObjUpdate)
  } catch (error){
    next(error)
  }
} //test with thunderclient http://localhost:3001/books/ID -> PUT paste in the body json data, update the data.

//front end render a form on button click? 

constructor(props) {
  super(props);
  this.state = {
    showForm: true
  }
}

<Button onClick={this.handleOpenForm}></Button>

<>
{this.state.showForm && 
  <UpdateBookForm 
    book={this.props.book}/>
}
</>

class UpdateBookForm extends Component {
  render() {
    return (
      //form stuff goes here on form defaultValue={this.props.book.title} -> form control
      // defaultChecked={this.props.book.status}
    )

  }
}

handleBookSubmit = (event) => {
  event.preventDefault();

  let bookToUpdate = {
    title: event.target.title.value,
    description: event.target.description.value,
    status: event.target.status.checked,
    _id: this.props.book._id
    __v: this.props.book.__v
  }
}


//update book handler --- call this function on form submit?

updateBook = async (bookObjToUpdate) => {
  try {
    //TODO: create the url for axios -> needs id in path param
    let url = `${process.env.REACT_APP_SERVER}/books/${bookObjToUpdate._id}`
    //TODO: send axios on a put with the url and data
    let updatedBook = await axios.put(url, bookObjToUpdate);

    //TODO: update state with the updated book returned from axios // return from axios -> updatedBook.data
    let updatedBookArray = this.state.books.map(existingBook => {
      return existingBook._id === bookObjToUpdate._id ? updatedBook.data : existingBook;
    })

    this.setState({
      book: updatedBookArray
    })

  } catch {

  }

}
```