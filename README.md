# ReactJS Lojeris

## Étapes d'installation

### Installation de react-router

```shell script
npm install react-router-dom
```

Modifier le fichier index.js pour charger le router :
```jsx
import {BrowserRouter} from "react-router-dom";

ReactDOM.render(
  <React.StrictMode>
    <BrowserRouter>
      <App />
    </BrowserRouter>
  </React.StrictMode>,
  document.getElementById('root')
);
```

### Installation de Redux

```shell script
npm install --save redux react-redux redux-devtools-extension
```
Créer un fichier reducer


Créer le fichier pour combiner les reducers :

```javascript
import {combineReducers} from 'redux';
import monReducer from './monReducer';

export default combineReducers({ monReducer });
```