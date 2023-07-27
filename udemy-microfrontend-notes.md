[Course Link](https://www.udemy.com/course/microfrontend-course/)

# Ch 3
* Direct communication between two micro-frontends (MFE) is not advisable. Each MFE is responsible to maintain its own state communicating with the service

# Ch 5, Ch 6
* Integration
	* Build-Time integration
		* Pros
			* Easy to setup and understand
		* Cons
			* Container has to be redeployed everytime a dependent mfe is updated
			* Tempting to tightly couple the container + MFE(s) together, as container has the source code access of the he dependent mfe
	* Run-Time integration
		* Pros
			* Dependent MFE(s) can be deployed independently at any time
			* Different versions of the MFE can be deployed and container can decide which one to use
		* Cons
			* Tooling + setup is far more complicated
			* Server integration : While sending down JS to load up Container, as server decides on whether or not to include MFE source.

# Ch 8
* Create package.json
	```
	npm init -y
	```
* Install dependencies (Product Module)
	```
	npm install webpack@5.88.0 webpack-cli@4.10.0 webpack-dev-server@4.7.4 faker@5.1.0 html-webpack-plugin@5.5.0
	```

# Ch 10
* Webpack : Combines many JS files (source code and dependencies) into one single file (created inside the `dist` folder)

# Ch 13
**Container Module dependencies**  
```
npm install webpack@5.88.0 webpack-cli@4.10.0 webpack-dev-server@4.7.4 html-webpack-plugin@5.5.0 nodemon
```
	