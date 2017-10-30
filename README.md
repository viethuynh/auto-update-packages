# Auto update all packages to latest at once
1/ Copy file wipe-dependencies.js to your root project
2/ Open package.json and add below line into scripts: "update:packages": "node wipe-dependencies.js && rm -rf node_modules && npm update --save-dev && npm update --save"
3/ Run: npm run update:packages
4/ Enjoy!