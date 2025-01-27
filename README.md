# Translation
A minimal single HTML application that allows for easy writing of bilingual translations.

## Overview
The Translation App is a web-based tool designed to facilitate translation tasks. It supports entering original sentences, adding translations, associating meanings to individual words, saving data as JSON, and resuming work by uploading saved files. The app provides a user-friendly interface with accessible keyboard shortcuts for efficient workflow management.

---

## Features

### 1. **Main Data Entry Page**
- Input original sentences and their translations.
- Add individual word meanings for each sentence.
- Edit or delete existing sentences.
- Automatically assigns and reorders sequences for each sentence.

### 2. **Save and Load Functionality**
- Save current data as a JSON file using:
  - **Button**: "Save"
  - **Shortcut**: `Ctrl + S`
- Load a previously saved JSON file to continue work.

### 3. **View Modes**
Toggle between different views for specific needs:
- **Original Sentences**:
  - Displays all original sentences in sequence.
  - Shortcut: `Alt + O`
- **Translated Sentences**:
  - Displays all translated sentences in sequence.
  - Shortcut: `Alt + T`
- **Words with Meanings**:
  - Displays all words and their meanings in sequence.
  - Shortcut: `Alt + W`
- **Back to Main Data Entry Page**:
  - Returns to the main interface for data entry.
  - Shortcut: `Ctrl + Shift + K`

### 4. **Keyboard Shortcuts**
| Action                         | Shortcut          |
|-------------------------------|-------------------|
| Save data as JSON             | `Ctrl + S`       |
| Load a saved JSON file        | Use upload button|
| View original sentences       | `Alt + O`        |
| View translated sentences     | `Alt + T`        |
| View words and meanings       | `Alt + W`        |
| Back to main data entry page  | `Ctrl + Shift + K`|

---

## Usage Guide

### Entering Data
1. Use the input box to type an original sentence.
2. Click **Next** or press `Enter` to confirm.
3. Add a translation and individual word meanings.

### Editing and Deleting
- **Edit**: Modify sentences or word meanings directly in the respective fields.
- **Delete**: Click the "Delete" button to remove a sentence.

### Saving Data
- Click **Save** or press `Ctrl + S` to download a JSON file of your work.

### Loading Data
- Click the file upload button and select a JSON file to resume work.

### Switching Views
- Use the view buttons or keyboard shortcuts to navigate between:
  - Originals
  - Translations
  - Words with meanings
  - Main data entry page

---

## JSON Schema
The app saves and loads data using the following schema:
```json
{
  "sentences": [
    {
      "sequence": 1,
      "original": "mama nAma Aditya",
      "translation": "my name is aditya",
      "word_translations": {
        "mama": { "translation": "my" },
        "naama": { "translation": "name" },
        "aditya": { "translation": "" }
      }
    }
  ]
}
```
- **sequence**: Numeric order of the sentence.
- **original**: The original sentence.
- **translation**: The translation of the sentence.
- **word_translations**: A mapping of words to their respective translations.

---

## Future Improvements
- Enhanced styling and dark theme options.

---

## Contact
For feedback or issues, reach out to adityabmv@gmail.com.

