# Mini Project 2 - Photo Gallery with Favorites

A simple photo gallery web app built with **Vue 3** that allows users to:

- Add photos by URL
- Mark/unmark photos as favorites (star toggle)
- Remove photos by clicking on the image

---

## Demos


---

## Features

- **Add Photos:** Submit a URL via the input form to add a photo to the gallery.
- **Favorite Photos:** Click the gold star button to toggle the favorite status of a photo.
- **Remove Photos:** Click directly on a photo to remove it from the gallery.
- **Responsive Gallery:** Uses CSS Grid to display photos evenly in a 4-column layout.
- **User Feedback:** Shows a friendly message when no photos are present.

---

## Technologies Used

- **Vue 3 (Composition API)** for reactive UI
- **CSS Grid** for layout
- **Normalize.css** to reset browser styles
- Vanilla JavaScript

---

## How It Works

- The gallery is an array of photo objects (`{ id, url, isFavorite }`), stored as a reactive `ref`.
- Adding photos pushes new photo objects into the array.
- Toggling favorite updates the boolean `isFavorite` property, which updates the star's color.
- Removing photos filters out the photo by ID.
- Conditional rendering shows a "No photos added yet" message when the gallery is empty.

---

## CSS Highlights

- `.gallery` uses CSS Grid with 4 equal columns and 10px gaps.
- `.photo img` fills the container width and displays as a block element for consistent sizing.
- `.favorite-button` positioned in bottom-right corner of each photo, styled as a star that changes color when active.
- `.no-photos` displays a centered message when the gallery is empty.

---

## Usage

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Enter an image URL in the input box and click **Add Photo**.
4. Click the star button on any photo to mark/unmark it as favorite.
5. Click on a photo to delete it.

---

## Future Improvements

- Persist photos and favorites in `localStorage` or backend.
- Add drag-and-drop to reorder photos.
- Add validation to check if the image URL is valid.
- Add transitions/animations for adding/removing photos.
- Support image captions or titles.

---

<br>

Feel free to customize or ask if you want a more detailed README or one with screenshots/tutorials!
