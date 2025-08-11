# Movie_App_React

A modern React application for browsing and managing your favorite movies. Built with React, Vite, and the TMDB API.

## Features

- 🎬 Browse popular movies
- 🔍 Search for movies by title
- ❤️ Add/remove movies to favorites
- 💾 Persistent favorites storage (localStorage)
- 📱 Responsive design
- ⚡ Fast development with Vite

## Tech Stack

- **Frontend**: React 18
- **Build Tool**: Vite
- **Routing**: React Router DOM
- **State Management**: React Context API
- **Styling**: CSS3 with custom components
- **API**: The Movie Database (TMDB) API

## Prerequisites

Before running this project, you need:

1. **Node.js** (version 16 or higher)
2. **npm** or **yarn**
3. **TMDB API Key** (free)

## Getting Started

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Movies_React/frontend
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Get TMDB API Key

1. Visit [The Movie Database](https://www.themoviedb.org/)
2. Create an account or sign in
3. Go to [API Settings](https://www.themoviedb.org/settings/api)
4. Request an API key (choose "Developer" option)
5. Copy your API key

### 4. Configure API Key

Open `src/services/api.js` and replace the empty API_KEY:

```javascript
const API_KEY = "your_actual_api_key_here";
```

**⚠️ Important**: Never commit your actual API key to version control. Consider using environment variables for production.

### 5. Start Development Server

```bash
npm run dev
```

The app will open at `http://localhost:5173`

## Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── movieCard.jsx   # Individual movie display card
│   └── NavBar.jsx      # Navigation header
├── contexts/            # React Context for state management
│   └── MovieContext.jsx # Favorites state and functions
├── pages/               # Main page components
│   ├── Home.jsx         # Movie browsing and search
│   └── Favorites.jsx    # User's favorite movies
├── services/            # API and external services
│   └── api.js          # TMDB API integration
├── CSS/                 # Component-specific styles
└── assets/              # Images and static files
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## API Endpoints Used

- **Popular Movies**: `/movie/popular`
- **Search Movies**: `/search/movie`

## Features in Detail

### Home Page
- Displays popular movies on load
- Search functionality with real-time results
- Loading states and error handling
- Responsive movie grid layout

### Favorites
- Add/remove movies from favorites
- Persistent storage using localStorage
- Empty state when no favorites exist

### Movie Cards
- Movie poster with overlay
- Favorite toggle button
- Movie title and release year
- Hover effects and animations

## Troubleshooting

### Page Not Loading
- Check if you've added your TMDB API key in `src/services/api.js`
- Ensure the development server is running (`npm run dev`)
- Check browser console for error messages

### API Errors
- Verify your API key is correct
- Check if you've exceeded API rate limits
- Ensure you have an active internet connection

### Development Server Issues
- **Windows PowerShell**: Use Command Prompt (cmd.exe) instead, or change execution policy
- **Port conflicts**: Vite will automatically try different ports if 5173 is busy

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for providing the movie data API
- [React](https://reactjs.org/) team for the amazing framework
- [Vite](https://vitejs.dev/) for the fast build tool

---
