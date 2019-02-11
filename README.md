# nhDev.io Express template

### Specifications
**Server**: node/express

**CSS Preprocessor**: SASS

**HTML Preprocessor**: Pug

For bootstrapping express sites. 

To initialize after clone
```
npm update
```

To start testing server
```
npm start
```

To add a page, create a new pug file in the views folder. 
Add the route to express in index.js 

```
app.get('/some_route', (req, res) => {
  res.render('some_view');
});
```

To pass data to the template, include the variables as an object in the render method.
```
app.get('/', (req, res) => {
  res.render('index', { step: 1 });
});
```

You can then use the variable in the pug template
```
h2 Step #{step}| Worksheets
```