# React Redux TypeScript

# Arhitectura app files

* bus - bissness logict 
* elements - "components" render some groups of view

# Setting 

*  yarn create react-app . --template typescript
*  yarn add -D eslint-config-airbnb
*  yarn add -D prettier-eslint-cli
*  yarn add -D eslint-plugin-import


* yarn add redux-logger  (and for the type 'yarn add -D @types/redux-logger')
* yarn add redux-saga
* yarn add redux react-redux  ( + yarn add -D @types/react-redux)
* yarn add redux-devtools-extension


```
    "lint": "yarn typescript && yarn lint:ts",
    "lint:ts": "eslint './src/**/*.{ts,tsx}'",
    "prettier:ts": "prettier-eslint --list-different $PWD/'src/**/*.{ts,tsx}'; prettier-eslint --write $PWD/'src/**/*.{ts,tsx}'",
    "typescript": "tsc"
```


# Saga



# extras 

# useSelector + type for the state :)

* [redux-hooks](https://levelup.gitconnected.com/react-redux-hooks-useselector-and-usedispatch-f7d8c7f75cdd)
```
export type AppState = ReturnType<typeof  rootReducer>
const counter = useSelector( (state: AppState) => state.counter)
```


# TS + GQL
* apollo:download-schema To download schema
* generate-types shema Convert to ts the codse if it needed.


```
"apollo:download-schema": "apollo client:download-schema --endpoint 'https://example.com/'"
"apollo:generate-types": "apollo client:codegen --LocalSchemaFile 'schema.json' --target 'typescript'"
```
