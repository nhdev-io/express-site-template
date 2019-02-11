# nhDev.io Express template

## Specifications
#### Platform
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
npm update
npm start
```

To add a page, create a new pug file in the views folder. 
Add the route to express. 

```
app.get('/some_route', (req, res) => {
  res.render('some_view');
});
```