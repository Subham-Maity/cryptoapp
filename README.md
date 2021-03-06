# Web3 Based Crypto Verse Application made By [Subham](https://subham-maity.github.io/subham/)

<hr>

## Working Frameworks

### 1. Frontend 
⭐ **[Using RapidAPI](https://redux.js.org/)** 
⭐ **[ReactJS](https://reactjs.org/)** 
⭐ **JS** [learn javascript from my js bootcamp [here](https://github.com/Subham-Maity/js-bootcamp)]
⭐ **HTML**[learn HTML from my HTML bootcamp [here](https://github.com/Subham-Maity/html-tutorial-for-beginners)]
⭐ **CSS**  /Tailwind

### 2. Smart contract for its functionality(backend) Using P2P network

⭐ **Solidity** 
- learn solidity from my Solidity bootcamp [here](https://github.com/Subham-Maity/solidity-tutorial)

(Solidity is an object-oriented, high-level language for implementing smart contracts on various blockchain platforms, most notably, Ethereum)

### 3. Api 
⭐ [**Coin Ranking Api**](https://rapidapi.com/Coinranking/api/coinranking1/)
⭐ [**Paw**](https://paw.app/)

### 4.Blockchain
⭐ **Ethereum Blockchain**

- learn blockchain from my documentation from [here](https://github.com/Subham-Maity/blockchain-basic)
- learn Ethereum from my documentation from [here](https://github.com/Subham-Maity/ethereum-tutorial)
<hr>

<h2 align=center>Contributors in This Project✨</h2>

Thanks to these **Wonderful People** 👨🏻‍💻 <br>
**Contributions** of any kind are welcome! 🚀

<table>
	<tr>
		 <td>
 <a href="https://github.com/Subham-Maity/cryptoapp/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Subham-Maity/cryptoapp" />
</a>
  </a>
		</td>
	</tr>
</table>

⭐ Star this repo on GitHub — it helps!
************
## Steps for making this project 

**1. First create a folder without space** 

**2. Open this folder through vs code/WebStorm(My Recommendation)** 

**3. open terminal and type** 
```text
npx create-react-app ./
```
**and wait for 1-2 minutes** 

**4. Delete the source folder which already made and create a source folder by yourself**

**5.Create index.js inside the SRC folder and Import this** 
```js
//index.js
import React from 'react';
import ReactDOM from 'react-dom';
import App from './App';
ReactDOM.render(<App/>, document.getElementById ('root'));
```
ReactDOM.render then inside here we need to pass this app as a component as a first parameter and then finally say
document.getElementById then '**root**' to hook our app onto our root div


**6. behind the scenes this means that we have a public with one index.html file now this html file looks a bit weird at the start but Remove some space and commends and make it as a simple html file** 

like this 
```html
<!--index.html-->
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />
    <meta name="description" content="Web site created using create-react-app"/>
    <link rel="apple-touch-icon" href="%PUBLIC_URL%/logo192.png" />
    <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
    <title>CryptoApp</title>
  </head>
  <body>
  <div id="root"></div>
  </body>
</html>

```
- You can copy this and paste on your index file 

**7. Make an app.js inside the SRC file** 

**8. Simple type rsc in WebStorm / type rafce in Vscode(install this app plugins ES7 React/Redux/GraphQL/React-Native snippets)** 

for this boilerplate 

```jsx
//App.js
import React from 'react';

const MyComponent = () => {
    return (
        <div>

        </div>
    );
};

export default MyComponent;

```

**9. Now add heading 'Cryptoxam' like this**

```jsx
//App.js
import React from 'react';

const MyComponent = () => {
    return (
        <div>

            <h1>Cryptoxam</h1>

        </div>
    );
};

export default MyComponent;
```

**10. Open your terminal and type 'npm start'(allow network) and look at your browser** 
```text
npm start
```
 
- For terminate the app just type on your terminal "Ctrl" + "C" and press Y
- then type clear for clear the terminal 
```text
clear
```

**11. Now again open terminal we can start by installing all the  necessary dependencies we can install  the dependencies by typing npm install  and now we can start listing all of the  dependencies  for styling we're going to use and  design so you can simply type antd  then we also need design so -design/ icons ... icons for the icons. We are also going to use redux, so you can  install react-redux @reduxjs/toolkit  then we're also going to use axios to  make api requests we're going to use  chart.js to create charts  we're going to use html react parser to  parse some html data we're also going to  use a hand a little package called millify that's going to transform  extremely large numbers into readable  strings  finally we're going to use moment to  parse times and dates, and we also need react-chartjs-2 to render those charts from  charges in our React application  there we go these are all the packages  that we need you can simply press enter ,and we're going to wait a few moments**

```txt
npm install antd @ant-design/icons react-redux @reduxjs/toolkit axios chart.js html-react-parser millify moment react-chartjs-2

```


**12. Now just type on the terminal after installation " npm start "**

```text
npm start 
```
- output will be react-scripts start

**13.** 
- Now open App.js and import this 
```js
//App.js
import { Switch, Route, Link } from 'react-router-dom';
import { Layout, Typography, Space } from 'antd';
```
and delete the heading and create three div for navbar main and footer 

- Entire code like this 
```jsx
//App.js
import React from 'react';
import { Switch, Route, Link } from 'react-router-dom';
import { Layout, Typography, Space } from 'antd';


const MyComponent = () => {
    return (
          <div className="app">
                <div className="navbar">
                </div>
                <div className="main">

                </div>
                <div className="footer">
                </div>
            </div>

    );
};

export default MyComponent;
```

**14. Create a folder in SRC folder name this folder as "components" and make a file Navbar.jsx inside components folder** 


**15. Type rfc for boilerplate in Navbar.jsx**

**16. For creating the navbar import some library** 
```jsx
//navbar.js
import React, { useState, useEffect } from 'react';
import { Button, Menu, Typography, Avatar } from 'antd';
import { Link } from 'react-router-dom';
import { HomeOutlined, MoneyCollectOutlined, BulbOutlined, FundOutlined, MenuOutlined } from '@ant-design/icons';
```
**17. We are gonna use some components(avatar,typography from antd) for this project and for now don't use button we are using it for phone later** 

- [ For more design you can find all the design from [**here**](https://ant.design/) ]

let's do this in your navbar.jsx for adding avatar typography and so on 

```jsx
<!--Navbar.js-->
<div className="nav-container">
      <div className="logo-container">
        <Avatar/>
        <Typography.Title level={2} className="logo">
            <Link to="/">Cryptoxam</Link></Typography.Title>
        {/*<Button className="menu-control-container" onClick={() => setActiveMenu(!activeMenu)}><MenuOutlined /></Button>*/}
      </div>
    </div>
```


**18. Now we are gonna add icon for our avatar you can download it from** [**here**](https://i.ibb.co/Z11pcGG/cryptocurrency.png)
- make a folder "images" in src folder 
- download the [image](https://i.ibb.co/Z11pcGG/cryptocurrency.png) and paste it on the images folder
- and drag it on to our image folder 
- edit the html avatar tag like this
```html
<!--Navbar.js-->
<Avatar src={icon} size="large" />
```
- and now import image location for icon  like this
```jsx
//Navbar.js
import icon from '../images/cryptocurrency.png';
```
**19. let's import this navigation bar into our App.js so that we can display it right here(App.js)**  

- components  from the components, folder looks like  this
```jsx
 import Navbar from './components/Navbar';
```
it's fine for one line or two lines or even three lines but later on you're going to have more components here it's not going to be just snap navbar and your code would look like this

```jsx
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
import Navbar from './components/Navbar';
```
so on....

- That's definitely not efficient or good-looking you're cluttering your view ,so I'm going to show you a little trick
- that's going to allow you to import all the components in one line
- to do that we can create a new file inside the 'components' folder called "index.js" inside here you can import this like import then curly braces....like this
```jsx
//index.js(component)
import { default as Navbar } from './Navbar';
```
this one line is going to allow us to import navbar in a different way


if we go to again App.js you no longer have to do it like this what you can do is like this 

```jsx
//index.js(src)
 import { Navbar } from './components';
```
Now add more like this

```jsx
//index.js (component)
 export { Navbar, Layout, Footer } from './components';
```

put navbar in curly braces and then  simply say dot slash components and now  all the components that you export  from here  are going to be importable like this  now bar we're gonna have for example a  layout  we're going to have footer  this seems really meaningful import  navbar layout and footer from components  ,and it's also in one line so that's a  cool little trick that you can use in  your React applications




**20.We are gonna export from index.js(component) to import app.js.Now we have to install " react router dom "**

for this do like this 

go to your app.js and open terminal and type
```text
 npm install react-router-dom
```
if your try to start npm start you might be faced an issue so for that you have to do 

go to your app.js and import this 

```jsx
//app.js
import { Switch, Route, Link } from 'react-router-dom';
```

Now so to be able to use links and other  things you need to wrap our app with the  router  so right inside here we can add the  router component ,and you need to put the app component inside it then that's going to look  something like this

```jsx
//app.js
ReactDOM.render(
  <React.StrictMode>
    <Router>
        <App />
    </Router>,
      document.getElementById('root')
      );
```

Then just do open app.js and open terminal 
```text
npm start
```
**21. For design, you have to make a css file(App.css) and just paste this on the file you make** 
```css

:root{
    --text-primary:#000;
    --bgPrimary:#fff;
   --bgSecondary: #F9F9F9;
   --pink: #0071bd;
   --light-blue: #e6f7ff;
   --border: #d9d9d9;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

a:hover{
    color: var(--pink) !important;
}

.app{
    display: flex;
    overflow: hidden;
}

.navbar{
    flex: 0.2;
    background-color: rgb(0, 21, 41);
}

.main{
    flex: 0.8;
    width: 100%;
    
}
.routes{
    padding: 20px;
}
.nav-container{
    position: fixed;
    left: 0;
    margin: 10px;
    height: 100vh;
    margin: 0px;
    background-color: rgb(0, 21, 41);
}

.logo-container{
    background-color: #001529;
    display: flex;
    padding: 20px;
    align-items: center;
    width: 100%;
}
.logo{
    margin:0 0 0 15px;
}
.logo a{
   color: white;
}
.menu-control-container{
    display: none !important;
    position: absolute !important;
    right: 10px !important;
    top: 25px !important;
    font-size: 1.2rem !important;
    background-color: var(--bgSecondary) !important;
    border: none !important;
}

.loader{
    height: 81vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

@media screen and (max-width:1300px){
    .main{
        margin-left: 50px;
    }
}

@media screen and (max-width:1170px){
    .main{
        margin-left: 50px;
    }
}

@media screen and (max-width:1000px){
    .main{
        margin-left: 100px;
    }
}

@media screen and (max-width:800px){
    .app{
        flex-direction: column;
        overflow: hidden;
    }

    .navbar{
        flex: 1;
    }

    .main{
        flex: 1;
        margin-top: 90px;
        margin-left: 0px;
        margin-right: 10px;
    }

    .nav-container{
        height: 8vh;
        position:fixed;
        width: 100%;
        z-index: 100;
        background-color: var(--bgSecondary);
    }
  
    .menu-control-container{
        display: block !important;
    }

    .ant-menu{
        position: absolute;
        right: 0px;
    }
    .home-title{
        font-size: 1.4rem !important;
    }
    .show-more{
        font-size: 1.3rem !important;
    }
}

.coin-detail-container{
    margin: 30px;
}

.coin-heading-container{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    border-bottom: 1px solid var(--border);
    padding-top: 20px;
    padding-bottom: 20px;
    gap: 10px;
}

.coin-heading-container .coin-name{
    font-weight: 900;
    color: var(--pink);
}

.coin-heading-container p{
    font-size: 1rem;
    opacity: 0.9;
    margin-bottom: 20px;
}

.stats-container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
}

.stats-container h2{
    font-weight: 700;
    font-size: 1.4rem;
    margin-top: 20px;
    color: var(--pink);
}

.coin-details-heading{
    font-weight: 700 !important;
    margin-top: 20px !important;
    color: var(--pink) !important;
}

.coin-stats{
    display: flex;
    justify-content: space-between;
    border-bottom: 1px solid var(--border);
    font-size: 1rem;
    opacity: 0.9;
    padding: 20px;

}

.coin-stats-name{
    display: flex;
    gap: 10px;
    font-size: 1rem;
}

.stats{
    font-weight: 800;
}

.coin-value-statistics-heading p{
    font-size: 1rem;
    opacity: 0.9;
}

.coin-desc-link{
    display: flex;
    gap: 40px;
    margin-top: 40px;
    padding-top: 20px;
}

.coin-desc-link h2{
    font-weight: 700;
    color: var(--pink);
}

.coin-desc-link p{
    font-size: 1rem;
    opacity: 0.9;
}

.coin-desc-link a{
    color: var(--pink);
}

.coin-desc-link h3{
    font-weight: 700;
}

.coin-desc{
    flex: 0.5;
}

.coin-links{
  padding: 0px 20px;
    flex: 0.5;
}

.coin-link{
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid var(--border);
    padding: 20px;
}

.link-name{
    text-transform: capitalize;
    font-size: 1rem;
}

.coin-link a{
    color: var(--pink);
    font-weight: 700;
    font-size: 1rem;
}

.coin-link:hover, .coin-stats:hover{
    background-color: var(--bgSecondary);
}

@media screen and (max-width:1000px){
    .stats-container{
        flex-direction: column;
    }
    .coin-desc-link{
        flex-direction: column;
    }
    .stats-container h2{
        margin-top: 0px;
    }
}

@media screen and (max-width: 500px){
    .coin-links{
        padding: 0px;
    }
    .coin-detail-container{
        margin: 0;
    }
}
@media screen and (max-width: 500px){
    .heading{
        margin-top: 20px;
    }
}

.select-news{
    width: 180px;
}
.news-card{
    min-height: 300px !important;
}
.news-image-container{
    display: flex !important;
    justify-content: space-between !important;
}
.news-title{
width: 70%;
}

.news-image-container .img{
    width:100px;
    height:100px;
}
.news-card p{
    color: black;
    margin: 10px 0px !important;
}
.provider-container{
    display: flex;
    justify-content: space-between;
}
.provider-name{
    margin-left: 10px;
}

.chart-header{
    display: flex;
    justify-content: space-between;
    gap: 50px;
    color: #0071bd;
}
.chart-title{
    color: #0071bd !important;
}
.price-container{
    display: flex !important;
    gap: 20px !important;
    align-items: center !important;
    flex-wrap: wrap !important;
}
.price-change{
    font-weight: 900 !important;
}
.current-price{
    margin-top: 0px !important;
    font-weight: 900 !important;
}
.home-heading-container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 40px;
}
.show-more{
    margin-top: 0px !important;
}
.exchange-image{
    margin: 0px 10px !important;
}
.search-crypto{
    margin: 20px auto 30px auto;
    width: 250px;
}
.crypto-card-container{
    min-height: 65vh !important;
}
.crypto-card{
    min-width: 250px;
}
.crypto-card .crypto-image{
    width:35px;
}
.select-timeperiod{
    width: 200px !important;
    margin-top: 20px !important;
}

.footer {
    background-color: #001529;
    display: flex;
    flex-direction: column;
    padding: 20px;
    align-items: center;
}
```

Now import this css on your App.js file like this 

```jsx
//App.js
import './App.css';
```
**22. navbar - menu** [Home,Cryptocurrencies,Exchange,News ]
- A menu is a component coming from ant design a menu is going to have a theme equal to dark 
- and inside there we can have  different menu items so let's create our  first menu
- we  already imported it but make sure to call it as a component with the opening component tag 
- make sure to  self-close it is like this is our menu item inside our menu  item 
- we are going to have a link tag so  in here we can say link  and more specifically the first one is  going to be 2 which is going to be equal to just forward slash which is our home  component  
- we can duplicate this link a few  more times  
- the second one is going to have the fund outlined icon,and it's going to go to cryptocurrencies  and of course d2 is also going to be slashed cryptocurrencies with the lowercase c 
- Then third icon is going to be  money  collect  outlined  this link is going to go to exchanges  and of course we can go to forward slash  exchanges with a lowercase e  f
- finally the last thing we can have a  bulb outlined icon 
- In here it's  going to point to news and then again  four slash news with a lowercase n  this is going to be our menu 
- let's save  it and take a look in the browser

```jsx

//navbar.jsx
/*<div className="nav-container">
      <div className="logo-container">
        <Avatar src={icon} size="large" />
        <Typography.Title level={2} className="logo"><Link to="/">Cryptoxam</Link></Typography.Title>
        <Button className="menu-control-container" onClick={() => setActiveMenu(!activeMenu)}><MenuOutlined /></Button>
      </div>*/
       
   
      
      <Menu theme="dark">
        <Menu.Item icon={<HomeOutlined />}>
          <Link to="/">Home</Link>
        </Menu.Item>
        <Menu.Item icon={<FundOutlined />}>
          <Link to="/cryptocurrencies">Cryptocurrencies</Link>
        </Menu.Item>
        <Menu.Item icon={<MoneyCollectOutlined />}>
          <Link to="/exchanges">Exchanges</Link>
        </Menu.Item>
        <Menu.Item icon={<BulbOutlined />}>
          <Link to="/news">News</Link>
        </Menu.Item>
      </Menu> 
</div>
);
    
```

**23. Open app.js and we need Homepage so and inside that we need exchanges cryptocurrencies and news for that 
just do this**
```jsx
// app.js
<div className="main">
      <Layout>
        <div className="routes">
          <Switch>
            <Route exact path="/">
              <Homepage />
            </Route>
            <Route exact path="/exchanges">
              <Exchanges />
            </Route>
            <Route exact path="/cryptocurrencies">
              <Cryptocurrencies />
            </Route>
            <Route exact path="/crypto/:coinId">
              <CryptoDetails />
            </Route>
            <Route exact path="/news">
              <News />
            </Route>
          </Switch>
        </div>
````

**24. now make Homepage.jsx and then Cryptocurrency.jsx inside the component folder** 

```jsx
//Homepage.jsx
 import React from 'react'
const Homepage = () ⇒ {
return (
<div>
Homepage
</div>
)
export default Homepage
```
same do this in Cryptocurrencies.jsx

```jsx
//Cryptocurrencies.jsx
 import React from 'react'

const Cryptocurrencies = () ⇒ {
return (
<div>
    Cryptocurrencies
</div>)
}
export default Cryptocurrencies

```

Let's do the same for Exchanges.jsx and News.js as I did both earlier 

**25. Now export components in index js(components )like this** 

```jsx
// indx.js(component)
export { default as Homepage } from './Homepage';
export { default as Navbar } from './Navbar';
export { default as News } from './News';
export { default as Cryptocurrencies } from './Cryptocurrencies';
export { default as Exchanges } from './Exchanges';
export { default as CryptoDetails } from './CryptoDetails';
```

make sure that is total 6 components in the componets folder
- Cryptocurrencies.jsx
- CryptoDetails.jsx
- Exchanges.jsx
- Homepage.jsx
- index.js (for export the components)
- Navbar.jsx
- News.jsx

**26. if your look at your website you can see something wrong allignment in the page for fixed this issue just import this
in your App.js folder** 
```jsx
// App.js 
 import 'antd/dist/antd.css';
```

**27.Let's make our footer part open App.js and add this** 
```jsx
// App.js
<div className="footer">
    <Typography.Title level={5} style={{ color: 'white', textAlign: 'center' }}><p>Copyright © 2022</p>
        <Link to="/">
            <p> <a href="https://github.com/Subham-Maity">Owned by Subham Maity</a></p>
        </Link> <br />
        All Rights Reserved.
    </Typography.Title>
    <Space>
        <Link to="/">Home</Link>
        <Link to="/exchanges">Exchanges</Link>
        <Link to="/news">News</Link>
    </Space>
```

- remember footer must be inside the div main 
- When we add content our footer part will go down

**28. Now go to Homepage.jsx**

import milify that's going to format our numbers 
```jsx
 // Homepage.jsx
 import millify from 'millify';
```
for ant design import this 
```jsx
// Homepage.jsx
 import { Typography, Row, Col, Statistic } from 'antd'; I
```
then add link for this 

```jsx
// Homepage.jsx
 import {Link} from 'react-router-dom';
```


**29. For Header Global Crypto Stats go to Homepage.jsx a**
```jsx
// Homepage.jsx
 const { Title } = Typography;
const Homepage = () => {
return(
    <>
        <Title level={2} className="heading">Global Crypto Stats from Cryptoxam</Title>
</>
)
}
```

**30.Now we need row and col where span is 12(space) for this do like this** 

- set value 5 later on we update the data don't worry (using api)
- make total 6 col for different lines (copy one line and add title)
```jsx
// Homepage.jsx
/*
 const { Title } = Typography;
const Homepage = () => {
return(
    <>
        <Title level={2} className="heading">Global Crypto Stats from Cryptoxam</Title>
</>
)
}
*/

            <Row gutter={[32, 32]}>
                <Col span={12}><Statistic title="Total Cryptocurrencies" value={globalStats.total} /></Col>
                <Col span={12}><Statistic title="Total Exchanges" value={millify(globalStats.totalExchanges)} /></Col>
                <Col span={12}><Statistic title="Total Market Cap:" value={`$${millify(globalStats.totalMarketCap)}`} /></Col>
                <Col span={12}><Statistic title="Total 24h Volume" value={`$${millify(globalStats.total24hVolume)}`} /></Col>
                <Col span={12}><Statistic title="Total Cryptocurrencies" value={globalStats.total} /></Col>
                <Col span={12}><Statistic title="Total Markets" value={millify(globalStats.totalMarkets)} /></Col>
            </Row>
```

**31. we can fetch real cryptocurrency data from rapid api using the redux toolkit**

to start fetching our data we are going  to go back to the rapid apis hub and  we're going to search for  coin  ranking  once this load you can click on this  blue button right here for you it might  say something different like subscribe  there is a free plan so don't worry  about that and as soon as you're  subscribed you'll be able to click here  to test the endpoint as you can see  you're immediately going to get all of  the possible data right away  so what do we have to do to use this api  well you can go under code snippets and  for now you can simply copy and paste  this options object  back in our app i'm going to close all  the files and folders  and we can go to source and create a new  folder  that folder is going to be called  services  that is redux's new way of fetching data  inside of services you can simply type  cryptoapi.js  and inside of here is where we'll do the  logic of fetching the data from the api  just so we don't forget about it you can  paste the options right here because we  have to use this data later on


https://rapidapi.com/Coinranking/api/coinranking1/

<p align="center">
        <img src="https://github.com/Subham-Maity/cryptoapp/blob/master/image(ignore)/1.png?raw=true"/>
        </p>


```js
//cryptoApi.js(src->services)

const options = {
    method: 'GET',
    url: 'https://coinranking1.p.rapidapi.com/coins',
    params: {
        referenceCurrencyUuid: 'yhjMzLPhuIDl',
        timePeriod: '24h',
        'tiers[0]': '1',
        orderBy: 'marketCap',
        orderDirection: 'desc',
        limit: '50',
        offset: '0'
    },
    headers: {
        'X-RapidAPI-Host': 'coinranking1.p.rapidapi.com',
        'X-RapidAPI-Key': '1d871cceacmshba48ac5bae3dc58p111f7bjsna1305d8edcc1'
    }
};
```


**32. but before we set crypto API we need to  create a store for our redux application  a store is one central state of truth  meaning your entire applications state, we can create a store by creating a  new folder in the source folder called app inside the app you can create one  file called store.js  redux simplified the process of creating  a store significantly you can simply say  import  and then import to configure store  function from  add redux js**

```jsx
//store.js(src->app)
import { configureStore } from '@reduxjs/toolkit';
```

**33.Export default configure store you need to call  it as a function and then pass an object  inside there  the first parameter in this object is  going to be reducer and for now we're  going to leave that as an empty object.**

```jsx
//store.js(src->app)
/*import { configureStore } from '@reduxjs/toolkit';*/



export default configureStore({
  reducer: {
      },
});
```

**34. Now that we're exporting the store let's actually use it inside our index.js**
```jsx
//index.js
import { Provider } from 'react-redux';
import { BrowserRouter as Router } from 'react-router-dom';


import App from './App';
import store from './app/store';
```
- import App from './App';
import store from './app/store';  this is the variable we have to provide to our provider 
so import { Provider } from 'react-redux';


- we have to do a  similar thing with it with this router  simply we have to wrap the app  by saying provider store and then  enclosing our app into that  as you can see we are now wrapping our  app with the router and also with the  provider where we are setting the store  variable to be equal to store

```jsx
//index.js
ReactDOM.render(
    <Router>
      <Provider store={store}>
        <App />
      </Provider>
    </Router>
document.getElementById('root'),
);
```

35. we can actually create the first piece of the data fetching functionality we can actually create the first  piece of the data fetching functionality  and we can do that by importing a few  things from redux js
```jsx
//cryptoApi.js(src->services)
import { createApi, fetchBaseQuery } from '@reduxjs/toolkit/query/react';

//for header 
const cryptoNewsHeaders = {
    'x-bingapis-sdk': 'true',
    'X-RapidAPI-Host': 'coinranking1.p.rapidapi.com',
    'X-RapidAPI-Key': '1d871cceacmshba48ac5bae3dc58p111f7bjsna1305d8edcc1'
};
```
later on we're going to replace these keys with environment variables so that they are not available to the public 

now store the url on the baseUrl variable 
```jsx
//cryptoApi.js(src->services)
 const baseUrl = 'https://coinranking1.p.rapidapi.com';
```

36.Export const crypto api  our crypto api is going to be equal to  create api that's coming from redux and  then we have to pass some options inside  of an object  first thing is going to be the reducer  path so we have to say what is this  reducer for  and you can simply provide the name here  in this case let's say crypto api  then you have to provide the base query  so right here base query is going to be  equal to  fetch base query which is a function  that accepts an object and inside of  there you can simply say base url is  equal to base url it's not bas url it's  base url  and the final and the most important  thing are the end points so we can say  endpoints  and that's going to be equal to a  function where you get a builder as a  first parameter  and that function instantly returns an  object  inside of that object you can specify  the names of the endpoints  for example something like get  cryptos  we can name it anything you want  and that's going to be equal to  dot query  you pass an object as options again and  then inside of there you say query  is equal to  and you provide a function that's going  to point to that specific request  so let's say that we want to get the  information for the exchanges in that  case it would simply be something like  forward slash  exchanges

```jsx
//cryptoApi.js(src->services)
 export const cryptoApi = createApi({
    reducerPath: 'cryptoApi',
});
baseQuery: fetchBaseQuery({ baseUrl }),
    endpoints: (builder) ⇒ ({
    getCryptos: builder.query({
        query: () ⇒ '/exchanges'
})
})
```
**37. if we want to make  this request we also need to pass the  headers so we can create a simple  utility function that's going to simply  add the url and the headers to our call  we can do that by saying const create  request  and that's going to be equal to a  function that accepts a url and simply  returns an object that contains the url  which is equal to the url and finally it  contains the headers which are equal to  crypto api headers**
```jsx
//cryptoApi.js(src->services)
/* const baseUrl = 'https://coinranking1.p.rapidapi.com';*/
 const createRequest = (url) ⇒ ({ url, headers: cryptoApiHeaders })
/*
export const cryptoApi = createApi({
    reducerPath: 'cryptoApi',
});
baseQuery: fetchBaseQuery({ baseUrl }),
    endpoints: (builder) ⇒ ({
    getCryptos: builder.query({
        query: () ⇒ '/exchanges'
})
})*/

```

**38.now instead of simply calling the  forward slash exchanges we can call  create request  and in there we can simply pass the url  which is in this case forward slash  exchanges**

```jsx
//cryptoApi.js(src->services)
/* export const cryptoApi = createApi({
    reducerPath: 'cryptoApi',
});
baseQuery: fetchBaseQuery({ baseUrl }),
    endpoints: (builder) ⇒ ({
    getCryptos: builder.query({*/

        query: () ⇒ createRequest('/exchanges')
/*
})
})*/

```

**38.we created a store in a storejs we  passed that store variable to a provider  that we are wrapping our app with as you  can see it's right here  and then we created a specific api that  we're going to use to fetch api data  from rapid api  now we need to find a way to connect  this api to the store  and we can do that by importing that api  import that's going to be crypto api  and that's going to be coming from  dot slash services slash  crypto  api  and the only thing you have to do is  inside of the reducers object  in square brackets  crypto  api  dot reducer path  and then that is equal to crypto api  that reducer  redux is doing everything for you you  just have to specify this for every  single reducer that you create as you  can see  we create an api and therefore we have  all of these variables like reducer path  and reducer  now our application is connected now we  have to see which data do we have to get  first and then fetch it from the  appropriate endpoint from the api**

```jsx
//store.js(src->app)
import { configureStore } from '@reduxjs/toolkit';

import { cryptoApi } from '../services/cryptoApi';


export default configureStore({
  reducer: {
    [cryptoApi.reducerPath]: cryptoApi.reducer,
   
  },
});

```