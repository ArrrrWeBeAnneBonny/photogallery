# Anne Bonny - Hipcamp.com Photogallery Service

Hipcamp.com is an ecommerce website that tailors to landowners and campers. On hipcamp.com, users can post parts of their land for consumers to "rent" for a few nights, much like AirBnB. But unlikely AirBnB, consumers are not renting homes, or appartments, but the land in a (hopefully) secluded area for them and some company to enjoy on a camping holiday. 

For Hack Reactors Front End Capstone (FEC) Project, we (the Anne Bonny group) was tasked with recreating a faithful item page, using modern front-end applications like React, Node, and MongoDB, as well as utalizing AWS for deployment. My Service is the "Photogallery". This service is in charge of the interactive image carousel that all campsite pages have. On this service, users can scroll through images that "users" have upload, "like" images, and quickly post them on several social media website (FB, Insta, Twitter, Pintrest).

## Related Projects

  - https://github.com/ArrrrWeBeAnneBonny/booking
  - https://github.com/ArrrrWeBeAnneBonny/overview
  - https://github.com/ArrrrWeBeAnneBonny/reviews

## Table of Contents

1. [Usage](#Usage)
2. [Requirements](#requirements)
3. [Installing Dependencies](#dependencies)
4. [Seeding Database](#database)
5. [Deployment](#deployment)

## Usage

![](photogallery_gif.gif)

> This service contains a photo gallery app, that contains one endpoint ('GET ‘/photogallery/?campId=’ ' that calls on mongoDB to prodvide an array of information, including:
```sh
- Usernames
- Date Published
- Location
- An Array of Uploaded Images
- Likes
- An Array of Captions
```
> It also calls on the Overview Service (not currently deployed), this will retrun the location of the campsite.
> ![alt text](photogallery.png)

## Requirements

Latest version of:
```sh
- Node.js / Express
- Webpack/Babel
- React
- Mongoose
- Jest
- Axios
```

package.json is included

## Installing Dependencies

From within the root directory:

```sh
npm install -g webpack
npm install
```

## Seeding The Database

From within the root directory: 
```sh
 - npm run seedCollection
 
Wait several minutes for the collections to populate. The time this takes will vary by hardware

 - npm run seed
 
Population of documents may take several minutes
```

## Deployment

If deploying, run from within the root directory:
```sh
npm run build-dev
npm run start
connect to http://localhost:3004/
```


