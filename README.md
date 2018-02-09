## Introduction
**Note**: This issue only show in iOS 11.2.5, not in ios 10.2.1

This project demonstrates the [issue](https://github.com/ionic-team/ionic/issues/13982#issuecomment-364095352). It only adds code below in a tab template.
```
home.ts

ionViewDidEnter() {
    let loader = this.loadingCtrl.create({
      content: "Please wait...",
      duration: 3000
    });
    loader.present();
  }
```
## Version

* ionic: 3.10
* cordova: 7.10.1
* Node: 8.1.4
* npm: 5.4.1

## Usage
```
git clone https://github.com/JerryMissTom/loadingissue.git

npm install

ionic cordova platform add ios

ionic cordova build ios --prod

```
Then use Xcode open the ios project in platforms/ios, run or archive.
