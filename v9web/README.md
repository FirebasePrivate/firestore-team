Using your own v9 SDK:


```
cd firebase/firebase-js-sdk/packages/firestore
yarn build
yarn pack  # this resulted in a tar file (e.g. firebase-firestore-v3.4.4.tgz)
cp firebase-firestore-v3.4.4.tgz ~/myproject/
cd ~/myproject
npm install ./firebase-firestore-v3.4.4.tgz
webpack --mode=development 
firebase deploy --only hosting
```
