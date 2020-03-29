# Udagram Image Filtering Microservice

  

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

  

## Github link

https://github.com/pongsottich/image-filter-starter-code

  

## Usage

### Installation

Once you have downloaded the repository, open a terminal inside the repository and install the dependencies as follows:

  

```

$ npm install

```

  

### Dependecies

```typescript

"@types/express": "^4.17.0",

"@types/node": "^11.13.17",

```

  

### Start the server for develop

After you finish install any dependencies. You can try to start the development server by run :

```

$ npm run dev

```

  

## REST API

<b>URL</b> : /filteredimage

<b>Method</b> :  GET

<b>Query Parameter</b> : image_url (URL of the image to filter)

<b>Auth required</b> : No

  
  

## Response

  
```
| Response Code | Definition						|
| ------------- |:---------------------------------:|
| 200	        | Success			   				|
| 400	        | Error - No image_url parameter	|
| 404			| Error - URL not found				|
```


## Images
### AWS elastic beanstalk application dashboard
![enter image description here](https://raw.githubusercontent.com/pongsottich/image-filter-starter-code/master/deployment_screenshots/deployment_screenshot.png)``
## URL
### EB_URL
http://image-filter-starter-code-dev2.us-east-1.elasticbeanstalk.com

### End Point URL
http://image-filter-starter-code-dev2.us-east-1.elasticbeanstalk.com/filteredimage?image_url=[image url]


## Example
### Image before filter 
> https://myhero.com/content/images/thumbs/0033769_bob-marley.jpeg

![enter image description here](https://myhero.com/content/images/thumbs/0033769_bob-marley.jpeg)

### Image after filter 
![enter image description here](https://raw.githubusercontent.com/pongsottich/image-filter-starter-code/master/deployment_screenshots/filteredimage.jpg)
