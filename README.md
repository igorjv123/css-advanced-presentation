# React Hooks

## Presentation

### Setup

```bash
npm install
```

### Start

```bash
npm start
```


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="./main.css">
    <title>Document</title>
</head>
<body>
    <div class="spinner-wrapper">
        <div class="spinner-back">
            <div class="spinner-inner"></div>
        </div>
</div>
    
    
</body>
</html>



*{
    margin: 0;
    padding: 0;
}
.spinner-wrapper{
    animation: rotation 2s infinite;
    width: 100px;
    animation-direction: alternate;

}
.spinner-back {
    width: 100px;
    height: 100px;
    background-color: #ddd;
    border-radius: 50%;
    animation: spin 2s infinite;
    overflow: unset;
    
}
.spinner-back::after {
    content: '';
    width: 20px;
    height: 20px;
    background-color: yellow;
    position: absolute;
    left: 40px;
    z-index: 4;

}
.spinner-inner {
    width: 70px;
    height: 70px;
    background-color: #fff;
    border-radius: 50%;
    position: absolute;
    top: 15px;
    left: 15px;
    z-index: 5;
}
@keyframes rotation {
    to {
        transform: rotateY(180deg);
    }
}
@keyframes spin {
    to {
        transform: rotate(360deg);

    }
}


