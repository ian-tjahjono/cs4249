# FoodLeh?

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### About us
We are a free, crowdsourced hawker platform in Singapore relying on Singaporeans to share information about our local F&B places. We love hawker food and hope you do too! If you want to contribute, hop over here: [contributing.md](https://github.com/limyifan1/hawkercentral/blob/master/CONTRIBUTING.md)

### Database Structure
We have 4 collections in use: hawkers, deliveries, cuisine, etc. The hakwers and deliveries collection are the most relevant.  <br/> 
##### hawkers collection: 
Each new hawker listing added as a new document, with an auto-generated id. Each document has the data has shown in data dictionary below<br/>
##### deliveries collection: 
Each delivery request is added as a new document, with an auto-generated id. Data still to be confirmed. 

### Data Dictionary (hawkers collection)
  url: (string) the first image uploaded, which is the cover picture<br />
  image2: (string) second image uploaded<br />
  image3: (string) third image uploaded<br />
  image4: (string) fourth image uploaded<br />
  image5: (string) fifth image uploaded<br />
  image6: (string) sixth image uploaded<br />
  name: (string) name of the stall<br />
  cuisine: (array<object>) array of cuisine tags<br />
  categories: (array<string>) the same, but with cuisine expressed as strings. Used for filtering<br />
  postal: (number) postal code of the stall<br />
  street: (string) street name of the stall autogenerated from OneMap api<br />
  unit: (string) unit number<br />
  description: (string) short description of the stall with char limit<br />
  description_detail: (string) long description of the stall<br />
  region: (array<object>) array of potential regions like north, south, east, west, islandwide<br />
  regions: (array<string>) the same, but regions expressed as strings. Used for filtering<br />
  islandwide: (boolean) now redundant, was used to check if delivery is islandwide<br />
  delivery: (string) now redundant, was used to list areas of delivery<br />
  price: (number) delivery fee<br />
  contact: (number) contact number of the stall<br />
  latitude: (number) now redundant<br />
  longitude: (number) now redundant<br />
  call: (boolean) indicates whether user should call the stall<br />
  whatsapp: (boolean) indicates whether user should whatsapp the stall<br />
  sms: (boolean) indicates whether user should sms the stall<br />
  inperson: (boolean) indicates whether user should visit the stall inperson<br />
  opening: (string) opening hours for the stall<br />
  pickup_option: (boolean) indicates customer can pick up from stall<br />
  delivery_option: (boolean) indicates customer can deliver from stall<br />
  website: (string) website url<br />
  promo: (string) promo e.g. 30% off<br />
  condition: (string) condition for promo e.g. if order more than $40<br />
  delivery_detail: (string) more details regarding <br />
  menu: (boolean) indicates whether there is a menu added<br />
  menuitem: (array) array of menu items<br />
  menuprice: (array) array of menu prices mapped by index to menuitem<br />
  docid: (string) document id generated by firebase<br />
  wechatid: (string) WeChat contact id<br />
  location: (object) Geopoint location generated with geo.point(Number(this.state.latitude), Number(this.state.longitude))<br />

## Available Scripts

In the project directory, you can run:

### `npm install`
Installs the app and necessary dependencies. More dependencies may need to be installed manually.

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify

# LICENSE

[MIT](LICENSE)
