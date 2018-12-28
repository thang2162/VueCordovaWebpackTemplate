# VueCordovaWebpackTemplate

##How to use:##
1. run: npm install
2. add platforms:  
cordova platform add android  
cordova platform add ios

3. build and run:  
npm run build && cordova run android  
npm run build && cordova build android  
npm run build && cordova run ios --buildFlag='-UseModernBuildSystem=0'  
npm run build && cordova build ios --buildFlag='-UseModernBuildSystem=0'  

##To create a project using the vue and cordova cli do the following:##
1. Create Vue project using Cli via command ('vue create my-project') or ui ('vue ui')
2. Create Cordova Project ('cordova create MyApp')
3. copy contents of folder containing cordova project into vue Project
4. Create a vue.config.js file and put into root of vue Project
5. Add the following to vue.config.js:  
const path = require("path");  
module.exports = {  
  baseUrl: '',  
  outputDir: 'www'
};  

6. add '<script type="text/javascript" src="cordova.js"></script>' to index.html in public folder
7. Use any of the following build commands:
npm run build && cordova run android  
npm run build && cordova build android  
npm run build && cordova run ios --buildFlag='-UseModernBuildSystem=0'  
npm run build && cordova build ios --buildFlag='-UseModernBuildSystem=0'  
