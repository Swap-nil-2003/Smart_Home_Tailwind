# Smart_Home_Tailwind
Built a simple landing page for a smart home decor company using Tailwind CSS.

# Setting up Tailwind:
* Install Tailwind CSS
Install tailwindcss and its peer dependencies via npm, and create your tailwind.config.js file.

Command:

npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init

* Add Tailwind to your PostCSS configuration
Add tailwindcss and autoprefixer to your postcss.config.js file, or wherever PostCSS is configured in your project.

postcss.config.js:

module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  }
}

* Configure your template paths
Add the paths to all of your template files in your tailwind.config.js file.

tailwind.config.js:

/** @type {import('tailwindcss').Config} */ 
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

* Add the Tailwind directives to your CSS
Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.

main.css:

@tailwind base;
@tailwind components;
@tailwind utilities;

* Start your build process
Run your build process with npm run dev or whatever command is configured in your package.json file.

Terminal:

npm run start

* Start using Tailwind in your HTML
Make sure your compiled CSS is included in the <head> (your framework might handle this for you), then start using Tailwind’s utility classes to style your content.
 

# Technologies Used:
HTML5, Tailwind CSS, Javascript.

# Live Link:
https://smart-home-tailwind.netlify.app/
