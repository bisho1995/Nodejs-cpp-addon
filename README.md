## Nodejs native modules

Cloned and edited the repo https://github.com/fcanas/node-native-boilerplate.
<br>

## How it works

Basically we can have cpp code, aka native code, in our nodejs projects. We can compile the cpp code to a .node file and can import the .node file in out nodejs project. In this way we can make use of native code. The advantage is cpp is faster and it can take advantage of multithreading and lot of things like that.
<br>
We can make use of cpp modules, aka those written in cpp and build wrappers for them in nodejs. In this way we can reuse a lot of code. It will also be very performant as well.
<br>

This project has a file called **NativeExtension.cc**, this is our file which will have the cpp code. We are compiling this file using the node-gyp package from npm to native code. Look at the npm start command from the package.json It cleans the project, aka removes the build folder, then it configures,idk what it does there and then builds it. The .node file is in the release folder inside build.
<br>
We can then require it in any of our nodejs project and use it.
<br>
Follow this link
<br>
https://nodejs.org/api/addons.html#addons_building
<br>
for more information about making cpp files and compiling them to .node files.
