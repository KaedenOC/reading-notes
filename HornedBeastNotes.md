# Feature Model For Understanding

## App Component

Renders the main layout of the application which includes Header, Main, SelectedBeast, and Footer components.

Manages the state of the application including clickedBeast, showModal, beastImg, beastDescription, and filteredBeast.

Defines a handlefilter method that filters the beasts based on the selected horn option and updates the state accordingly.

Defines an updateSelectedBeast method that updates the state with the clicked beast's information.

Defines a closeModalHandler method that closes the modal for the selected beast.
Passes down the filteredBeast, updateSelectedBeast, and closeModalHandler methods as props to the Main and SelectedBeast components.

## Main Component

Renders the main content of the application, which includes a HornForm component for filtering the beasts and a list of HornedBeast components for displaying the beasts.

Receives beasts data as props from the App component.

Maps through the beasts data and renders a HornedBeast component for each beast.

Passes down the title, imageUrl, description, and clickState as props to the HornedBeast components.

## HornForm Component

Renders a form with a select dropdown for filtering the beasts based on the number of horns.

Calls the onFilter method passed down from the Main component when the select value changes.

## HornedBeast Component

Renders a single beast card with its title, image, and description.

Calls the clickState method passed down from the Main component when the card is clicked.

## SelectedBeast Component

Renders a modal that displays the clicked beast's information including title, image, and description.

Receives the clickedBeast, beastImg, beastDescription, show, and onClose as props from the App component.

Calls the onClose method passed down from the App component when the modal is closed.

## Header and Footer Components

Render the header and footer of the application respectively.
