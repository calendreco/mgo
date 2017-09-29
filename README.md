Note
-------------------------

This branch is based off the 10gen version with some fixes.
To work on this
```
go get gopkg.in/mgo.v2
cd $GOPATH/src/gopkg.in/mgo.v2
git remote add 10gen https://github.com/10gen/mgo.git
git remote add calendre https://github.com/calendreco/mgo.git
git checkout calendre/v2
```

To pull in the latest 10gen changes while keeping our bugfixes
```
git fetch 10gen
git checkout calendre/v2
git merge 10gen/v2
git push
```

To ship a feature
```
git checkout v2
git reset --hard calendre/v2
git checkout -b feature/new-feature
git commit -am 'great features'
git push calendre feature/new-feature
```

The MongoDB driver for Go
-------------------------

Please go to [http://labix.org/mgo](http://labix.org/mgo) for all project details.

