# memo

https://create-react-app.dev/docs/running-tests/

- element 関連のテスト：login.test.tsx
- Event(fireEvent), change, click :
- jest.spyOn(
- async waitForElement, mock resolve

## install

```
npx create-react-app jest-react --template typescript
npm install axios
yarn add -D @types/react

// ??
npm run-script build // ??不要かも
npm start

npm test

npm test -- --coverage --watchAll=false
```

## cors error 対応

- TSTestCourse の Server に下記を追加

```
this.addCorsHeader(res);

  private addCorsHeader(res: ServerResponse) {
    res.setHeader('Access-Control-Allow-Origin', '*');
    res.setHeader('Access-Control-Allow-Methods', '*');
    res.setHeader('Access-Control-Allow-Headers', '*');
  }
```
