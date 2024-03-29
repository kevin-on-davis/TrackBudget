# TrackBudget

L2K_TrackBudget
Due to the generosity of our instructors, the assignment was already completed on the students' behalf. The task as outlined was to implement IndexedDB so budget tracker data is persistent. All of IndexedDB code to be written in `public/db.js`.

## Instructions

- Create a new db request for a `budget` database.

- Inside `onupgradeneeded`, create an object store called `pending` and set `autoIncrement` to `true`.

- Inside your `saveRecord()` function:

  - Create a transaction on the `pending` object store with `readwrite` access.

  - Access your pending object store.

  - Add a record to your store with the `add` method.

- Inside the `checkDatabase` function:

  - Open a transaction on your `pending` object store.

  - Access your `pending` object store.

  - Get all records from store and set to a variable.

- Inside `getAll.onsuccess`:

  - If successful, open a transaction on your `pending` object store.

  - Access your `pending` object store.

  - Clear all items in your store.

## 💡 Hint(s)

- You can use the the comments in `public/db.js` as a guide.

## 🏆 Bonus

- Create a button that resets all funds to zero in your indexedDB.
