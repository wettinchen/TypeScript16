## TypeScript 16
## Chapter 16: Shopping Cart-Part 1
It is my coding practice with the TUTORIAL of Dave Gray. 

## Source
### Dave Gray 的 TypeScript 資源
https://github.com/gitdagray/typescript-course

### Dave Gray 的 TypeScript 課程
https://youtube.com/playlist?list=PL0Zuz27SZ-6NS8GXt5nPrcYpust89zq_b&si=8IJALfXOcur2OO_K

### Dave Gray 的 YouTube 頻道
https://www.youtube.com/@DaveGrayTeachesCode

## Quick Concept offline
###  1. Intro
        教學影片開頭和介紹

###  2. Welcome

###  3. Project Overview

###  4. Creating the Project with Vite
        (1)在 terminal 輸入 npm create vite@latest
        (2)設定專案名稱
        (3)選取框架 React，變體選擇 TypeScript
        (4)開啟專案資料夾
        (5)在 terminal 輸入 npm i，安裝
        (6)在 terminal 輸入 npm run dev，執行
        (7)刪除 App.css
        (8)修改 index.css
        (9)新增 counter.tsx
        (10)修改 App.tsx

###  5. Adding Product Data
        (1)新增資料夾 data
        (2)新增 products.json

###  6. Components & Context Overview
        (1)新增資料夾 component
        (2)新增資料夾 context

###  7. Product Images
        (1)新增資料夾 images
        (2)新增 item0001.jpg, item0002.jpg, item0003.jpg

###  8. Products Context
        (1)新增 ProductProvider.tsx
        (2)匯出 ProductType 類型
        (3)宣告 initState
        (4)匯出 UseProductsContextType 類型
        (5)宣告 initContextState
        (6)宣告 ProductsContext
        (7)匯入 createContext
        (8)設定 ChildrenType 類型
        (9)匯出 ProductsProvider
        (10)匯入 ReactElement
        (11)匯入 useState
        (12)回傳 ProductsContext.Provider 元素
        (13)匯出 ProductsContext

###  9. Promise, Fetch, useEffect & json-server
        (1)修改 initState
        (2)匯入 useEffect
        (3)使用 useEffect
        (4)在 terminal 輸入 npx json-server -w data/products.json -p 3500

### 10. Cart Context Reducer
        (1)新增 CartProvider.tsx
        (2)匯出 CartItemType 類型
        (3)設定 CartStateType 類型
        (4)宣告 initCartState
        (5)宣告 REDUCER_ACTION_TYPE
        (6)匯出 ReducerActionType
        (7)匯出 ReducerAction
        (8)宣告 reducer，使用 switch 描述式

### 11. useCartContext hook
        (1)宣告 useCartContext
        (2)匯入 useReducer
        (3)使用 useReducer
        (4)匯入 useMemo
        (5)宣告 REDUCER_ACTIONS，使用 useMemo
        (6)宣告 totalItems
        (7)宣告 totalPrice
        (8)宣告 cart
        (9)回傳 dispatch, REDUCER_ACTIONS, totalItems, totalPrice, cart

### 12. Create the Cart Context
        (1)匯出 UseCartContextType
        (2)宣告 initCartContextState
        (3)匯出 CartContext
        (4)匯入 createContext

### 13. Cart Provider
        (1)設定 ChildrenType
        (2)匯出 CartContext
        (3)設定 ChildrenType 類型
        (4)匯出 CartProvider
        (5)匯出 CartContext

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
   parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
   },
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
