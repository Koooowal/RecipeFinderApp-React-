# Recipe Book App

A modern React application for discovering and exploring recipes across various cuisines. This application uses the Spoonacular API to fetch recipe data and provides an intuitive interface for users to browse popular recipes, search for specific dishes, and filter by cuisine type.

![Recipe Book App](https://placeholder-image.com/recipe-book-app.png)

## Features

- **Homepage with Featured Recipes**
  - Popular recipe carousel
  - Vegetarian recipe recommendations
  - Smooth animations between page transitions

- **Recipe Filtering**
  - Browse by cuisine (Italian, American, Thai, Japanese)
  - Search functionality for specific ingredients or recipe names

- **Detailed Recipe Views**
  - Full recipe instructions
  - Ingredients list
  - Recipe summary and information

- **Responsive Design**
  - Works on desktop and mobile devices
  - Intuitive navigation and user interface

## Technologies Used

- React 18
- React Router v6 for navigation
- Styled Components for styling
- Framer Motion for animations
- Spoonacular API for recipe data
- React Splide for carousels
- React Icons for UI elements
- Local Storage for caching API responses

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/recipe-book.git
   cd recipe-book
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add your Spoonacular API key:
   ```
   REACT_APP_API_KEY=your_spoonacular_api_key_here
   ```

4. Start the development server:
   ```bash
   npm start
   ```

5. Open [http://localhost:3000](http://localhost:3000) to view the app in your browser.

## Project Structure

```
recipe-book/
├── public/
├── src/
│   ├── Components/
│   │   ├── Category.jsx    # Cuisine category navigation
│   │   ├── Popular.jsx     # Popular recipes section
│   │   ├── Search.jsx      # Search functionality
│   │   └── Veggie.jsx      # Vegetarian recipes section
│   ├── Pages/
│   │   ├── Cuisine.jsx     # Cuisine-specific recipes page
│   │   ├── Home.jsx        # Homepage component
│   │   ├── Pages.jsx       # Routes configuration
│   │   ├── Recipe.jsx      # Individual recipe details page
│   │   └── Searched.jsx    # Search results page
│   ├── App.js              # Main app component
│   └── index.js            # Entry point
└── package.json
```

## Usage

### Home Page
The home page displays popular and vegetarian recipe carousels. Users can scroll through these carousels to discover new recipes.

### Cuisine Categories
Users can click on cuisine icons to filter recipes by cuisine type:
- Italian
- American
- Thai
- Japanese

### Search
The search bar allows users to find recipes by name or ingredient. Enter a search term and press enter to see matching recipes.

### Recipe Details
Click on any recipe card to view detailed information, including:
- Recipe instructions
- Ingredients list
- Summary information

## API Usage

This application uses the Spoonacular API for recipe data. The API is called with the following endpoints:

- Random recipes: `https://api.spoonacular.com/recipes/random`
- Recipe search: `https://api.spoonacular.com/recipes/complexSearch`
- Recipe details: `https://api.spoonacular.com/recipes/{id}/information`

API responses are cached in local storage to reduce API calls and improve performance.

## Performance Optimization

- Local storage caching of API responses
- Lazy loading of images
- Efficient state management
- Callback optimization with useCallback hook

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Acknowledgments

- [Spoonacular API](https://spoonacular.com/food-api) for providing recipe data
- [React Icons](https://react-icons.github.io/react-icons/) for the icon collection
- [Styled Components](https://styled-components.com/) for the styling solution
- [Framer Motion](https://www.framer.com/motion/) for animations
- [React Splide](https://splidejs.com/integration/react-splide/) for carousels