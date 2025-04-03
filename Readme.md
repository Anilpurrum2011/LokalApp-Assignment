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
  - No. of Vacancies

### 3. Job Details Screen

- Shows additional details when a job card is clicked
- Job Details
    - Location
    - salary
    - Job Type
    - Qualification
    - Experience


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
git clone https://github.com/Anilpurrum2011/LokalApp-Assignment.git
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

## Screenshots :
     ![IMG-20250403-WA0005](https://github.com/user-attachments/assets/db79f2ac-0c17-46b1-bbbb-28ebc6a37f60)
     ![IMG-20250403-WA0006](https://github.com/user-attachments/assets/ad9f0004-e485-49d0-8154-637a80035ba5)
     ![IMG-20250403-WA0004](https://github.com/user-attachments/assets/2a0e518e-3fce-45ef-9ce6-9faf4b9431cd)
     ![IMG-20250403-WA0003](https://github.com/user-attachments/assets/0beaf880-689d-43ab-84f2-67739d8df3d8)
     ![IMG-20250403-WA0007](https://github.com/user-attachments/assets/1b96683c-3fca-4667-ac22-8460390a2097)
     
     ![IMG-20250403-WA0004](https://github.com/user-attachments/assets/85964c0a-d807-43c7-afd3-5b5947816b55)

      
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
    BookmarkButton.js
    Tag.js
  /screens
    JobsScreen.js
    BookmarksScreen.js
    JobDetailsScreen.js
  /navigation
    AppNavigator.js
    TabBarlcon.js
  /services
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

- Purru Annaiah
- anilpurrum@gmail.com
- https://github.com/Anilpurrum2011/
