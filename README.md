# polymer-model
Model layer for Polymer apps with a REST backend

```html
<link rel="import" href="polymer/polymer.html" />
<link rel="import" href="polymer-model/polymer-model.html" />

<h1>{{ a_thing.title }}</h1>

<polymer-model auto 
    baseUrl="/things/" 
    modelId="15"
    model="{{ a_thing }}"></polymer-model>
```

#### Attributes

1. **baseUrl**
2. **modelId**
3. **model**
4. **collection**
5. **query**

#### Methods

1. **.get()**
2. **.save()** (issues a POST or PUT request, depending on the `modelId`)
3. **.delete()**
