# silicon-valley-camp

[![Join the chat at https://gitter.im/maodouio/silicon-valley-camp](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/maodouio/silicon-valley-camp?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
硅谷Meteor孵化营

## Demos
* http://meteorhunt.meteor.com
* http://meteoric.github.io
* http://pikpak.meteor.com
* http://liklak.meteor.com
* http://welog.meteor.com
* http://reactioncommerce.com
* http://materializecss.com

## Install
* http://docs.meteor.com/
* http://atmospherejs.com

### Useful Commands
* pwd
* mkdir Github
* meteor create myapp
* meteor
* meteor help
* meteor list-sites
* meteor authorized limingth.meteor.com
* meteor authorized limingth.meteor.com help
* meteor authorized limingth.meteor.com --add fradac
* meteor authorized limingth.meteor.com --remove fradac
* meteor create --help
* meteor create --list 
* meteor create --example localmarket

## Tools
* pop
* Sublime Text 3

## Design
* Form New 
* List
* Item Detail

# From Prototype to Template
## Meteor Template
* name
* layout
* parameter

## Meteor Router
* name 
* data

## Meteor Server and Client
* seed
* allow
* collections
* autoform

## UI Frameworks
### Bootstrap
* http://getbootstrap.com/
* http://www.bootcss.com/
* https://atmospherejs.com/twbs/bootstrap
  - meteor add twbs:bootstrap

### Inoic
* http://meteoric.github.io
* https://atmospherejs.com/meteoric/ionic
  - meteor add meteoric:ionic-sass
  - meteor add meteoric:ionicons-sass
  - meteor add meteoric:ionic
  - meteor add meteoric:autoform-ionic

### Inspinia
* https://wrapbootstrap.com/themes/admin
* http://wrapbootstrap.com/preview/WB0R5L90S
* http://maodou-webdemo.meteor.com/

### Material Design
* http://materializecss.com
* https://atmospherejs.com/materialize/materialize
   - meteor add materialize:materialize

## Other Packages
* default
  - autopublish
  - insecure
* iron-router
  - iron:router
* autoform 
  - aldeed:collection2
  - aldeed:autoform
  - aldeed:simple-schema
  - yogiben:autoform-file
* cfs
  - cfs:standard-packages
  - cfs:gridfs

## From templates to beta version
### Collection
* http://docs.meteor.com/#/basic/Mongo-Collection

### Robomongo
* http://robomongo.org/download.html

### Mongo DB
* http://docs.mongodb.org/manual/

## Data submit
### Autoform
* http://autoform.meteor.com

### cfs
* https://github.com/CollectionFS/Meteor-CollectionFS

### autoform-file
* https://github.com/yogiben/meteor-autoform-file

## Data list view
* Mongo ops
  * find
  * fetch
  * sort
    - Projects.find().fetch()
    - Projects.find({}, {sort: {createdAt: -1}}).fetch()
    - Projects.find({}, {sort: {createdAt: -1}, limit:2}).fetch()
* helper
* events
* Spacebars
  * #each
  * #with
  * #if/else

## Data detail view
* pathFor
* Router data/:id


# Router and Data
## Iron Router
* https://github.com/iron-meteor/iron-router
* http://iron-meteor.github.io/iron-router/

## Pub/Sub
* http://docs.meteor.com/#/basic/pubsub

### publish-composite
  - https://atmospherejs.com/reywood/publish-composite

# Deploy
## AWS
* http://aws.amazon.com/ec2/
  - launch instance (ubuntu 14.04 64-bit paravirtual)
  - download pem file
  - change security group: Inbound (all traffic)
  - ssh -i your.pem ubuntu@your-ip-address

## Mup
* https://github.com/arunoda/meteor-up
  - https://github.com/arunoda/meteor-up#installation
  - Install npm: https://nodejs.org/

* How to use mup
  - npm install -g mup
  - mup 
  - cd your-project-dir
  - mup init
    - mup.json
    - settings.json 
  - modify mup.json
    - Example File: https://github.com/kevingzhang/welog/tree/master/mup
  - mup setup
    - ssh -i xxx.pem ubuntu@xx.xx.xx.xx ifconfig
  - mup deploy 

## How to make an app
* https://www.meteor.com/tutorials/blaze/running-on-mobile
  - meteor install-sdk ios
  - meteor add-platform ios
  - meteor run ios
  - meteor run ios-device
  - meteor run ios-device --mobile-server maodou-weixin.meteor.com
