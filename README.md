### :point_right: CloudFront website link: https://d36xt76wa2f2x8.cloudfront.net/
### :point_right: S3 link: https://s3.console.aws.amazon.com/s3/buckets/sk-second-app/?region=us-east-1&tab=overview

- [+]**Install** the latest version of Serverless Framework (https://www.serverless.com/).
- [+]**Configure** credentials for AWS to make them accessible by Serverless.
- [+]**Clone** **MyShop!** single page app from [FE repository](https://github.com/rolling-scopes-school/nodejs-aws-fe). (PLEASE DON'T CREATE PRs WITH YOUR TASK IMPLEMENTATION TO THIS REPOSITORY)
- [+]**Install** dependencies…
- [+]**Check** if everything works for you...

### 2.1 (manual deployment):
1. [+]In the AWS Console **create** and **configure** **S3 bucket** where you will host your app (follow instructions in training materials).
2. [+]**Build** and **manually upload** the MyShop! app to the created S3 bucket. Check if the app is available through the Internet over **_http://{your-bucket-name}.s3-website-{aws-region}.amazonaws.com_** .
3. [+]**Create** a _CloudFront distribution_ for your app as it was described in training materials. **Check** your S3 bucket policy changes. **Check** if the app is available through the Internet over given CloudFront URL.
4. [+]**Make** some minor but visible changes in the app, **build** and **upload** them to your bucket, and create CloudFront distribution invalidation.

### 2.2 (automated deployment using serverless-finch + serverless single-page-app plugins):

1. [+]**Add** and **configure** _serverless_ and _serverless-finch_ plugin. Add necessary npm script(s) to build and deploy your app from your machine in an automated way. (_See the_ [demo repo](https://github.com/boale/serverlessTestApp)). **Check** if everything works correctly for you. (_Please note, that after uploading an application's build to the S3 bucket you need to create manually a CloudFront invalidation_).
2. [+]**Destroy** created AWS infrastructure (S3 bucket and CloudFront distribution) from the previous part and steps. **Make sure** nothing is left.
3. [+]**Add** and **configure** _serverless-single-page-app-plugin_ as it is implemented in the demo repository. **Add** necessary npm script(s) to build, upload to your S3 bucket, and invalidate CloudFront cache from your machine in an automated way. Check if everything works fine and all changes appear on the Web. (_Please note, that you don’t need to manually create CloudFront invalidations any more_).



This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:  
You can use NPM instead of YARN (Up to you)  

### `yarn start` OR `npm run start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test` OR `npm run test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build` OR `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject` OR `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
