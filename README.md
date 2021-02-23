# bootstrap4

## DONT USE

```
<div class="container">
  <div class="row">
    <div class="col-12">
      <div class="row">
        <Welcome name="Sara" />
        <Welcome name="Cahal" />
        <Welcome name="Edite" />
      </div>
    </div>
  </div>
</div>
```

This will make Block elements in rows display like inline-block in Bootstrap 4

https://stackoverflow.com/a/48643939

> You are NOT supposed to place any content into a .row directly. 

> Instead, put a column (.col-*) into a row and then put your content inside the column(s).

> Rows and columns in Bootstrap are designed to work as a pair. Never alone.

> So, if you just need one column that fills out the entire width of the row, then you put a div with the col class inside your row and that's it.

```
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

<div class="container">
    <div class="row">
        <div class="col">
            <h1>Hello, world!</h1>
            <p>This is a paragraph</p>
        </div>
    </div>
</div>
```


So instead use

```
<div class="container">
  <div class="row">
    <div class="col-12">
      <Welcome name="Sara" />
      <Welcome name="Cahal" />
      <Welcome name="Edite" />
    </div>
  </div>
</div>
```
