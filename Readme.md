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
### Jobs Screen :
  <table align="center"> <tr> <td><img src="https://github.com/user-attachments/assets/8131d1c3-1367-401e-9aa9-b48dac336e74" width="400"></td> <td><img src="https://github.com/user-attachments/assets/0c43a795-373c-4e66-bfae-fc4c09ae16f0" width="400"></td> </tr> </table>

</p>

### Job Details Screen : 
<table align="center"> <tr> <td><img src="https://github.com/user-attachments/assets/2372d14e-9e39-4f3b-8bd8-e113c137927e" width="400"></td> <td><img src="https://github.com/user-attachments/assets/ea3535cd-aa7b-4b04-bbb3-4c9e116ae357" width="400"></td> </tr> </table>

### Bookmark Functionality :
<table align="center"> <tr> <td><img src="https://github.com/user-attachments/assets/f0c48798-31d8-4f32-9333-096b9c346b9e" width="400"></td> <td><img src="https://github.com/user-attachments/assets/4242a33a-c231-472a-9d2a-31c368755cb2" width="400"></td> </tr> </table>
      
### Video Demo

<video width="640" height="360" controls>
  <source src="https://github.com/Anilpurrum2011/LokalApp-Assignment/raw/main/LokalApp%20Screenrecoder.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Code Structure:

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
