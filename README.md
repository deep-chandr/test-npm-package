This project was bootstrapped with [Create React App]

# Reference: https://www.pluralsight.com/guides/export-reactjs-components-as-node-modules-to-npm

Steps:

1.  npm install --save-dev @babel/cli @babel/preset-react
2.  Script
    "publish:npm": "rm -rf dist && mkdir dist && babel src/component -d dist --copy-files"
3.  Set path in 'main' key in `package.json` file
4.  Set babel settings
    "babel": {
    "presets": [
    "@babel/preset-react"
    ]
    }
5.  npm login
6.  npm run publish:npm
7.  npm publish
