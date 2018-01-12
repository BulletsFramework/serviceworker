# Service Worker for WordPress

This simple service worker:

- Caches your themes static assets e.g. graphics, styles and JS
- Caches pages of your site as your visitors browser, maximum 25
- Caches an Offline page which is displayed if a page not in the cache is requested

Pre-requisites
--------------

- Your website must have an offline page. This is cached within the `offlineFundamentals` object. Make sure any static assets this page requires are also included in the cache.
- Edit the theme foldername to match yours, and edit the static assets within `offlineFundamentals` to match the stylesheets and JS your theme uses.
- Don't forget to register the service worker in your footer, and that the service worker must reside in the root directory of your site. If you'd prefer it to be within the theme, you could create a symbolic link.
