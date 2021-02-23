# Flex Box

### Com Flex box é possível fazer alinhamento, posicionamento de objetos de um mandeira muito mais pratica

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Curso de FlexBox</title>
    <link href="app.css" rel="stylesheet">
  </head>
  <body>
      <div id="app">
        <div class="box red"></div>
        <div class="box green"></div>
        <div class="box blue"></div>
      </div>
  </body>
</html>
```

```css
*{
  /* zero as configuraçções padrões do navegador e etc */
  margin:0;
  padding:0;
  box-sizing: border-box;  /* faz com que o padding não aumente o tamanho do meu controller */
 
}
html, body, #app{
  height: 100%;
  margin: 0;
}
#app{
  display: flex; /* por padrão o flex direction fica como row */
  
flex-wrap: wrap;
}

.box{
  background-color: red;
  /*align-itens: defini o alimento verticalmente na pagina para quando o flex direction está em row*/
  width:700px;
  height: 200px;
  margin:5px;
/*align-content: é utilizado quando os elementos estão em mais de uma linha, ou seja, quebrando, no caso quando se poem no container flex wrap: wrap*/
}

.red{
  order:0;
}

.green{
background: green;
order: 3;
}

.blue{
  background: blue;
  order: 2
}
```

