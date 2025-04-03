# React Native Jobs App with Bookmarks

## Overview

This is a React Native application built with Expo that allows users to browse job listings and bookmark their favorite jobs. The app features:

- Bottom navigation with "Jobs" and "Bookmarks" tabs
- Infinite scrolling job listings
- Job details screen
- Bookmark functionality with offline storage
- Loading and error states

## Features

### 1. Bottom Navigation

- **Jobs tab**: Displays job listings fetched from the API
- **Bookmarks tab**: Shows all bookmarked jobs stored locally

### 2. Jobs Screen

- Fetches data from [API](https://testapi.getlokalapp.com/common/jobs?page=1)
- Implements infinite scrolling
- Displays job cards with:
  - Title
  - Location
  - Salary
  - Phone number

### 3. Job Details Screen

- Shows additional details when a job card is clicked

### 4. Bookmark Functionality

- Users can bookmark/unbookmark jobs
- Bookmarked jobs persist using AsyncStorage
- Available for offline viewing

### 5. State Management

- Loading states during API calls
- Error handling for failed requests
- Empty state displays

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/react-native-jobs-app.git
cd react-native-jobs-app
```

Install dependencies:

```bash
npm install
# or
yarn install
```

Start the development server:

```bash
expo start
```

## Dependencies

- **React Navigation** (Bottom Tabs, Stack)
- **Axios** for API calls
- **AsyncStorage** for local storage
- **React Native Vector Icons**
- **Expo** (for cross-platform development)

## Screenshots

(Include screenshots or GIFs of the app in action here)

## Video Demo

(Link to video demonstration)

## Code Structure

```plaintext
/src
  /components
    JobCard.js
    LoadingIndicator.js
    ErrorMessage.js
    EmptyState.js
  /screens
    JobsScreen.js
    BookmarksScreen.js
    JobDetailsScreen.js
  /navigation
    AppNavigator.js
    BottomTabNavigator.js
  /utils
    api.js
    storage.js
  /contexts
    BookmarksContext.js
App.js
```

## Implementation Notes

- Used **React Context API** for managing bookmarks state
- Implemented **custom hooks** for API calls and infinite scrolling
- Added **pull-to-refresh** functionality
- Optimized performance with **FlatList** and memoization
- Included proper **error handling and loading states**

## Future Improvements

- Add **search functionality**
- Implement **authentication**
- Add **more job filters**
- Improve **offline support**
- Add **animations and transitions**

## Author

Purru Annaiah
anilpurrum@gmail.com
https://github.com/Anilpurrum2011/
