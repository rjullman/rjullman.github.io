# Generating the Blog
1. Clone the repository 

  ```bash
  git clone git@github.com:rjullman/rjullman.github.io.git website; cd website;
  ```
  
2. Install [npm](https://docs.npmjs.com/getting-started/installing-node) and [buster](https://github.com/axitkhurana/buster#the-installation)
3. Start the ghost blog locally

  ```bash
  cd ghost-0.7.9/; GHOST_NODE_VERSION_CHECK=false npm start;
  ```
  
4. View and edit the blog at `localhost:2368` (go to `localhost:2368/ghost` for the admin interface)
5. Run `buster` from the project root directory to generate static pages:

  ```bash
  rm -rf blog; buster generate --dir=blog;
  ```
