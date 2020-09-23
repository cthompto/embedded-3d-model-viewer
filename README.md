# embedded-3d-model-viewer
Simple example of code to embed a 3D model into a webpage hosted on GitHub. Please review the guide found here first:
https://codelabs.developers.google.com/codelabs/model-viewer/index.html?index=..%2F..index#2

The below steps are based on this guide and are meant to help connect the guide to Github Pages. 

The GitHub repo for the scripts being used can be found here:

https://github.com/google/model-viewer

Detailed documentation for all the availble commands ad options can be found here:

https://modelviewer.dev/

Steps:

1. Make a new GitHub Project

    a. Set it to public.
    
2. In "Settings" on GitHub navigate down to GitHub Pages and active the project as a GitHub page. 

    a. Make the master branch the source.
    
    b. Note the web address.
    
3. Upload the assests used to your new GitHub repo.

    a. Upload them to the root.
    
    b. If errors occur try using the GitHub desktop application to push new files to your repo.
    
4. Create a new index.html file in your GitHub repo and include the following.
    
    a. Add the following scripts to the <head>:
    
       <script src="https://unpkg.com/@webcomponents/webcomponentsjs@2.1.3/webcomponents-loader.js"></script>
       <script src="https://unpkg.com/intersection-observer@0.5.1/intersection-observer.js"></script>
       <script src="https://unpkg.com/resize-observer-polyfill@1.5.1/dist/ResizeObserver.js"></script>
         
    b. Add the following scripts to the bottom of <body>:
    
       <script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.js"></script>
       <script nomodule src="https://unpkg.com/@google/model-viewer/dist/model-viewer-legacy.js"></script>
         
    c. Add the following to create a model viewer, using your own source URL and alt text:
    
       <model-viewer src="your source here" alt="Your alt text here."></model-viewer>
    
    d. Add other elements as desired.
    
5. Test and share using the URL from the GitHub Pages section.
