# Oh.Studio Clone

This project is a clone of the [Oh.Studio](https://oh.studio/) website built using **HTML** and **TailwindCSS**. The aim is to replicate the design and animations of the original site while maintaining simplicity and responsiveness.

## Features

- Sticky navigation bar with active link highlighting.
- Animated hero section with a bouncing text effect.
- Responsive grid layout for showcasing images and videos.
- Hover effects on gallery items (blur and brightness adjustments).
- Fully responsive design for different screen sizes.

## Technologies Used

- **HTML5**: For the structure of the webpage.
- **TailwindCSS**: For styling and layout.
- **JavaScript**: For configuring Tailwind animations.

## Preview

![Preview of the clone](preview-Oh.Studio.png)


## File Structure

```
├── assets
│   ├── images
│   │   ├── aire.avif
│   │   ├── correlated.avif
│   │   ├── channel_5.avif
│   │   ├── ronald_abraham.avif
│   │   ├── schuh.avif
│   │   ├── paperstreet.avif
│   └── videos
│       └── propeller.mp4
├── pages
│   ├── profile.html
│   └── contacts.html
├── index.html
├── icono.jpg
└── README.md
```

## Tailwind Configuration

The animation for the hero section is implemented using custom TailwindCSS configuration. Below is the snippet added to extend Tailwind's default settings:

```javascript
<script>
  tailwind.config = {
    theme: {
      extend: {
        keyframes: {
          bounceUpDown: {
            '0%, 100%': { transform: 'translateY(0)' },
            '50%': { transform: 'translateY(-20px)' },
          },
        },
        animation: {
          bounceUpDown: 'bounceUpDown 1s ease-in-out',
        },
      },
    },
  };
</script>
```

## How It Works

- **Hero Section**: The title text uses the custom `bounceUpDown` animation defined in the Tailwind configuration.
- **Gallery**: A responsive grid layout showcases images and a video with hover effects to enhance interactivity.
- **Sticky Navbar**: The navigation bar remains visible while scrolling, ensuring ease of navigation.


## License

This project is open-source and available under the [MIT License](./LICENSE).

---

**Author**: Jonathan Salinas
