# Tasteology

Tasteology is a Vue 3 + TypeScript + Vite project designed to showcase visually appealing components and layouts using Tailwind CSS. The project includes reusable Vue components and assets to create a modern, responsive web application.

---

## Table of Contents

1. [Project Setup](#project-setup)
2. [Development](#development)
3. [Build and Preview](#build-and-preview)
4. [Folder Structure](#folder-structure)
5. [Key Features](#key-features)
6. [Components](#components)
7. [Styling](#styling)
8. [Dependencies](#dependencies)

---

## Project Setup

To set up the project locally, follow these steps:

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd tasteology
   ```

2. Install dependencies:
   ```sh
    npm install
   ```

## Development

 To start the development server, run:

   ```sh
    npm run dev
   ```
  This will start a Vite development server, and you can access the application at http://localhost:[port].

## Build and Preview

To build the project for production, run:

   ```sh
    npm run build
   ```

  To preview the production build locally, run:

   ```sh
    npm run preview
   ```

## Folder Structure

```yaml
.gitignore
[index.html](http://_vscodecontentref_/0)
[package.json](http://_vscodecontentref_/1)
[README.md](http://_vscodecontentref_/2)
[tailwind.config.ts](http://_vscodecontentref_/3)
[tsconfig.app.json](http://_vscodecontentref_/4)
[tsconfig.json](http://_vscodecontentref_/5)
[tsconfig.node.json](http://_vscodecontentref_/6)
[vite.config.ts](http://_vscodecontentref_/7)
.vscode/
  [extensions.json](http://_vscodecontentref_/8)
  [settings.json](http://_vscodecontentref_/9)
public/
  vite.svg
src/
  [App.vue](http://_vscodecontentref_/10)
  [main.ts](http://_vscodecontentref_/11)
  [style.css](http://_vscodecontentref_/12)
  [vite-env.d.ts](http://_vscodecontentref_/13)
  assets/
    vue.svg
    img/
      card-block-1.png
      card-block-2.png
      card-block-3.png
      image-text-block-1.png
      image-text-block-2.png
      image-text-block-3.png
  components/
    [Card.vue](http://_vscodecontentref_/14)
    [CardBlock.vue](http://_vscodecontentref_/15)
    [ImageTextBlock.vue](http://_vscodecontentref_/16)
```
## Key Features

- **Vue 3 Composition API:** Utilizes <code><script setup></code> for concise and efficient component development.
- **TypeScript:** Ensures type safety and better developer experience.
- **Tailwind CSS:** Provides utility-first styling for rapid UI development.
- **Vite:** Fast build tool and development server.
- **Reusable Components:** Modular and reusable Vue components for scalability.

## Components

<code>Card.vue</code>
- Displays an image, title, and description.
- Props:
  - **image** (String, required): Path to the image.
  - **title** (String): Title of the card.
  - **description** (String): Description text.

<code>CardBlock.vue</code>
  - A collection of cards displayed in a grid layout.
  - Uses the Card component to render individual cards.
  - Data:
    - Array of card objects with title, image, and description.

<code>ImageTextBlock.vue</code>
 - Displays a grid of images alongside a descriptive article.
  - Data:
    - Array of image objects with image and class properties.

## Styling
The project uses Tailwind CSS for styling. Key customizations include:
  - **Custom Fonts:** Open Sans is imported and applied globally.
  - **Dark Mode:** Enabled by default using the dark variant.
  - **Responsive Design:** Tailwind utilities ensure layouts adapt to different screen sizes.


## Dependencies
Production Dependencies
  - **vue:** Core Vue 3 library.
  - **tailwindcss:** Utility-first CSS framework.
  - **@tailwindcss/vite:** Tailwind CSS integration with Vite.

## Development Dependencies
  - **vite:** Build tool and development server.
  - **@vitejs/plugin-vue:** Vue plugin for Vite.
  - **typescript:** TypeScript language support.
  - **vue-tsc:** TypeScript type checking for Vue components.
  - **@vue/tsconfig:** Shared TypeScript configuration for Vue projects.
  - **@types/node:** TypeScript definitions for Node.js.

## Additional Notes
  - **IDE Support:** Recommended to use Visual Studio Code with the Volar extension for Vue 3 support.
  - **Custom Configuration:**
    - Tailwind CSS is configured in <code>tailwind.config.ts</code>.
    - TypeScript configurations are split across <code>tsconfig.json</code>, <code>tsconfig.app.json</code>, and <code>tsconfig.node.json</code>.