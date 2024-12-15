
## Introduction

**HD Media Explorer** is a responsive web application designed to provide a seamless way to search and watch high-definition movies, TV shows, and episodes. By leveraging the IMDb search and embedding content from trusted streaming services, this tool allows users to easily discover and play their favorite media.

The user interface features a gradient-rich, animated background with a modern and accessible design. It dynamically adjusts inputs based on the type of media being searched, ensuring a straightforward and user-friendly experience.

---

## Features

1. **Dynamic Media Type Selection:**
   - Choose between **Movies**, **TV Shows**, or **Episodes**.
   - Inputs for season and episode numbers are displayed only when relevant.

2. **Media Search:**
   - Utilizes IMDb's search capabilities to identify media by name.

3. **HD Media Embedding:**
   - Embeds content using the `vidsrc.xyz` streaming service.
   - Automatically constructs URLs for movies, TV shows, and specific episodes.

4. **Responsive Design:**
   - Fully responsive layout with support for mobile, tablet, and desktop views.

5. **Animated UI Enhancements:**
   - Gradient backgrounds with smooth animations.
   - Loading spinner for a polished user experience.

---

## How to Use

### 1. Prerequisites
Ensure you have:
- A modern web browser (e.g., Chrome, Firefox, Edge).
- Access to the internet.
- Optionally, ensure the [CORS Anywhere proxy](https://cors-anywhere.herokuapp.com/) is active. If it is inactive, you can set up your own proxy instance or modify the fetch requests.

---

### 2. Launching the App
1. Open [Free HD Media Search](https://rockyandthepawpatrol20.github.io/freemoviewatch.github.io/)
---

### 3. Searching for Media
1. **Select Media Type:**
   - From the dropdown menu, choose between:
     - **Movie**
     - **TV Show**
     - **Episode** (requires season and episode numbers).
   
2. **Enter Media Name:**
   - Type the name of the media you want to find.

3. **For Episodes:**
   - Provide the season number and episode number.

4. **Click `Search & Watch`:**
   - A loading spinner will appear while the system retrieves data.

---

### 4. Watching Media
- After a few moments, the content will embed directly in the application.
- The player is fully interactive and supports fullscreen playback.

---

## Code Walkthrough

### 1. **HTML Structure**
- A simple layout with:
  - **Search Controls:** Dropdown, text inputs, and a button for triggering searches.
  - **Loading Indicator:** A spinner animation displayed while fetching data.
  - **Iframe Container:** Displays the embedded media player.

### 2. **CSS Styling**
- **Modern Design:**
  - Gradient animations for backgrounds.
  - Smooth transitions for hover effects and focus styles.
- **Responsiveness:**
  - Adjusts styles for smaller screens using media queries.

### 3. **JavaScript Logic**
- **Event Handlers:**
  - Dynamically shows/hides season and episode inputs based on the media type.
- **Fetching Media:**
  - Uses IMDb search results to extract the unique `IMDb ID`.
  - Constructs appropriate URLs for embedding.
- **Error Handling:**
  - Alerts users if a media item cannot be found or if inputs are invalid.
- **Dynamic Embedding:**
  - Creates an iframe with the constructed URL and embeds it in the container.

---

## Important Notes
1. **Proxy Setup:**
   - The script uses the [CORS Anywhere](https://cors-anywhere.herokuapp.com/) proxy to bypass cross-origin restrictions. If the public instance is unavailable, consider hosting your own instance.

2. **Embedding Restrictions:**
   - Ensure compliance with content licensing and regional restrictions when using the embedded player.

3. **Third-Party Dependencies:**
   - This project relies on IMDb and `vidsrc.xyz`. Service availability may affect functionality.

---

## Browser Compatibility
| Browser         | Compatibility |
|------------------|---------------|
| Google Chrome    | ✅ Full Support |
| Mozilla Firefox  | ✅ Full Support |
| Microsoft Edge   | ✅ Full Support |
| Safari           | ✅ Full Support |

---

## Potential Enhancements
- Add support for custom media players.
- Integrate user authentication and media bookmarks.
- Provide fallback options for unavailable media.

---

## Troubleshooting
1. **Media Not Found:**
   - Double-check the media name for typos.
   - Verify if IMDb contains the requested content.

2. **Loading Indicator Stuck:**
   - Refresh the page and try again.
   - Check network connectivity.

3. **Embed Not Loading:**
   - Ensure `vidsrc.xyz` is operational.

---
