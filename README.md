# Test UI5 Basic

## Setup

* Install **LTS version** of Node.js : https://nodejs.org/en/download/
* Install the repository
  - Either `git clone https://github.com/ArnaudBuchholz/test-ui5-basic.git`
  - Or **download** and **unzip** https://github.com/ArnaudBuchholz/test-ui5-basic/archive/refs/heads/main.zip
* Change **current directory** to `test-ui5-basic` directory
* Run `npm install`
* Run `npm start`

The application is available at http://localhost:8080

> If the port `8080` is already in use, this error will appear :
> 
> ```Error: listen EADDRINUSE: address already in use :::8080```
> 
> Then, **edit** the file `reserve.json` and **set** the value of `port` to `0`. Then run `npm start` again, a port will be **allocated** and **displayed**. For instance :
> 
> ```Server running at http://0.0.0.0:56121/```
>
> Meaning the application is available at http://localhost:56121

## Documentation

* OpenUI5 is documented [here](https://openui5.hana.ondemand.com/topic)
* The application is based on the [Quick Start
tutorial](https://openui5.hana.ondemand.com/topic/592f36fd077b45349a67dcb3efb46ab1) *(Steps 1 & 2)*

## Questions

### Add a new button named count

* Add a **new button** to the page, it should be labelled *Count*
* When clicking the button, a **Message Toast** should display the initial value `0`
* **Every time** the button is clicked, the value should be **incremented** by `1`

**OPTIONAL** : The current count is stored inside a [JSONModel](https://openui5.hana.ondemand.com/api/sap.ui.model.json.JSONModel)

**OPTIONAL** : Update the label of the button with the current value of the counter : *Count (0)* 

### Limit the count

* When the count **reaches `10`**, the button should **not be clickable** anymore

### Reset the count

* Add a button that resets the state of the application every time it is clicked :
  - The counter is reset to `0`
  - The count button is clickable again